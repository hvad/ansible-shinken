# ansible-shinken

##Shinken version 2.4.x Infrastructure deployment

- Requires Ansible 2.2 or newer
- Expects CentOS/RHEL 7.x hosts

These playbooks were tested on CentOS 7.x so we recommend
that you use CentOS or RHEL to test these modules.

These playbooks can deploy a simple all-in-one Shinken server or a distributed 
infrastructure. The inventory file 'hosts' defines the nodes in which the 
stacks should be configured.

        [arbiter]
        arbiter

        [broker]
        broker

        [reactionner]
        reactionner

        [poller]
        poller
        
        [scheduler]
        scheduler

The stack can be deployed using the following command:

        ansible-playbook -i hosts site.yml

