swarm-demo
==========

This is the high level plan ::

So what we are going to see here is the following flow:

1. Setup 3 Virtual Mavhines { via Virtualbox } or 3 Instances on AWS
2. Setup all the needed packadges, services etc on each of the vms/instances
3. Configure each node individually
4. Deply a demo application on top of the Swarm Cluster

This project uses [Ansible](http://www.ansible.com) to automate the entire process.
Once we are done for a kickstart you will need to:

1. Install perquisites: Vagrnat (& Virtualbox), Ansible, Git + Optional requirements: AWS account for the aws flow.
2. Invoke ansible like so: `ansible-playbook playbooks/swarm-cluster.yml` - if you stop here you should have a clean swarm cluster
3. Deploy your application by running: `ansible-playbook playbooks/deploy-app.yml`
4. Test the app

To definitely be continued ... 