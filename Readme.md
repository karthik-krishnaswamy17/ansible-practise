Simple ansible playbook to install docker services.

After cloing the repo,create host file named <bold>hosts</bold> and add below contents.

<bold>
[ec2_webserver]
</bold>
# List of Instance IPS
XXX.XXX.XXX.XXX
XXX.XXX.XXX.XXX
<bold>
[ec2_webserver:vars]
</bold>
ansible_ssh_private_key_file= <bold> <Path of private key file> </bold>
ansible_user=<bold>username</bold>
ansible_ssh_common_args='-o StrictHostKeyChecking=no'

