## This Repo will only be used to implement drupal advance features like Drupal Behaviours, Mega Multi Level Menu, Responsive Design, Drupal Paragraphs, Theme Preprocess, Mastering Twig & other complex problems

## PR #1 (Responsive Design): DRPL-001
## PR #2 (Some Twig Mastering): DRPL-002
## PR #3 (Theme Preprocess): DRPL-003
## PR #4 (Drupal Paragraphs): DRPL-004
## PR #5 (Mega Menu): DRPL-005
## PR #6 (Drupal Behaviours): DRPL-006
## PR #7 (Some Drupal): DRPL-007

## Figma Refrence Design (HomePage) Only
 - https://www.figma.com/file/s2nsvgGV3BtPcSygtEeGNv/Portfolio_Responsive_Template_from_Laaqiq?node-id=101%3A412&t=nTahQU4SPH8UOvIV-1

# Local setup guide

## Using ddev

1. Starting the project and installing the dependencies

- `ddev start`
- `ddev composer install`
- `ddev drush si`

2. quick checks:

   - check if composer is working properly
     `ddev composer`
   - check if drush is working properly
     `ddev drush`
   - check if node is working properly
     `ddev exec node --version`

3. Goto [https://oneseven.ddev.site/](https://oneseven.ddev.site/)

4. Theme build tasks
   - Install all the dependecies
     ddev exec -d /var/www/html/web/themes/custom/drupalastic yarn
   - Start the development server and watch assets for changes to compile
     ddev exec -d /var/www/html/web/themes/custom/drupalastic yarn start
   - Build assets for production
     ddev exec -d /var/www/html/web/themes/custom/drupalastic yarn build
   - Lint assets
     ddev exec -d /var/www/html/web/themes/custom/drupalastic yarn lint
