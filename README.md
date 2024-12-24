# NGINX Config

## Steps to follow
* Config Location
  ```
  /etc/nginx/sites-available
  ```
* Make a backup of the current file and add date to it, so that you'll know which file to revert to.
  ```
cp default default-2024-12-24
  ```
* Edit the `default` file
```
vi default
```
* Test if config has no errors
```
nginx -t
```
`successful results`
```
nginx: the configuration file /etc/nginx/nginx.conf syntax is ok
nginx: configuration file /etc/nginx/nginx.conf test is successful
```
`unsuccessful results`
```
nginx: [emerg] duplicate location "/itac-api/" in /etc/nginx/sites-enabled/default:108
nginx: configuration file /etc/nginx/nginx.conf test failed
```
