What is this?
-------------

Basic
=====

A few template examples for learning servers, volumes and public IPs

PerfTesting
===========

Templates and environment files I used to setup some OpenStack performance
testing. These templates will configure x number of instances with 2 volumes
(root and test) and drop some config files on each machine.  The cloud-init
file will then fill the volume under test (/dev/vdb) with random data. The
stack will complete when all instances have filled their volumes, Then assign
a public IP to one node which you should use to run tests. This all assumes a
couple things are installed in your image like vdbench and a script to find
the load generators (all on local private network).
