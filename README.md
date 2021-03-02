# K8s-Cluster-Ansible

Here we have Ansible-role for AWS-instances having amazon-linux, Kubernetes-controller-node and Kubernetes-worker-node.

## Usage:

- Install ansible 2.9.0+ in your system.
- Clone this repository in any location you want.
- Create a folder "/etc/ansible" in your system.
- Copy the "ansible.cfg" file in /etc/ansible location.
- Open the ansible.cfg file and change the required parameters.
- Cd to the location of cloned repository.

For AWS  credentials, variables are available in aws role in vars folder.

- Run the playbook using "ansible-playbook aws-k8s.yml" command.

## Verification:

- Login to the master node.
- Verify cluster is fully running using kubectl:

```sh
kubectl get nodes
kubectl get pods
kubectl get pods -n "kube-system"
```
