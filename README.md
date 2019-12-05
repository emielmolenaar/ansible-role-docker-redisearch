Redisearch in docker role for Ansible
=================

A simple role for deploying and configuring [Redisearch](https://oss.redislabs.com/redisearch/index.html) on your hosts using [Ansible](http://www.ansibleworks.com/).

Usage
-----

Clone this repo into your roles directory:

    $ git clone https://github.com/emielmolenaar/ansible-role-docker-redisearch.git roles/docker-redisearch

And add it to your play's roles:

    - hosts: ...
      roles:
        - docker-redisearch
        - ...

I recommend using a `requirements.yml` in your roles directory though:
   
    - src: https://github.com/emielmolenaar/ansible-role-docker-redisearch.git 
      name: docker-redisearch

Installing the role will require a `ansible-galaxy install -r ./roles/requirements.yml -p ./roles` from the root directory of your playbook. 
