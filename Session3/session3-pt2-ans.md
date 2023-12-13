# Session 3 Answer - Part 2

## SQL Master/Slave replication

the task brief for the second part of session3 was to:

```md
1. Setup a single MySQL/MariaDB node without any configurations (default configuration). Secure it so you could only be able to connect to it by authentication (root user MUST only be able to connect to it from localhost). Create some databases and within these databases, create some tables and then insert some data in these tables (Play with it).

2. Now lets create a slave node. you need to set some configuration for your master (read where you can put your configurations and what is the best way to do so to make it easy to eyes for read).

3. In which way you desire, corrupt your master node and then change your slave to be act as new master node and then recover your old master node and set it up to be your new slave (switch master & slave roles between your 2 nodes).

4. Now let's use what we did in last task and create a slave for our wordpress service and do as described in section 3 of this task, on this service.
```
