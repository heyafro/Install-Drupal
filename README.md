# Install Drupal 9 on Ubuntu Server 20.04

This is a simple automated BASH script to install Drupal 9 on Ubuntu 20.04.  This could work on other Ubuntu/Debian versions, but it has not been tested.

Before running this script, you will need to make some changes to variables at the top:
```
domain=your.domain.com
```

Make sure that the domain name of the Drupal Site is filled out correctly in `domain`.  The full url isn't needed and neither is `www` part.  That part is assumed and will be filled in later on different configuration files.
