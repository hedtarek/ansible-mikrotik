cmd1: ansible all -i inventory/hosts.yml -m apt -a "name=nginx state=present" -b  
cmd2:ansible all -m apt -a "name=nginx state=present" -b

"changed": true ---  >Cela signifie qu’Ansible a fait un changement : ici, il a installé Nginx.
systemctl status nginx

