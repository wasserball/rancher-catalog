# [Rancher](http://rancher.com/) Catalog


Add this Repo to your Catalog (`/admin/settings` --> `Add Catalog`)

![image](https://raw.githubusercontent.com/wasserball/rancher-catalog/master/img/rancher-admin.png)

...

![image](https://raw.githubusercontent.com/wasserball/rancher-catalog/master/img/rancher-catalog.png)

### After adding the repo you should see the new Catalog

![image](https://raw.githubusercontent.com/wasserball/rancher-catalog/master/img/rancher-catalog-lib.png)

# Plex
This Catalog-Item uses the docker-image from [linuxserver/docker-plex](https://github.com/linuxserver/docker-plex) witch is hostet on the docker-hub @ [linuxserver/plex](https://hub.docker.com/r/linuxserver/plex/).

## Install

click on View Details, Choose a Version, modify some settings (Name, Port) and hit Launch.

- Config Path: I created a folder in my home dir (~) with the name plex `/home/nick/plex`



 ```
 nick@ubuntu:~/plex$
 // after starting the Server, you should see the Folder "Library" (ls)
 nick@ubuntu:~/plex$ ls
	Library
 ```
- Media Path: I have mounted an NFS (Network Mount) @ /mnt:/media so i used this one

## Open Plex
Open a Web-Browser and got to `<ip of your server>:32400/web/index.html`.

```
watch :-)
```

# PlexConnect

## Install

click on View Details, Choose a Version and hit Launch.

## Config
Doku @ [wasserball/plexconnect](https://github.com/wasserball/plexconnect)







