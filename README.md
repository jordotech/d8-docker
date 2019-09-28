This is a modified version of [docker4drupal](https://github.com/wodby/docker4drupal), for full instructions on using the stack go there.  
This version will get you up and running locally with less steps.

Clone this repo to your local and perform the following:

1. add the following to your hosts file (osx: /private/etc/hosts) `127.0.0.1  drupal.docker.localhost`
2. create your settings.php in ./drupal/sites/default with [this content](https://gist.github.com/jordotech/f0c7726bc6212881287ae1872bf3c313)
3. bring the project up with `docker-compose up -d`. This will build your containers and perform the initial `composer install`
as well as import a small db so you don't even have to do site install.

After it's done (composer install takes a long time) go to drupal.docker.localhost:8000 and the site should be running.

The initial user and password are admin/admin
