Step 1 - establish infrastructure
=================================

Choose your poizen:
-------------------
vbx - short for Virtualbox ;)

aws


What we need ?
--------------

1-2 base machines which provide:
--------------------------------

- Network time
- Domain Name Resolution
- Service Discovery service - for our Swarm cluster to connect to

3 or more swrm nodes
--------------------

- Register against consul cluster
- Resolve against DNS services
- Resolce service anemes via DNS interface

