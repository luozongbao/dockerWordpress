# dockerLEMP
I create docker compose for a LEMP stack for at least can run wordpress in development environment.  For better understanding how to make this please watch Andrew Schmelyun's Chanel on this at [this link](https://www.youtube.com/watch?v=kIqWxjDj4IU)

## Initial data
1. simply put the sql file in the "initdb" folder
2. On spin up, the composer will import all data in the file to a new database same name as the sql file.

## conf.d
I created 2 versions of .conf files
1. the default.conf will be use everything recommended by the experts
2. the min.conf will be just only the part needed to run (on experiment) 

## wordpress
1. simply download zip file and unzip
2. edit docker-compose.yml file and point the volume in php and nginx to
```
volumes:
  - ./wordpress:/var/www/html
```
3. spin up the containers
