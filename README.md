# docker-wordpress   
Wordpress - MySQL - PhpMyAdmin stack in Docker   
### Start WordPress in docker with only 2 commands 
You need to have docker and docker compose installed.    
If you don't have them, see [here](http://www.spiralout.eu/2015/12/docker-installation-in-linux-mint-and.html) first.
```
$ git clone git@github.com:SpiralOutDotEu/docker-wordpress.git   
$ cd docker-wordpress && docker-compose up   
```
You are ready!   
Go to [0.0.0.0:8000](http://0.0.0.0:8000) and start building your WordPress site.   
Go to [0.0.0.0:8081](http://0.0.0.0:8081) and play with PhpMyAdmin.   
You credentials for phpMyAdmin is what you declared in `docker-compose.yml`   
```
    environment:
      MYSQL_ROOT_PASSWORD: wordpress
      MYSQL_DATABASE: wordpress
      MYSQL_USER: wordpress
      MYSQL_PASSWORD: wordpress
```
Have fun!

