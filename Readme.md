<p align="center"><img alt="Ihlecloud" src="https://me.ihlecloud.de/img/logo.png" height="76"></p></img>
<h1 align="center">Icinga2 Scripts</h1>
<h3 align="center">check_postfwd_rate</h3>

<br>
<h3 align="center">
    <a href="https://github.com/n1tr0-5urf3r/check_postfwd_rate/releases/">Download Latest
    </a>・
    <a href="https://exchange.icinga.com/n1tr0-5urf3r">Other Projects</a>・<a href="https://www.paypal.com/donate/?hosted_button_id=KXMYX49C6MLLN">Donate</a></h3>

---

## check_postfwd_rate
This plugin checks for senders that exceeded a sending limit. A valid postfwd installation and configuration is required. The configured rate limits are automatically checked against.

### Installation
To avoid permission issues when running this check via nrpe
configure a cronjob like following to periodically cache data:

```sh
*/3 * * * * /usr/sbin/postfwd --dumpcache > /var/opt/postfwd_dumpcache.txt
```

### Usage    
Simply invoke with `./check_postfwd_rate`

---

## Donation
If you like my work a donation is very welcome :) 

[![](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/donate/?hosted_button_id=KXMYX49C6MLLN)