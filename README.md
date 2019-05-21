## Docker Compose - Laravel Multi-Site LEMPR Stack
A docker compose configuration for local Laravel development with Linux, nGinx, MySql, PHP-7.3, and Redis.

this is used on a windows system, have not tested on Mac or Linux yet.

#### pre-reqs

- must have a ```$home/sites``` folder with ```$home``` being your user directory.
- must symlink your desired laravel project into the sites folder ```mklink /J $home/sites/name.test /path/to/your/laravel/root```
- docker will require your local drive to be shared in your ```Docker Settings -> Shared Drives```



## Building, Starting, and Stopping

start by creating the images:
```docker-compose build```

if there were no errors, you should be able to start the server:
```docker-compose up```

when down:
```docker-compose down```


## Logging
if you need to look at nginx logs:
```docker logs laravel_multi_lempr_websrv_1```  
changing ```laravel_multi_lempr_websrv_1``` depending on your container
