# js-skeleton-webapp01

A simple skeleton for a website using `JS`

## Deployment

```
git clone https://github.com/freddieventura/js-skeleton-webapp01 <your-newrepo>
npm install
npm run build
```

If you want to visualize it in your `apache2` webserver you can do a symlink

```
sudo ln -s /home/user/new/repo/path/ /var/www/html/
```

Now you can simply access your webbrowser

```
http://localhost:port/reponame/public/index.html
```

**Extra!!**

Would you be deploying this in a server and need to access it but have the webserver port firewalled, you can throw a ssh tunnel from it

```
ssh -TN -p <serverSSHport> -L <tunnelPort>:127.0.0.1:<apache2Port> user@serverIp
```
Note !! : TunnelPort has to be above 1024 if you are not superuser


With this extra you can now access to this webApp remotely in whatever host you are connected from just open the local webbrowser

```
http://localhost:<tunnelPort>/reponame/public/index.html
```
