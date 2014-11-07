# UT64-fend

[protean/UT64-fend](https://vagrantcloud.com/protean/boxes/UT64-fend) is a standard Ubuntu 14.04 box with LAMP and some helpful programs for Front-End Developers.

## Usage

1. Clone this repository
2. Vagrant up

## Update softwares

### deb

```
$ sudo apt-get update
$ sudo apt-get upgrade
```

### npm

Check update with david.

```
$ sudo david -g
$ sudo npm install -g (updated-packages)
```

### gem

rbenv ready. rbenv-rehash is already installed.

```
$ gem update
```

## Box info.

* Box root passwd: vagrant
* MySQL password: root/root

Connect to MySQL and MongoDB w/ SSH（Host: 192.168.33.100, id: vagrant, password: vagrant）.