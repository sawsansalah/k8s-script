# k8s-script
Deployment Instructions:
Master Node Setup:

On the master node, run the script install-kubeadm-master.sh:
bash
chmod +x install-kubeadm-master.sh
sudo ./install-kubeadm-master.sh
Worker Node Setup:

On each worker node, run the script install-kubeadm-worker.sh:
bash
chmod +x install-kubeadm-worker.sh
sudo ./install-kubeadm-worker.sh
Joining Worker Nodes:

After running the worker node script, make sure to run the kubeadm join command that was output by the master node script on each worker node.
Verify the Cluster:

On the master node, verify that the worker nodes have joined the cluster:
bash
kubectl get nodes
This setup will install and configure Kubernetes with containerd as the container runtime and set up your master and worker nodes on Ubuntu 22.04.