# UT64-fend

[protean/UT64-fend](https://vagrantcloud.com/protean/boxes/UT64-fend) is a standard Ubuntu 14.04 box with LAMP(WP-CLI ready), NodeJS, MongoDB, Redis, Ruby(rbenv), Git and some helpful programs for front-end developers.

---

## Changelog

Update Vagrantfile.

* Fixed synced_folder permission issue. :smiley:

## Changelog(Box)

* Ver. 1.0.0: Box size optimized.
* Ver. 0.4.0: Remove Laravel Installer. Add jspm(0.8.4) and fixed ngrok web interface loopback address issue.
* Ver. 0.3.1: Add Composer (WP-CLI ready) and some npm modules. Modify apache2 `/var/www` AllowOverride option.  
* Ver. 0.2.0: Add ngrok and JSON Server.

If you already installed this box, run `vagrant box outdated`.

```
$ vagrant box outdated
```

> Checking if box 'protean/UT64-fend' is up to date...  
> A newer version of the box 'protean/UT64-fend' is available! You currently have version '0.3.2'. The latest is version '0.4.0'. Run `vagrant box update` to update.

```
$ vagrant box update
```

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

### composer

```
$ composer selfupdate
```

### WP-CLI (via Composer)

```
$ cd ~/.composer
$ composer update
```

## Box info.

* Box root passwd: vagrant
* MySQL login: root/root
* PHP info: [http://192.168.33.100/info.php](http://192.168.33.100/info.php)

Connect to MySQL and MongoDB w/ SSH（Host: 192.168.33.100, id: vagrant, password: vagrant）.
