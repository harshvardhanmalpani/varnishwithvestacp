# varnishwithvestacp
## NO WARRANTY OR ANYTHING LIKE THAT, USE AT YOUR OWN RISK
Vesta CP config with Nginx + PHP FPM with Varnish proxy for Wordpress

Thanks to @fevangelou for varnish vcl file

## VestaCP config
curl -O http://vestacp.com/pub/vst-install.sh

./vst-install.sh --nginx yes --phpfpm yes --apache no --named no --remi yes --vsftpd no --proftpd yes --iptables no --fail2ban no --quota no --exim yes --dovecot yes --spamassassin no --clamav no --softaculous no --mysql no --postgresql no

### Port for Nginx
- Listening at 443
- Fetching from 8443

### Port for Varnish
- Listening at 8443
- Fetching from 8445

### Port for Apache
- Listening at 8445
- Fetching from home dir of virtual node