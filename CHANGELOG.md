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
