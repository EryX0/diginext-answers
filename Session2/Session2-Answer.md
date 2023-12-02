# Session 2 Answer

the task brief was to:

```md
1. Lunch a blog via wordpress using docker-compose
2. Persist your data, so you don't lose them in case of container restart
```

but I took it a step further with adding **Nginx** to this task, and using it as a webserver to do a **reverse proxy** to our wordpress blog.

also added tls (certs) to nginx reverse proxy and also redirection to 443 port and tls connection from port 80.

no further explaination is needed, docker-compose.yaml and default.conf (nginx config) is in the current folder you're reading this file from.
