

This is a forked version of Gitlist that contains edits used for my own purposes on https://repos.brandonrozek.com

For the main project, please go to https://github.com/klaussilveira/gitlist

## Requirements
In order to run GitList on your server, you'll need:

* git
* Apache with mod_rewrite enabled or nginx
* PHP 5.3.3

## Installation
* Download GitList from [gitlist.org](http://gitlist.org/) and decompress to your `/var/www/gitlist` folder, or anywhere else you want to place GitList. 
* Do not download a branch or tag from GitHub, unless you want to use the development version. The version available for download at the website already has all dependencies bundled, so you don't have to use composer or any other tool
* Rename the `config.ini-example` file to `config.ini`.
* Open up the `config.ini` and configure your installation. You'll have to provide where your repositories are located.
* In case GitList isn't accessed through the root of the website, open .htaccess and edit RewriteBase (for example, /gitlist/ if GitList is accessed through http://localhost/gitlist/).
* Create the cache folder and give read/write permissions to your web server user:

```
cd /var/www/gitlist
mkdir cache
chmod 777 cache
```

That's it, installation complete! If you're having problems, check the [Troubleshooting](https://github.com/klaussilveira/gitlist/wiki/Troubleshooting) page.


## Authors and contributors
* [Klaus Silveira](http://www.klaussilveira.com) (Creator, developer)

## License
[New BSD license](http://www.opensource.org/licenses/bsd-license.php)

