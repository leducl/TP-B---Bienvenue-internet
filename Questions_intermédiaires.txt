Quelle est la structure de la ligne GET / HTTP/1.1 ? Quels sont les trois éléments et leur rôle ?

La ligne contient GET, qui est la méthode pour demander une ressource. Ensuite /, qui est l’adresse de la ressource (ici la racine du site). Enfin HTTP/1.1, qui est la version du protocole utilisée.

2. Pourquoi faut-il appuyer deux fois sur Entrée pour que le serveur réponde ? Que représente cette ligne vide dans le protocole HTTP ?

La ligne vide sert à dire qu’on a fini d’envoyer la requête. Sans cette ligne vide, le serveur pense qu’on n’a pas fini et il attend encore.

3. Que se passe-t-il si vous oubliez cette ligne vide ? Le serveur répond-il quand même ?

Non, le serveur ne répond pas. Il attend toujours la fin de la requête car il croit qu’on n’a pas terminé.

4. Que signifie le code 200 OK dans la réponse ? Qu’indique un code 404 ou 301 ?

Le code 200 OK veut dire que tout s’est bien passé et que la ressource a été trouvée. Le 404 veut dire que la ressource n’existe pas. Le 301 veut dire que la ressource a été déplacée ailleurs.

5. Quelle est la toute première ligne envoyée par le serveur ? Que contient-elle ?

La première ligne est par exemple HTTP/1.1 200 OK. Elle contient la version du protocole, le code de réponse, et le message expliquant le code.

6. Relevez les entêtes présents dans la réponse (Content-Type, Content-Length, etc.) : à quoi servent-ils ?

Content-Type indique le type de contenu (par exemple du HTML ou une image).
Content-Length donne la taille du contenu.
Date indique quand la réponse a été envoyée.
Server donne le nom du serveur qui a répondu.

7. Quelle est la première ligne non entête du corps ? À quoi reconnaît-on la séparation ?

La première ligne du corps est souvent <!DOCTYPE html> ou une balise <html>. On reconnaît la séparation avec la ligne vide qui termine la partie des entêtes.

8. Que se passe-t-il si vous tapez une URL invalide (ex : GET /truc HTTP/1.1) ? Quel est le code de retour ?

Le serveur répond avec le code 404 Not Found car il ne trouve pas la ressource demandée.

9. Le contenu retourné dans ce cas est-il aussi du HTML ? Que contient-il exactement ?

Oui, même en cas d’erreur 404, le serveur envoie souvent du HTML. Ce HTML contient un message d’erreur disant que la page n’a pas été trouvée.
