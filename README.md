# ansible_demo
Instructions:
* Change branch: git checkout test1
* Up: vagrant up
* Test connection: vagrant ssh
* Test ssh key: ssh vagrant@127.0.0.1 -p 2222 -i ~/.vagrant.d/insecure_private_key
* Ping: ansible testserver -i inventory -m ping
* Change branch: git checkout test2
* Testing commands:
 * ansible testserver -m ping
 * ansible testserver -m command -a uptime
 * ansible testserver -a uptime
 * ansible testserver -a "tail /var/log/dmesg"
 * ansible testserver -s -a "tail /var/log/syslog"
* Playing with nginx:
 * ansible testserver -s -m apt -a name=nginx
 * ansible testserver -s -m apt -a update_cache=yes
 * ansible testserver -s -m service -a "name=nginx state=restarted"
 * vagrant reload
 * Test browser: http://localhost:8080/
