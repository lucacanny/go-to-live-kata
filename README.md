Lamp Stack
==========

This project build a simple server based on Ubuntu 14.04 using Vagrant and Virtualbox

Requirements
============

-   Vagrant 2.0.2
-   Virtualbox 5.2.8r121009
-   Ansible 2.4.3.0

HowTo start
===========


``` {.bash org-language="sh"}
$ git clone https://github.com/lucacanny/go-to-live-kata.git
$ cd go-to-live-kata
```

The configuration can be customized using the config file.

Create the virtual machine:

``` {.bash org-language="sh"}
$ vagrant up
```

Once the process is finished you can connect to the wordpress site from the following url:

[WordPress](http://192.168.33.20/wordpress) - 
For convenience it has been configured with static ip

**Optional:** you can add the next rule to your host file and go to http://mywordpress.local

``` {.bash org-language="sh"}
192.168.33.20     mywordpress.local
```

use this command line to add the rule:

``` {.bash org-language="sh"}
$ echo "\n192.168.33.20     mywordpress.local" | sudo tee -a /etc/hosts
```