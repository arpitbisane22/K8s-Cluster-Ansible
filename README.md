# K8s-Cluster-Ansible
Here we have Ansible-role for AWS-instances, kubernetes-controller-node and Kubernetes-worker-node.

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
