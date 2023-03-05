# k3s
Raspberry pi k3s install

Provided your inventory has the groups "kube-managers" and "kube-workers" with your targets this should work fine for you.

example of hosts file below.


---
[kube-managers]
kube-manager ansible_ssh_host=192.168.1.110

[kube-workers]
kube-worker-1 ansible_ssh_host=192.168.1.111
kube-worker-2 ansible_ssh_host=192.168.1.112
kube-worker-3 ansible_ssh_host=192.168.1.113
kube-worker-4 ansible_ssh_host=192.168.1.114