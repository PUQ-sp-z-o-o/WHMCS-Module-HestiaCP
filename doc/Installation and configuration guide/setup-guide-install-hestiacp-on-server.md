# Setup guide: Install HestiaCP on server

### ![Logo.png](https://doc.puq.info/uploads/images/gallery/2022-10/scaled-1680-/logo.png)Hestia Control Panel

##### **Step 1: Make sure that your server is running a supported operating system (amd64 or arm64):**

- Debian 10
- Debian 11
- Ubuntu 18.04 LTS
- Ubuntu 20.04 LTS
- Ubuntu 22.04 LTS

##### **Step 2: Log in as the system user (root):**

You'll need to connect to your server as **root**, either directly from the console or remotely using SSH.

##### **Step 3: Download the installer:**

`wget https://raw.githubusercontent.com/hestiacp/hestiacp/release/install/hst-install.sh`

##### **Step 4: Run the installer and follow the prompts:**

`bash hst-install.sh`

##### **To perform an unattended installation (with defaults):**

`bash hst-install.sh --interactive no --email <em>email@domain.tld</em> --password <em>p4ssw0rd</em> --hostname <em>hostname.domain.tld</em> -f `

##### **Or modify your installation with for exmaple:**

`bash hst-install.sh --apache no --postgresql yes --clamav no --spamassassin no `

Will install Hestia without Apache2, ClamAV and Spamassassin How ever it will install Postgresql as additional feature

More options or examples can be found in the [Documentation](https://docs.hestiacp.com/getting_started.html#all-available-options-of-install-script) or use the [Install string generator](https://gabizz.github.io/hestiacp-scriptline-generator/)

##### **Reporting bugs and issues:**

If something isn't working as expected on HestiaCP, please report the issue to our development team on [GitHub](https://github.com/hestiacp/hestiacp/issues).  
  
**Please include:**

- Hestia Control Panel version/release
- Operating system distribution and release/version
- Options specified during installation (if applicable)
- A detailed description of the issue, with any relevant logs or files as well.

**License**

Hestia Control Panel is open-source and licensed under GPLv3.