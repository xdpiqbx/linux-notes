# linux-notes

```code
sudo apt-get update
sudo apt-get upgrade

sudo apt install ssh

cat /etc/passwd --- про користувачів

echo 'AllowUsers root' >> /etc/ssh/sshd_config --- Додав строку в кінці файлу

chown -R root:administrators ./ssh
id -Gn или groups

groupadd ssh-users
usermod -a -G ssh-users root
usermod -a -G ssh-users max

chown -R :ssh-users /etc/ssh

chmod -R g+rwx /etc/ssh
```