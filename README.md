capbash-phpapp
==============

Scripts for deploying a PHP application from a git repository

# How to Install #

Install capbash first, more details at:
https://github.com/aforward/capbash

```
git clone https://github.com/aforward/capbash YOUR_REPO_ROOT
cd YOUR_REPO_ROOT
./bootstrap
```

Now you can install phpapp into your project

```
./capbash install phpapp
```

# Configurations #

The available configurations include:

```
GIT_URL=${GIT_URL-git@github.com:aforward/samplephp.git}
PHPAPP_NAME=${PHPAPP_NAME-samplephp}
PHPAPP_SERVER_NAME=${PHPAPP_SERVER_NAME-samplephp.vm}
PHPAPP_PUBLIC_PATH=${PHPAPP_PUBLIC_PATH-/public}
```

# Deploy to Remote Server #

To push the phpapp script to your server, all you need if the IP or hostname of your server (e.g. 192.167.0.48) and your root password.

```
./capbash deploy <IP> phpapp
```

For example,

```
./capbash deploy 127.0.0.1 phpapp
```
