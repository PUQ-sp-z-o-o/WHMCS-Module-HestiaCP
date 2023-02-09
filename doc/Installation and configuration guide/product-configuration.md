# Product Configuration

#####  [Order now](https://panel.puqcloud.com/index.php?rp=/store/whmcs-module-hestiacp) | [Dowload](https://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-HestiaCP/) | [FAQ](https://faq.puqcloud.com/)

##### Add new product to WHMCS

```
System Settings->Products/Services->Create a New Product
```


In the **Module settings** section, select the **"PUQ HestiaCP"** module

[![image-1672998951322.png](https://doc.puq.info/uploads/images/gallery/2023-01/scaled-1680-/image-1672998951322.png)](https://doc.puq.info/uploads/images/gallery/2023-01/image-1672998951322.png)

- **License key:** A pre-purchased license key for the **"PUQ HestiaCP"** module. For the module to work correctly, the key must be active
- **Chose pakage on server:** The list of packages is pulled from the server. Will be used when the **"Use the package parameters"** option is not selected. And also if for some reason it will not be possible to create a custom package. <p class="callout warning">**Attention!** To deploy a custom package, you must set the interface language for the account administrator to English.</p>
- **Use the package parameters:** The option allows you to make a choice of settings. Whether you want to use the packages already configured on the server or upload a customized custom package. Use the package parameters entered below, and create the package if it does not exist on the server. And if there is a package, then change its values to those entered below.
- **Filemanager settings:** File manager settings  
    
    - **Hostname:** The hostname of the file manager
- **Pakage configuration:** Setting up a custom package  
    
    - **Name pakage:** The package name entered will be used to configure the custom package if the option is selected **"Use the package parameters"**
    - **Quota:** The disk quota that is given to the user in the system. Set in megabytes
    - **Bandwidth:** Bandwidth Limit that is given to the user in the system. Set in megabytes
- **WEB Pakage configuration:** Setting up a web section for a custom package 
    - **Web Domains:** The number of web domains allowed per user in the package
    - **Web Aliases:** The number of web aliases allowed for each domain in the package
- **SSH Access:** Selecting a user access template for SSH Access. The list is loaded from the connected server
- **Databases Pakage configuration:** Section for database configuration in a custom package 
    - **Databases:** The number of databases allowed for the user
- **DNS Pakage configuration:** DNS section configuration for custom package 
    - **DNS Zones:** The number of DNS zones allowed in the package for the user
    - **DNS Records:** The number of DNS records in each domain zone allowed in the package for the user
    - **Name Servers:** Nameservers configuration in custom package
- **System Pakage configuration:** System settings section, custom package 
    - **Cron Jobs:** The number of cron jobs that are allowed for the user
    - **Template settings**: If you want to control the display of templates in Client Area, activate this option. Your template name should be **default.tpl**, **no-php.tpl**, **socket.tpl**, **PHP-5\_6.tpl, PHP-7\_0.tpl, PHP-7\_1.tpl, PHP-7\_2.tpl, PHP-7\_3.tpl, PHP-7\_4.tpl, PHP-8\_0.tpl, PHP-8\_1.tpl, "custom\_name".tpl** this name will be displayed in Client Area. And match your "custom\_name" in "custom\_name".tpl on HestiaCP server. Each of the templates is activated separately. <p class="callout warning">**Attention!** If the specified heatplate name is not found on the server, then the heatplate will not be available to Client Area. If the option is disabled, all templates available on the server will be available for selection by the client!</p>
- **Backups:** Backup configuration in custom package 
    - **Backups:** The number of backup copies that are allowed for the user
- **Mail Pakage configuration:** Mail settings section, custom package 
    - **Mail Domains:** Number of email domains allowed for a user
    - **Mail Accounts:** Number of email accounts per email domain allowed for a user
- **Web templates:** Choosing a template Web Template <span class="optional"> APACHE2. The list of templates is loaded from the server</span>
- **Web templates backend:** Choosing a Backend Template <span class="optional">PHP-FPM. The list of templates is loaded from the server</span>
- **Proxy templates:** Choosing a Proxy Template <span class="optional">NGINX. The list of templates is loaded from the server  
    </span>
- <span class="optional">**Dns templates:** Choosing a DNS Template BIND9. The list of templates is loaded from the server  
    </span>
- <span class="optional">**Client configuration:** The permissions that will be active in the client area and more  
    </span>
    - <span class="optional">**Button Filemanager:** Show/hide file manager button in client area  
        </span>
    - <span class="optional">**Button phpPgAdmin:** Show/hide phpPgAdmin button in client area</span>
    - <span class="optional">**Button phpMyAdmin:** Show/hide phpMyAdmin button in client area  
        </span>
    - <span class="optional">**Button Go to HestiaCP:** Show/hide "Go to HestiaCP" button in client area  
        </span>
    - **<span class="optional">Opening the file manager in a new tab: </span>**<span class="optional">If this is enabled, the file manager will open in a new window</span>
    - <span class="optional">**Show password for server:** If this is enabled, the user will see information about his password</span>
    - <span class="optional">**Used space limit notification:** Setting the limit, when exceeded, a notification will be sent to the user that the place is running out. The value can be entered from 10 to 99. When 0 do not send notification to users. Default is 99  
        </span>
    - <span class="optional">**Print module logs:** Enable or disable printing of module logs  
        </span>
    - <span class="optional">**Print activity logs**: Enable or disable printing activity logs of module</span>
- <span class="optional">**Email configuration:** Setting up email templates. Selection of pre-prepared templates to inform the user about some actions  
    </span>
    - <span class="optional">**Reset service password email template:** When resetting the service password  
        </span>
    - <span class="optional">**FTP User is ready email template:** When a new FTP user was created  
        </span>
    - <span class="optional">**Reset FTP password email template:** When the FTP user password was changed  
        </span>
    - <span class="optional">**e-Mail Account is ready email template:** When a new mail account was created  
        </span>
    - <span class="optional">**Reset email password email template:** When the password is changed in the mail account  
        </span>
    - <span class="optional">**Database is ready email template:** When the new database is created  
        </span>
    - <span class="optional">**Reset database password/username email template:** When the database password or username has been changed  
        </span>
    - <span class="optional">**End of place email email template:** When the space in the account is already running out  
        </span>