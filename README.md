# afterWork2

###Installation

```
docker-compose build


docker-compose up -d

docker exec -it symfonyApp bash 

composer update

bin/console doctrine:database:create --if-not-exists

bin/console doctrine:schema:update --force
```

###Local Environment


- App URL : http://localhost:8080/
- Mysql url: http://localhost:3306 
- Db : afterwork 
###PhpMyAdmin 
- URL : http://localhost:8090 
- Login : root 
- Password : root


###Symfony command

Mise à jour de la Database
```
php bin/console doctrine:migrations:diff
php bin/console doctrine:migrations:migrate

```

ce rajouter le role admin

```
bin/console fos:user:promote <votrenomutilisateur> ROLE_ADMIN
```


### Lien Serveur de Prod

http://after-tech.fr/

DATABASE_URL=mysql://root:root@symfonyDb:3306/afterwork

travisCi
