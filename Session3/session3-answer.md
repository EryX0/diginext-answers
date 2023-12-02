# Session 3 Answer

## Part 1

the task brief for the first part was to:

```md
1. Create 3 VM & install Nginx on them
2. Configure all Nginx instances as equal and serve a static page on each of them
3. Specify an instance specific content on each node which enables you to see which one you’re accessing
4. Create a forth VM and install HAproxy on it
5. Configure the HAproxy to answer on a specific URL and balance the load on that Nginx instances
6. Reconfigure the HAproxy to answer on the same URL but on 3 different path which each of them will connect to each Nginx instances
7. Reconfigure the HAproxy to answer on the different URL which each of them will connect to each Nginx instances
```

I wrote a docker-compose to deploy **Nginx + Sample Webapp** on all the tree VM's that we created to make things easier.

the Nginx reverse proxies requests to our webapp which will have a unique respond in each VM/container (this was our webapp's feature)

then got ssl certificate from certbot, made cert.pem and privkey.pem into one file with something like this:

```sh
cat /path_to_cert/cert.pem | /path_to_cert/privkey.pem | /path_to_cert/combined-cert.pem
```