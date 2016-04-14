auto-alpaca
===========

> Note: It is recommended that you create a new user as numerous-alpaca is heavily in development and may have security exploits that allow an attacker access to your system

Auto-update numerous-alpaca without a githook!

Simply `./install.sh`, then add `update.sh` to cron. Here's an example:

```sh
$ ./install.sh
$ crontab -e
```
An example cronjob to use is (make sure to replace the path to the path of your script):
```sh
* * * * * /home/numerous-alpaca/auto-alpaca/update.sh >> /home/numerous-alpaca/auto-alpaca/update.log  2>&1
```
