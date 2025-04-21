# FTPS_homelab_IIS_port-forwarded
### Personal documentation: My HomeLab FTPS setup/configuration using the Windows IIS feature, with port forwarding

### IP Bindings

* Its important to turn the private ip into static

![Ip Bindings](img/IpBindings.png)

---

### Passive port range

* This will be in passive mode so configuring port range is necessary.

![Passive ports](img/FTP-firewall-passive-ports.png)

---

### Windows Firewall

* Configure port range in Windows Firewall as well for port forwarding.

![Windows Firewall](img/WindowsFirewall.png)

---

### Port Forwarding Configuration

* Using port 21 for control port and the port range for data channel.

![Port Forwarding](img/Port-Forwarding.png)

---

### FTP Authentication

* Disabling Anonymous login for security purpose.

![Authentication](img/Authentication.png)

---

### FTP Authorization Rule

* Adding the created users to allow read and write permission.

![Authorization Rules](img/Authorization-Rules.png)

---

### FTP User Isolation

* Isolating users in their respective root directories.

![User Isolation](img/UserIsolation.png)

---

### SSL

* Adding a self-signed SSL certificate for data encryption.

![SSL](img/SSL-setting.png)

---

### FTP Logs Configuration

![FTP Logging](img/Logging.png)

---

### FTP root folder structure

* Created a virtual directory for admin and points it to the root directory to grant access to all sub directory.

![Folder-Structure](img/FolderStructure.png)

---

### NTFS Permission Configuration

* Adding an extra layer of security 

![NTFS-Config](img/NTFS-Security.png)
