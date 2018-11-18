# deploy_nginx
<p>Step by step: Using Ansible to deploy Nginx virtual host into Vagrant Box </p>.
<p>Step 1: Tạo folder để chứa Vagrant Box file</p>
<p>Step 2: Clone 2 Box files.</p>
<p>  git clone</p>
<p>Step 3: Add the Box into Vagrant Install</p>
<p>  vagrant box add Ansible-Server Ansible.box</p>
<p>  vagrant box add Nginx-Server Nginx.box</p>
<p>Step 4: Initialize New Vagrant Box</p>
<p>  vagrant init Ansible</p>
<p>  vagrant init Nginx</p>
<p>Step 7: Customize Vagrantfile for Ansible-Server</p>
<p>  Add line:</p>
<p>Step 8: Customize Vagrantfile for Nginx-Server</p>
<p>  Add line:</p>
<p>Step 9: Run vagrant box</p>
<p>  vagrant up</p>
<p>Step 10: SSH to Ansible-Server</p>
<p>  vagrant ssh</p>
<p>Step 11: Deploy Nginx using ansible</p>
<p>  sudo ansible-playbook /root/nginx_deploy/deploy_nginx.yml</p>
<p>Step 12: Check web page</p>
<p>  http://192.168.10.101/</p>
<p>    My name's Ha Manh Cuong.</p>
<p>    This is my LAB.</p>
<p>    Using Ansible to deploy Nginx virtual host in Vagrant Box.</p>
<p>    Thank you so much for reviewing.</p>
