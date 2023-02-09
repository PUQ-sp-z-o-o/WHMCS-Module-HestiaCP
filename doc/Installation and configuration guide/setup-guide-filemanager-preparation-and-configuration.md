# Setup guide: Filemanager preparation and configuration

#####  [Order now](https://panel.puqcloud.com/index.php?rp=/store/whmcs-module-hestiacp) | [Dowload](https://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-HestiaCP/) | [FAQ](https://faq.puqcloud.com/)

### 1. Simple installation Filemanager

##### 1. Prepare hosting for the file manager.

<p class="callout info">**Minimum Requirements:** PHP 7.2.5+ (with php-zip extension)</p>

##### 2. Download the latest version filemanager from the module folder.<textarea readonly="readonly" spellcheck="false" style="position: absolute; bottom: -1em; padding: 0px; width: 1px; height: 1em; outline: currentcolor none medium;" tabindex="0" wrap="off"></textarea>

```
wget http://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-HestiaCP/filemanager/filemanager.zip
```

<p class="callout info">All versions are available via link: [http://download.puqcloud.com/WHMCS/servers/PUQ\_WHMCS-HestiaCP/filemanager/](http://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-HestiaCP/filemanager/)</p>

##### 2. Unzip the archive with the Filemanager and upload them to your PHP server

```
unzip filemanager.zip
```

##### 3. Make sure your webserver can read and write to `../repository/` and `../private/` folders

##### 4. Set the website document root to `../dist/` directory. This is also known as 'public' folder

<p class="callout warning">**NOTE:** For security reasons `filegator/dist` is the ONLY folder you want to be exposed through the web. Everything else should be outside of your web root, this way people can’t access any of your important files through the browser. If you run the script from the root folder, you will see the message 'Development mode' as a security warning.</p>

### 2. A<span class="HwtZe" lang="en"><span class="jCAhz ChMk0b C1N51c"><span class="ryNqvb">dvanced</span></span></span> installation Filemanager

#### 1. Installing a file manager

<section class="col-sm-offset-3 col-lg-offset-2 col-sm-9 col-lg-10" id="bkmrk-minimum-requirements-0" style="padding-left: 40px;"><p class="callout info">The original instructions for installing and configuring the file manager [https://docs.filegator.io/install.html](https://docs.filegator.io/install.html)</p>

<p class="callout info">Minimum Requirements: PHP 7.2.5+ (with php-zip extension)</p>

##### Download precompiled build

Precompiled build is created for non-developers. In this version, the frontend (html, css and javascript) is compiled for you and the source code is removed so the final archive contains only minimum files.

- - - Download the [latest release](https://github.com/filegator/static/raw/master/builds/filegator_latest.zip)
        - Unzip files and upload them to your PHP server
        - Make sure your webserver can read and write to `filegator/repository/` and `filegator/private/` folders
        - Set the website document root to `filegator/dist/` directory. This is also known as 'public' folder
        - Visit web page, if something goes wrong check `filegator/private/logs/app.log`

<p class="callout warning">NOTE: For security reasons `filegator/dist` is the ONLY folder you want to be exposed through the web. Everything else should be outside of your web root, this way people can’t access any of your important files through the browser. If you run the script from the root folder, you will see the message **'Development mode'** as a security warning.</p>

##### Install on fresh Ubuntu 18.04 or Debian 10.3

On a new server login as root and enter this into the shell:

```
apt update<br></br>apt install -y wget unzip php apache2 libapache2-mod-php php-zip php-mbstring php-dom php-xml<br></br><br></br>cd /var/www/<br></br>wget https://github.com/filegator/static/raw/master/builds/filegator_latest.zip<br></br>unzip filegator_latest.zip && rm filegator_latest.zip<br></br><br></br>chown -R www-data:www-data filegator/<br></br>chmod -R 775 filegator/<br></br><br></br>echo "<br></br><VirtualHost *:80><br></br>    DocumentRoot /var/www/filegator/dist<br></br></VirtualHost><br></br>" >> /etc/apache2/sites-available/filegator.conf<br></br><br></br>a2dissite 000-default.conf<br></br>a2ensite filegator.conf<br></br>systemctl restart apache2<br></br><br></br>exit
```

Open your browser and go to http://your\_server\_ip\_address

##### Show your support

- - - Please star this repository on [GitHub](https://github.com/filegator/filegator/stargazers) if this project helped you!

##### Upgrade instructions

- - - Backup everythig
        - Download the latest version
        - Replace all files and folders except `repository/` and `private/`

Which versions am I running? Look for `APP_VERSION` inside `dist/index.php` file

</section>#### 2. Installing API script and file manager configuration script

##### 1. Download the latest version API script and file manager configuration script from the module folder.<textarea readonly="readonly" spellcheck="false" style="position: absolute; bottom: -1em; padding: 0px; width: 1px; height: 1em; outline: currentcolor none medium;" tabindex="0" wrap="off"></textarea>

```
wget http://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-HestiaCP/filemanager/api/Filegator-api-for-HestiaCP-module.zip
```

<p class="callout info">All versions are available via link: [http://download.puqcloud.com/WHMCS/servers/PUQ\_WHMCS-HestiaCP/filemanager/api/](http://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-HestiaCP/filemanager/api/)</p>

##### 2. Unzip the archive with the API script and file manager configuration script and upload them to your PHP server

```
unzip Filegator-api-for-HestiaCP-module.zip
```

<p class="callout warning">Attention! **The configuration.php file must be located in the root folder** of your file manager. The api.php **file must be located in the /dist folder** of your file manager.</p>