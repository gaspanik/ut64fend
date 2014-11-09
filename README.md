# UT64-fend

[protean/UT64-fend](https://vagrantcloud.com/protean/boxes/UT64-fend) is a standard Ubuntu 14.04 box with LAMP/MxxN stack and some helpful programs for front-end developers.

---

## Changelog

Update Vagrantfile.

* Fixed synced_folder permission issue. :smiley:

## Changelog(Box)

Ver. 0.2.0: Add ngrok and JSON Server.

If you already installed this box, run `vagrant box outdated`.

```
$ vagrant box outdated
```

> Checking if box 'protean/UT64-fend' is up to date...  
> A newer version of the box 'protean/UT64-fend' is available! You currently have version '0.1.0'. The latest is version '0.2.0'. Run `vagrant box update` to update.

---

## Usage

1. Clone this repository
2. Vagrant up
3. Vagrant ssh or Open [http://192.168.33.100](http://192.168.33.100) ([http://localhost:8080](http://localhost:8080))

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
* MySQL login: root/root
* PHP info: [http://192.168.33.100/info.php](http://192.168.33.100/info.php)

Connect to MySQL and MongoDB w/ SSH（Host: 192.168.33.100, id: vagrant, password: vagrant）.
