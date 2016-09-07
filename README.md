Shelleg Swarm demo
==================

This is the high level plan ::

So what we are going to see here is the following flow:

1. Setup 1 Virtual Instances { via Virtualbox } or 1 Instance on AWS
2. Setup 3 Virtual Instances { via Virtualbox } or 3 Instances on AWS
3. Setup all the needed packadges, services etc on each of the vms/instances
4. Configure each node individually
5. Deply a demo application on top of the Swarm Cluster

This project uses [Ansible](http://www.ansible.com) to automate the entire process.

Once we are done for a kickstart you will need to:

1. Install perquisites: Vagrnat (& Virtualbox), Ansible, Git + Optional requirements: AWS account for the aws flow.
2. Invoke Ansible for infra services such as DNS, NTP etc like so: `ansible-playbook playbooks/deploy-infra.yml` - if you stop here you should have a clean vm named **shelleg-infra01** with a Docker daemon you can play arround with Docker ...
3. Invoke Ansible for swarm cluster like so: `ansible-playbook playbooks/deploy-swarm-cluster.yml` [ still WIP ]
4. Deploy your application by running: `ansible-playbook playbooks/deploy-app.yml` [ still WIP ]
5. Test the app lets run zulip via compose -> https://github.com/galexrt/docker-zulip/blob/master/docker-compose.yml 

To definitely be continued ... 