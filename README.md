# auto-alpaca

./install.sh

then add in a cron ./update.sh

Auto-update numerous-alpaca without githook

Cron example:

```
SHELL=/bin/bash
PATH=/usr/local/sbin:/usr/local/bin:/sbin:/bin:/usr/sbin:/usr/bin

* * * * * /home/numerous-alpaca/auto-alpaca/update.sh >> /home/numerous-alpaca/auto-alpaca/update.log  2>&1
```