# Product configuration in WHMCS

#####  [Order now](https://panel.puqcloud.com/index.php?rp=/store/whmcs-module-hestiacp) | [Dowload](https://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-HestiaCP/) | [FAQ](https://faq.puqcloud.com/)

##### Here is the data provided when configuring the product for the service administrator in WHMCS.

[![image-1672999068611.png](https://doc.puq.info/uploads/images/gallery/2023-01/scaled-1680-/image-1672999068611.png)](https://doc.puq.info/uploads/images/gallery/2023-01/image-1672999068611.png)

- **License key:** A pre-purchased license key for the **"PUQ HestiaCP"** module. For the module to work correctly, the key must be active
- **Chose pakage on server:** The list of packages is pulled from the server. Will be used when the **"Use the package parameters"** option is not selected. And also if for some reason it will not be possible to create a custom package.  
    <p class="callout warning">**Attention!** To deploy a custom package, you must set the interface language for the account administrator to English.</p>
- **Use the package parameters:** The option allows you to make a choice of settings. Whether you want to use the packages already configured on the server or upload a customized custom package. Use the package parameters entered below, and create the package if it does not exist on the server. And if there is a package, then change its values to those entered below. <p class="callout info">The module works as follows: It can use existing packages on the server or create new packages on the server with the HestiaCP panel. If you are using existing packages on the server, disable this option. If you want the module to create packages on its own - enable this option to create a package with the parameters given below.</p>
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
    - <span class="optional">**End of place email email template:** When the space in the account is already running out</span>

#### <span style="color: #993300;">**<span class="optional">Features of the service package deployment on the HestiaCP server</span>**</span>

<span style="color: #993300;">**<span class="optional">If the "Use the package parameters" option is enabled The package settings in this section will be used to deploy to the server, while the "Name pakage" field will be used as the package name. If the "Use the package parameters" option is disabled, the "Chose pakage on server" field will be used as the package name.</span>**</span>

<span style="color: #993300;">**<span class="optional">After saving the settings, the package will not be deployed. Package deployment will start when a new service user is created.</span>**</span>

<span style="color: #993300;">**<span class="optional">It is also possible to deploy manually the package on the server. To do this, you need to enter in the admin panel and any client that has this service and call the "Change Package" module function.</span>**</span>

<span style="color: #993300;">**<span class="optional">If for some reason it is not possible to deploy a custom package on the server, in this case, the already existing package from the server, previously selected in the "Chose package on server" option, will be used.</span>**</span>