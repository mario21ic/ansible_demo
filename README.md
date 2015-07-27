# ansible_demo
Instructions:
* Up: vagrant up
* Test connection: vagrant ssh
* Test ssh key: ssh vagrant@127.0.0.1 -p 2222 -i ~/.vagrant.d/insecure_private_key
* Ping: ansible testserver -i inventory -m ping
