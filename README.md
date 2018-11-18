# deploy_nginx
<p>Step by step: Using Ansible to deploy Nginx virtual host into Vagrant Box </p>.
Step 1: Tạo folder để chứa Vagrant Box file
Step 2: Clone 2 Box files.
  git clone
Step 3: Add the Box into Vagrant Install
  vagrant box add Ansible-Server Ansible.box
  vagrant box add Nginx-Server Nginx.box
Step 4: Initialize New Vagrant Box
  vagrant init Ansible
  vagrant init Nginx
Step 7: Customize Vagrantfile for Ansible-Server
  Add line:
Step 8: Customize Vagrantfile for Nginx-Server
  Add line:
Step 9: Run vagrant box
  vagrant up
Step 10: SSH to Ansible-Server
  vagrant ssh
Step 11: Deploy Nginx using ansible
  sudo ansible-playbook /root/nginx_deploy/deploy_nginx.yml
Step 12: Check web page
  http://192.168.10.101/
    My name's Ha Manh Cuong.

    This is my LAB.

    Using Ansible to deploy Nginx virtual host in Vagrant Box.

    Thank you so much for reviewing.
