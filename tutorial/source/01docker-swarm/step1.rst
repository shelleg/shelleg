Step 1 - establish infrastructure
=================================

Choose your poizen:
-------------------
vbx - short for Virtualbox ;)

aws - Amazon Web Services


What we need ?
--------------

1 or more base machines which provide:
-------------------------------------

- Network time
- Domain Name Resolution
- Service Discovery service - for our Swarm cluster to connect to

3 or more sdocker warm nodes
----------------------------

- Register against consul cluster
- Resolve against DNS services
- Resolve service names via DNS interface

