# Setup guide: Downloading backups description and configuration

#####  [Order now](https://puqcloud.com/whmcs-module-hestiacp.php) | [Download](https://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-HestiaCP/) | [FAQ](https://faq.puqcloud.com/)

In order to gain the ability to download backups directly from the WHMCS billing system, you can use this functionality. This feature is implemented by deploying a custom script to the root directory of the administrator's website. Once the script is created, users will be able to download backups by exchanging tokens and hashes between the billing system.

<p class="callout info">Note: Only the admin account has access to the backup files. Only those sites that were created in the administrator account will have access to backups</p>

In order for the backup to be downloaded, it is necessary to create a new template based on the existing one with a suitable configuration for example:

1\. Copy an existing template with a custom name

```
cp /usr/local/hestia/data/templates/web/php-fpm/PHP-8_1.tpl /usr/local/hestia/data/templates/web/php-fpm/download_backups.tpl
```

2\. Let's edit the created template, add a directory with backups to the line with `php_admin_value[open_basedir]`, at the end of the line

```
nano /usr/local/hestia/data/templates/web/php-fpm/download_backups.tpl
```

The line will look something like this:

```
php_admin_value[open_basedir] = /home/%user%/.composer:/home/%user%/web/%domain%/public_html:/home/%user%/web/%domain%/private:/home/%user%/web/%domain%/public_shtml:/home/%user%/tmp:/tmp:/var/www/html:/bin:/usr/bin:/usr/local/bin:/usr/share:/opt:/backup
```

3\. Activate the template on the server

[![Снимок экрана 2023-04-26 002743.png](https://doc.puq.info/uploads/images/gallery/2023-04/scaled-1680-/snimok-ekrana-2023-04-26-002743.png)](https://doc.puq.info/uploads/images/gallery/2023-04/snimok-ekrana-2023-04-26-002743.png)