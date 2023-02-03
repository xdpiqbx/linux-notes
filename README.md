# linux-notes

```code
su -c 'apt-get install sudo' - устанавливаю SUDO
su -c 'gpasswd -a username sudo' - добавляю пользователя в группу SUDO (перезагрузить)

sudo apt-get update - Обновление индекса пакетов
sudo apt-get upgrade - Обновление пакетов
sudo apt-get install build-essential dkms

sudo mount -o remount,exec,ro /media/cdrom0 - перемонтировал CD ROM чтоб можно было с него запустить файлик
sudo /media/cdrom0/VBoxLinuxAdditions.run - запустил с CD ROM нужный файлик

Установка - Python
sudo apt-get install gcc
sudo apt-get install zlib1g-dev
Качаю PythonX.X.X.tar.xz
tar -xf Python-X.X.X.tar.xz - Разархивировал в ту же папку
сd Python-X.X.X/ - перешел в разархивированую папку
 ./configure
 ./configure --enable-optimizations
 sudo apt-get install make
 sudo make
 sudo make install


sudo  apt install ssh

cat /etc/passwd

Додав строку в кінці файлу
echo 'AllowUsers root' >> /etc/ssh/sshd_config

chown -R root:administrators ./ssh
id -Gn или groups

groupadd ssh-users
usermod -a -G ssh-users root
usermod -a -G ssh-users max

chown -R :ssh-users /etc/ssh

chmod -R g+rwx /etc/ssh
```