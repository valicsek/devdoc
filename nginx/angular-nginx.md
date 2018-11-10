# Angular application using Nginx

First, enable the port in Linux:

```
ufw allow :port_number
```

then run your angular on a specific IP

```
ng serve --host :ip_of_your_server
```

_Note: If you run on localhost, no one will able to reach your application from outside_

After you finished your app, you should close your port

```
ufw deny :port_number
```

## Errors

### Invalid Host header

I got this error when I just started my app using `ng serve` command.

> **Error: Invalid Host header**
>
> use the **--disable-host-check** flag
>
> ```
> ng serve --open --host $IP --port $PORT --disable-host-check
> ```



## Get your Angular Project to your server

Clone your repo

```
git clone: your_repo
```

Get the newest branches

```
git branch -r :your_branch_name
```