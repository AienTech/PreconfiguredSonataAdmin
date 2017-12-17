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
Configuration detailsand instructions:
### Sonata RTL support and Locale
Sonata RTL stylesheets are located in `web/assets/css`. This files are used in twig's global parameters and are read by `app\Resources\SonataAdminBundle\views\standard_layout.html.twig:53`. Changing application default locale will also affect the layout directions in Sonata dashboard.
### Sonata Admin Theme
To change sonata admin dashboard theme (colors etc.), just download the [AdminLTE Full Theme](https://github.com/almasaeed2010/AdminLTE) and change the colors in `build/less/skins/skin-{color you want to customize}.less`. Then configure `Gruntfile.js` to get the correct output file (export the output css to your `web/assets/css` folder).
After that, add the following files to sonata stylesheets (Both RTL and LTR):
- `assets/css/AdminLTE.min.css`
- `assets/css/skins/_all-skins.min.css`
- `assets/css/admin-custom.css`

Don't forget to remove `bundles/sonataadmin/vendor/admin-lte/dist/css/AdminLTE.min.css` and `bundles/sonataadmin/vendor/admin-lte/dist/css/skins/skin-black.min.css` from both RTL and LTR configurations