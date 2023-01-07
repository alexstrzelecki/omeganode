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