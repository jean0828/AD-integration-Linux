# AD-integration-Linux
This is a tutorial to integrate a linux server in an Active Directory environment.

For this tutorial we have the following devices:
* Active Directory Server: IP 10.0.0.4
* Linux Server: IP 10.0.0.5

## Instalation of Active Directory
1. we need a Windows server and adding the role of Active Directory.

![AD server installation](https://github.com/jean0828/AD-integration-Linux/blob/main/ADtutorial/ADserver1.jpg)
![AD server installation part 2](https://github.com/jean0828/AD-integration-Linux/blob/main/ADtutorial/ADserver2.png)
![AD server installation part 3](https://github.com/jean0828/AD-integration-Linux/blob/main/ADtutorial/ADserver3.png)
![AD server installation part 4](https://github.com/jean0828/AD-integration-Linux/blob/main/ADtutorial/ADserver4.png)
![AD server installation part 5](https://github.com/jean0828/AD-integration-Linux/blob/main/ADtutorial/ADserver5.png)

2. Configure the domain

In this case the domain name is: *lab.local*

![AD server configuration](https://github.com/jean0828/AD-integration-Linux/blob/main/ADtutorial/adconfiguration.png)
![AD server configuration part 2](https://github.com/jean0828/AD-integration-Linux/blob/main/ADtutorial/adconfiguration2.png)
![AD server configuration part 3](https://github.com/jean0828/AD-integration-Linux/blob/main/ADtutorial/adconfiguration3.png)

then next > install. Afterward, the server will reboot.


![AD server configuration part 4](https://github.com/jean0828/AD-integration-Linux/blob/main/ADtutorial/adconfiguration4.png)

## Check Connectivity

3. Ensure the Linux server (in this case Centos7) responds to the domain.

![Linux connectivity](https://github.com/jean0828/AD-integration-Linux/blob/main/ADtutorial/linuxserver.png)
![Linux connectivity part 2](https://github.com/jean0828/AD-integration-Linux/blob/main/ADtutorial/linuxserver2.png)

## Install requirements in Linux

4. Install the following requirements in order to ensure a proper integration.

```yum install sssd realmd oddjob oddjob-mkhomedir adcli samba-common samba-common-tools krb5-workstation openldap-clients policycoreutils-python
 ```
 ![requirements](https://github.com/jean0828/AD-integration-Linux/blob/main/ADtutorial/requirements.png)
 
 ## Join the server to the Active Directory
