Preconfigured Sonata Admin
=========

This project is a preconfigured setup of SonataAdminBundle with default RTL support

## Features
- Doctrine ORM
- ckeditor
- rest configs (withoud nelmio doc bundle)
- liipImagine
- symfonyjdate
- vichUploader

## Installation
Download the ZIP file and install dependencies using composer

## Configs
### Sonata
Sonata RTL stylesheets are located in `web/assets/css`. This files are used in twig's global parameters and are read by `app\Resources\SonataAdminBundle\views\standard_layout.html.twig:53`. Changing application default locale will also affect the layout directions in Sonata dashboard.
