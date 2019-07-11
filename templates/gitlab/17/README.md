# GitLab CE

GitLab CE is a free alternative to GitHub

Stack based on official GitLab version: latest

https://hub.docker.com/r/gitlab/gitlab-ce/


## config

### Supporting proxied SSL
    
https://gitlab.com/gitlab-org/omnibus-gitlab/blob/master/doc/settings/nginx.md

use Rancher LB 443 -> 80

edit `/gitlab/etc/gitlab# vi gitlab.rb`
```
nginx['listen_port'] = 80
nginx['listen_https'] = false
nginx['proxy_set_headers'] = {
  "X-Forwarded-Proto" => "https",
  "X-Forwarded-Ssl" => "on"
}
``` 