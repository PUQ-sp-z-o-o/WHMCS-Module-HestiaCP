# WEB section

#####  [Order now](https://panel.puqcloud.com/index.php?rp=/store/whmcs-module-hestiacp) | [Dowload](https://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-HestiaCP/) | [FAQ](https://faq.puqcloud.com/)

The end client, having entered the WEB section of the client panel, has access to the following information and parameters:

- Navigation bar and status information on each card.
- Button to go to add a new domain
- Button to go to FTP user management
- Cards with information about the client's WEB domains 
    - Domain name
    - SSL certificate status[ ![image-1666617121265.png](https://doc.puq.info/uploads/images/gallery/2022-10/scaled-1680-/image-1666617121265.png)](https://doc.puq.info/uploads/images/gallery/2022-10/image-1666617121265.png)
    - Domain name status in the system HestiaCP is suspended or not suspended (Active)[ ![image-1666617136198.png](https://doc.puq.info/uploads/images/gallery/2022-10/scaled-1680-/image-1666617136198.png)](https://doc.puq.info/uploads/images/gallery/2022-10/image-1666617136198.png)
    - IP Address
    - Document root
    - Aliases
    - Backend
    - Disk Space (Size)
    - Bandwidth (Traffic)
    - Time and date the entry was created
    - Buttons for managing WEB domain 
        - Edit
        - Suspend / Unsuspend
        - Delete

[![image-1666685881939.png](https://doc.puq.info/uploads/images/gallery/2022-10/scaled-1680-/image-1666685881939.png)](https://doc.puq.info/uploads/images/gallery/2022-10/image-1666685881939.png)

#### Adding a new WEB domain

After clicking on the button in the pop-up window, you must enter the name of the domain that you want to add. DNS Zones and Mail Domain will also be created

[![image-1666617427556.png](https://doc.puq.info/uploads/images/gallery/2022-10/scaled-1680-/image-1666617427556.png)](https://doc.puq.info/uploads/images/gallery/2022-10/image-1666617427556.png)

#### WEB domain editing

After clicking on the button, the following configuration is available in the pop-up window:

- Adding a WWW Alias
- Let's Encrypt certificate generation and delete (Enable SSL / Disable SSL)  
    <p class="callout warning">Attention! Requires a properly configured DNS zone for HestiaCP to properly obtain a certificate.</p>
- Enabling and disabling redirect to HTTPS (Enable SSL Force / Disable SSL Force) <p class="callout warning">Attention! Will only work if you have an SSL certificate.</p>
- List of aliases with the ability to delete each
- Dropdown list of available backend templates on the server

![image-1666617884497.png](https://doc.puq.info/uploads/images/gallery/2022-10/scaled-1680-/image-1666617884497.png)

<p class="callout warning">Attention! Web domains are the main setting. When creating a new web domain, a DNS zone will be created as well as a Mail domain. Also, if you delete the Web domain, the DNS zone of this domain will be deleted as well as the Mail domain. It also works when Suspend / Unsuspend.</p>

#### WEB domain suspend

After clicking on the button, confirmation of the action is available in a pop-up window.

[![image-1666685593532.png](https://doc.puq.info/uploads/images/gallery/2022-10/scaled-1680-/image-1666685593532.png)](https://doc.puq.info/uploads/images/gallery/2022-10/image-1666685593532.png)

#### WEB domain unsuspend 

After clicking on the button, confirmation of the action is available in a pop-up window.

[![image-1666685632008.png](https://doc.puq.info/uploads/images/gallery/2022-10/scaled-1680-/image-1666685632008.png)](https://doc.puq.info/uploads/images/gallery/2022-10/image-1666685632008.png)

#### WEB domain delete

After clicking on the button, confirmation of the action is available in a pop-up window.

[![image-1666685943210.png](https://doc.puq.info/uploads/images/gallery/2022-10/scaled-1680-/image-1666685943210.png)](https://doc.puq.info/uploads/images/gallery/2022-10/image-1666685943210.png)