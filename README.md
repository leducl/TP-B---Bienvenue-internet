Analyse d'une Requête HTTP
1. Quelle est la structure de la ligne GET / HTTP/1.1 ?
Cette ligne se compose de trois éléments principaux :

GET : méthode HTTP qui indique qu'on souhaite récupérer une ressource.

/ : chemin de la ressource demandée (ici, la racine du site).

HTTP/1.1 : version du protocole HTTP utilisée pour la requête.

2. Pourquoi faut-il appuyer deux fois sur Entrée pour que le serveur réponde ?
La ligne vide indique la fin de la requête. Sans cette ligne, le serveur attend encore car il pense que la requête est incomplète.

3. Que se passe-t-il si vous oubliez cette ligne vide ?
Le serveur ne répond pas. Il attend toujours la fin de la requête car il croit qu'elle n’est pas terminée.

4. Que signifie le code 200 OK dans la réponse ? Que signifient les codes 404 ou 301 ?
200 OK : la requête a réussi, la ressource a été trouvée.

404 Not Found : la ressource demandée n’existe pas.

301 Moved Permanently : la ressource a été déplacée de façon permanente vers une autre URL.

5. Quelle est la toute première ligne envoyée par le serveur ?
Exemple :

Copier
Modifier
HTTP/1.1 200 OK
Cette ligne contient :

La version du protocole,

Le code de réponse,

Le message associé au code.

6. Relevez les entêtes présents dans la réponse : à quoi servent-ils ?
Content-Type : type du contenu (ex. : text/html, image/png, etc.).

Content-Length : taille du contenu en octets.

Date : date et heure de la réponse.

Server : information sur le serveur ayant répondu.

7. Quelle est la première ligne non entête du corps ? À quoi reconnaît-on la séparation ?
La première ligne du corps est souvent :

html
Copier
Modifier
<!DOCTYPE html>
ou une balise <html>.
La séparation entre entêtes et corps se fait grâce à une ligne vide.

8. Que se passe-t-il si vous tapez une URL invalide (ex : GET /truc HTTP/1.1) ?
Le serveur renvoie un code 404 Not Found : la ressource n'existe pas.

9. Le contenu retourné dans ce cas est-il aussi du HTML ? Que contient-il exactement ?
Oui, même en cas d’erreur 404, le contenu est souvent en HTML. Il contient une page d’erreur expliquant que la ressource demandée est introuvable.
