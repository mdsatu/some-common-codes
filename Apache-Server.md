## Apache basic commands

```bash
ssh username@ip_or_host_name

# Check conf file configuration
sudo apachectl configtest

# Restart alache2 with all conf file
sudo service apache2 restart
```

## Nuxtjs Conf File Example

```bash
<VirtualHost *:80>
  ServerName upojukto.com
  ServerAlias www.upojukto.com

  ProxyRequests Off
  ProxyPreserveHost On

  <Proxy *>
      Order deny,allow
      Allow from all
  </Proxy>

  ProxyPass / http://localhost:3004/
  ProxyPassReverse / http://localhost:3004/
</VirtualHost>
```
