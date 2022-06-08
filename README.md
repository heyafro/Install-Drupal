# Install Drupal 9 on Ubuntu Server 20.04

This is a simple automated BASH script to install Drupal 9 on Ubuntu 20.04.  This could work on other Ubuntu/Debian versions, but it has not been tested.

Before running this script, some changes to variables will be needed at the top:
```
domain=your.domain.com
```

Make sure that the domain name of the Drupal Site is filled out correctly in `domain`.  The full url isn't needed and neither is `www` part.  That part is assumed and will be filled in later on different configuration files.

After the script has been modified, make the script executable by running `chmod +x install-drupal.sh` and run it as below:
```
sudo ./install-drupal.sh
```

When the script completed its run, there will be out put for each step of the process that looks like:
```
Installing LAMP Server

Installing software requirements via APT...

Configuring firewall..

Creating configuration files for Apache Webserver...

Finalizing changes to Apache Webserver...

Going through MySQL secure setup...

Installing Drupal 9...
YOUR MYSQL PASSWORD IS: <SOME RANDOM LETTERS AND NUMBERS>
YOUR DRUPAL MYSQL PASSWORD IS: <SOME RANDOM LETTERS AND NUMBERS>
```
Make sure to record these passwords at the end of the script and **DO NOT LOSE THEM**.  They are needed for root access to MySQL and Drupal's access the MySQL.  The Drupal MySQL Password is need in the next steps for installation.

