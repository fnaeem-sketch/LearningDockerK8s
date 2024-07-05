# Underderstanding Pods
- In Kubernetes terms, a container is referred to as a pod. 
- A node is a worker machine in Kubernetes. 
- Each node is managed by a Master. 
- A Node can have multiple pods. 

We can configure Kubernetes pods using a YAML file

# Kubernetes Clusters
- etcd is where the configuration data is stored 

1. kube-apiserver
The kube-apiserver acts as the front door for the Kubernetes control plane. It's the component through which all the requests to the system are managed. It handles and processes all the REST requests and updates the state of the objects in etcd, ensuring that deployments and other Kubernetes functions are correctly maintained.

2. etcd
etcd is a highly available key-value store used to store all the data needed to manage the cluster state. Think of it as the "memory" of your Kubernetes cluster, storing configuration data, state, and metadata of various Kubernetes objects. It is crucial for the consistency and reliability of the cluster, keeping track of everything happening within Kubernetes.

3. kube-scheduler
The kube-scheduler is responsible for scheduling pods onto nodes. It selects the most suitable node for a pod to run on based on resource availability (like CPU and memory), constraints, affinities, and other factors. Essentially, it decides which machines in the cluster will run the workloads based on their current workload and the workload's specific requirements.

4. Useful Tools
Utilize tools that can help make these concepts clearer:

Kubernetes Dashboard: This is a web-based Kubernetes user interface. It allows you to manage applications running in the cluster and troubleshoot them, as well as manage the cluster itself.
Lens: A Kubernetes IDE that provides a clearer, real-time visualization of your Kubernetes clusters. It helps you to manage your clusters in a more user-friendly way than the CLI.
K9s: Provides a terminal UI to interact with your Kubernetes clusters, which can help in simplifying the command-line outputs.

