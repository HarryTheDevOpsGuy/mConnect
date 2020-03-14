#### Welcome  [ mConnect - a Powerful SSH Session Manager ]

**mConnect** : v0.0.6

##### Getting Start

###### What is mConnect?
**mConnect** is small utility to manage ssh connection credentials. and allow you to connect any server smartly with mConnect.

#### How To install ?
Just download this repository and follow below steps.

```bash
sudo apt-get install -y sshpass
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
## This is Variable file you can update this file accordingly.
MAIL_TO="HarryTheDevOpsGuy@gmail.com"
declare -A HOSTS=(
  # Development Env
  ["ABC-DEV"]="ubuntu@172.31.1.12:secret_pass"
  ["ABC-QA"]="ubuntu@172.31.2.99:keyname.pem"
  ["ABC-Stage-New"]="harry@172.1.19.4:private_key"
  # You can add comments like below
  # ["ABC-TEST"]="ubuntu@172.31.22.12:ur_pass_here"
)
```

#### Where do i store ssh private_keys or pem keys?
All Private keys should be stored in `~/inventory/keys` directory. and key name should be updated in `~/inventory/hosts` (without key path) file accordingly.


---
Thanks
Hari </br>
Profile : [Hire me - harrythedevopsguy.github.io  ][677a6d8b]

  [677a6d8b]: https://harrythedevopsguy.github.io/ "Visit my profile page."
