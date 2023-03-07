# Product configuration in WHMCS

#####  [Order now](https://puqcloud.com/index.php?rp=/store/whmcs-module-hestiacp) | [Dowload](https://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-HestiaCP/) | [FAQ](https://faq.puqcloud.com/)

### Here is the data provided when configuring the product for the service administrator in WHMCS.

![image](https://user-images.githubusercontent.com/81689153/223441688-a30c6f64-8237-4dee-96b7-3ba79ee60697.png)

- **License key:** A pre-purchased license key for the **"PUQ HestiaCP"** module. For the module to work correctly, the key must be active
- **Chose pakage on server:** The list of packages is pulled from the server. Will be used when the **"Use the package parameters"** option is not selected. And also if for some reason it will not be possible to create a custom package.  
>**Attention!** To deploy a custom package, you must set the interface language for the account administrator to English.
- **Use the package parameters:** The option allows you to make a choice of settings. Whether you want to use the packages already configured on the server or upload a customized custom package. Use the package parameters entered below, and create the package if it does not exist on the server. And if there is a package, then change its values to those entered below. 
>The module works as follows: It can use existing packages on the server or create new packages on the server with the HestiaCP panel. If you are using existing packages on the server, disable this option. If you want the module to create packages on its own - enable this option to create a package with the parameters given below.
- **Filemanager settings:** File manager settings  
    
    - **Hostname:** The hostname of the file manager
- **Pakage configuration:** Setting up a custom package  
    
    - **Name pakage:** The package name entered will be used to configure the custom package if the option is selected **"Use the package parameters"**
    - **Custom username:** A new name will be generated each time the create account function is called.
The custom name will be generated as follows, where PREFIX_ will only be present if the field is set: *PREFIX_[*random_x4*]_[*user_id*]_[*service_id*]*
    - **Prefix username:** This is prefix of your users. May remain empty. This will work when the Custom username option is enabled, also when the user has not ordered a domain and the username field is left blank, the username is invalid
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
- **Web templates:** Choosing a template Web Template APACHE2. The list of templates is loaded from the server
- **Web templates backend:** Choosing a Backend Template PHP-FPM. The list of templates is loaded from the server
- **Proxy templates:** Choosing a Proxy Template NGINX. The list of templates is loaded from the server  
    
- **Dns templates:** Choosing a DNS Template BIND9. The list of templates is loaded from the server  
    
- **Client configuration:** The permissions that will be active in the client area and more  
    
    - **Button Filemanager:** Show/hide file manager button in client area  
    - **Button phpPgAdmin:** Show/hide phpPgAdmin button in client area
    - **Button phpMyAdmin:** Show/hide phpMyAdmin button in client area  
    - **Button & link Go to HestiaCP:** Show/hide "Go to HestiaCP" button and full link in client area  
    - **Opening the file manager in a new tab:** If this is enabled, the file manager will open in a new window
    - **Show username & password for server:** If this is enabled, the user will see information about his password and username
    - **Used space limit notification:** Setting the limit, when exceeded, a notification will be sent to the user that the place is running out. The value can be entered from 10 to 99. When 0 do not send notification to users. Default is 99  
    - **Print module logs:** Enable or disable printing of module logs  
    - **Print activity logs**: Enable or disable printing activity logs of module
- **Email configuration:** Setting up email templates. Selection of pre-prepared templates to inform the user about some actions  
    
    - **Reset service password email template:** When resetting the service password  
    - **FTP User is ready email template:** When a new FTP user was created  
    - **Reset FTP password email template:** When the FTP user password was changed  
    - **e-Mail Account is ready email template:** When a new mail account was created  
    - **Reset email password email template:** When the password is changed in the mail account  
    - **Database is ready email template:** When the new database is created  
    - **Reset database password/username email template:** When the database password or username has been changed  
    - **End of place email email template:** When the space in the account is already running out

> ### Features of the service package deployment on the HestiaCP server
>
>If the "Use the package parameters" option is enabled The package settings in this section will be used to deploy to the server, while the "Name pakage" field will be used as the package name. If the "Use the package parameters" option is disabled, the "Chose pakage on server" field will be used as the package name.
>
>After saving the settings, the package will not be deployed. Package deployment will start when a new service user is created.
>
>It is also possible to deploy manually the package on the server. To do this, you need to enter in the admin panel and any client that has this service and call the "Change Package" module function.
>
>If for some reason it is not possible to deploy a custom package on the server, in this case, the already existing package from the server, previously selected in the "Chose package on server" option, will be used.
