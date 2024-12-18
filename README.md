## Deployment Instructions

### Master Node Setup

1. On the master node, run the script `install-kubeadm-master.sh`:
   ```bash
   chmod +x install-kubeadm-master.sh
   sudo ./install-kubeadm-master.sh

Worker Node Setup

On each worker node, run the script `install-kubeadm-worker.sh`:
   ```bash

chmod +x install-kubeadm-worker.sh
sudo ./install-kubeadm-worker.sh
    bash```

Joining Worker Nodes
After running the worker node script, make sure to run the kubeadm join command that was output by the master node script on each worker node.

Verify the Cluster

kubectl get nodes