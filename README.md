# Home_server

Configuration for home server. 
Based on Proxmox with containerization of various services.

## Manual Steps
To enable Nextcloud sync client to connect to the server, you have to adjust `config.php` in the Nextcloud configuration. 
(e.g. ./www/nextcloud/config/config.php)
```
  'overwrite.cli.url' => 'http://cloud.rhombo.xyz',
  'overwriteprotocol' => 'https',
```
See https://github.com/nextcloud/desktop/issues/3707 


## Links
Traefik
* https://gist.github.com/alexzorin/f856d54d228ca4ca1abdca41c7d89f72
* https://major.io/2021/08/16/wildcard-letsencrypt-certificates-traefik-cloudflare/
* https://greenfrognest.com/LMDSTraefikProxy.php