# NGINX-vagrant
Vagrant and ansible playbooks to provision a simple CentOS 7  VM with NGINX+ and app protect in a basic configuration.

# Prereqs
1) Vagrant
2) A valid NGINX+ key and cert in the host ~/secrets directory
3) A bridged interface so it's possible to connect to the webserver.
4) Ansible 2.9+


# To run

    git clone https://github.com/my0373/NGINX-vagrant.git
    cd NGINX-vagrant
    vagrant up
    
    
At the end of run you'll see the IP address of the machine printed out to connect to.


You will then be able to connect to the dashboard at http://[ip-address]/dashboard
You can test App Protect is working with a fake XSS URI
    http://[ip-address]/dashboard?a=<script>


# Official documentation
### Admin install guide
https://docs.nginx.com/nginx-app-protect/admin-guide/install

### Configuring App-protect
https://docs.nginx.com/nginx-app-protect/configuration/

### Policy authoring guide
https://docs.nginx.com/nginx-app-protect/configuration/#policy-authoring-and-tuning
