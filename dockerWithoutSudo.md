$ sudo groupadd docker
$ sudo gpasswd -a $USER docker
$ sudo usermod -aG docker $USER
$ sudo service docker restart
