# Drupal 8 Workbench Moderation to Content Moderation Migration Concept

This is a proof of concept of how to migrate from Workbench Moderation to Content Moderation in Drupal 8.4.

# Requirements

1. [Composer](https://getcomposer.org/)
2. [Drush 9.x](https://www.drush.org/) ([link to core 8.4 support in drush 8](https://www.drupal.org/node/2874827))

NOTE: In order to get drush 9.x installed in this repo, phpunit has been removed due to a dependency version conflict between drush and the version of phpspec that phpunit requires.

# Getting Started

NOTE: these instructions only apply to the wbm-upgrade branch:

1. Create a Drupal.

    ```
    $ composer create-project josephdpurcell/drupal8_wbm2cm_concept-project MY_PROJECT --no-interaction --stability dev
    ```

    This will create a directory `MY_PROJECT`. Inside of it will be a directory `web` which is the website's docroot.

2. Install the Drupal.

    ```
    drush si
    ```

    or

    go to `/install.php`.
