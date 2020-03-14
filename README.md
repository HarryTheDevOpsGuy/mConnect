#### Welcome  [ mConnect - a Powerful SSH Session Manager ]

**mConnect** : v0.0.2

##### Getting Start

###### What is mConnect?
**mConnect** is small utility to manage ssh connection credentials. and allow you to connect any server smartly with mConnect.

#### How To install ?
Just download this repository and follow below steps.

```bash
sudo git clone https://github.com/HarryTheDevOpsGuy/mConnect.git /opt/mconnect
sudo chown -R ${USER}:${USER} /opt/mconnect
sudo chmod a+x /opt/mconnect/mConnect
sudo ln -s /opt/mconnect/mConnect /usr/local/bin/mconnect
mconnect -v
```

if you got mConnect version after executing `mconnect -v` command. it means you have install this perfectly.

#### How to add host in mConnect manager?
There is `inventory/hosts` or `~/inventory/hosts` file in project repository. you need to add your host related details in `inventory/hosts` file.

```bash
#vim /opt/mconnect/inventory/hosts



```




---
Thanks
Hari
