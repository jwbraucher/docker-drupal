# braucher/drupal 1.3.1

## Bugfixes
  - fixed php_home and app_home to be compatible with new php image
  - fixed shell vars in app.restore

# braucher/drupal 1.3

## Features
  - Merged in docker/app-1.4

# braucher/drupal 1.2.1

## Bugfixes
  - don't start after install or restore
  - always start/restart with command=start to preserve containers on restart
  - ls-volumes is now volumes. Improved volumes output.

# braucher/drupal 1.2.0

## Features
  - made Drupal start after restore

## Bugfixes
  - make clean preserves export volume
  - sudo -u www-data can now read /root/.drush
  - drush install --yes instead of yes | drush install

# braucher/drupal 1.1.0
  - added ‘make backup’ and ‘make restore’
  - ‘make clean’ will not erase backups (excludes volumes/export)

# braucher/drupal 1.0.0
  - first version, based off braucher/php and braucher/wordpress
  - installs drush
  - app.install script to install Drupal on boot
