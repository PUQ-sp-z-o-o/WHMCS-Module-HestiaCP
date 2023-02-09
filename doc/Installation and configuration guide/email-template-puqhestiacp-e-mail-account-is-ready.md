# Email Template (puqHestiaCP e-Mail Account is ready)

#####  [Order now](https://panel.puqcloud.com/index.php?rp=/store/whmcs-module-hestiacp) | [Dowload](https://download.puqcloud.com/WHMCS/servers/PUQ_WHMCS-HestiaCP/) | [FAQ](https://faq.puqcloud.com/)

##### Create an email template for customer notifications.

```
System Settings->Email Templates->Create New Email Template
```

- **Email Type:** Product/service
- **Unique Name:** puqHestiaCP e-Mail Account is ready

[![image-1666612442813.png](https://doc.puq.info/uploads/images/gallery/2022-10/scaled-1680-/image-1666612442813.png)](https://doc.puq.info/uploads/images/gallery/2022-10/image-1666612442813.png)**Subject:**

```
e-Mail Account {$email} is ready
```

**Body:**

```
Dear {$client_name},


You have created a new e-Mail account on Product/Service: {$service_product_name}. 
Below is the user logging data.

Hostname: {$hostname}
Email: {$email}
Password: {$password}
Webmail: http://webmail.{$hostname}
Hostname: mail.{$hostname}


IMAP SETTINGS
Authentication: Normal Password
SSL/TLS: Port 993
STARTTLS: Port 143
No encryption: Port 143

POP3 SETTINGS
Authentication: Normal Password
SSL/TLS: Port 995
STARTTLS: Port 110
No encryption: Port 110

SMTP SETTINGS
Authentication: Normal Password
SSL/TLS: Port 465
STARTTLS: Port 587
No encryption: Port 25


{$signature}
```

[![image-1666612546508.png](https://doc.puq.info/uploads/images/gallery/2022-10/scaled-1680-/image-1666612546508.png)](https://doc.puq.info/uploads/images/gallery/2022-10/image-1666612546508.png)