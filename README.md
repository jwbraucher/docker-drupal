# braucher/drupal 1.1.0

This [braucher/drupal](https://hub.docker.com/r/braucher/drupal/) docker image provides an Ubuntu 14.04 drupal application container.

The [braucher/drupal](https://hub.docker.com/r/braucher/drupal/) image also includes the following:

* drush
* postfix
* /app* entrypoint scripts

## Usage

By default, ```/app start``` is the entrypoint and command, 
the daemon listens on port 9000, and files are served from /var/www/app.
Run ```/app install``` to install drupal.
Run ```/app backup``` to backup the drupal installation

See the
[docker-compose.yml from the sample-project branch](https://github.com/jwbraucher/docker-drupal/tree/sample-project/docker-compose.yml)
for an example of how to build a new project from this image using the
following Docker images:

* [braucher/drupal](https://hub.docker.com/r/braucher/drupal/) (this one)
* [braucher/fcgi](https://hub.docker.com/r/braucher/fcgi/)
* [mysql](https://hub.docker.com/r/_/mysql/)

If you fork the sample-project branch, modify the following files:
* Makefile.local 
* docker-compose.yml
app/app.*

### Environment Variables

Whenever this container starts it re-configures drupal.
Be sure to supply the correct runtime environment variables when
you first launch the containers. Docker will remember the environment
variables for subsequent container restarts.

See the [/app.env script](https://github.com/jwbraucher/docker-drupal/tree/latest/app/app.env)
for all accepted parameters. 

## Development
See DEVELOPMENT.md

## License
MIT license

