checkout the blog on this project -->https://aakibkhan1.medium.com/project-6-deployment-of-super-mario-on-kubernetes-using-terraform-74c7ce79b1f6

Step 1 - Create a Virtual Machine on Microsoft Azure 

Step 2 - Connect the Virtual Machine and install Azure CLI & kubectl and clone the repository.

Step 3 - After installing and setting up the Docker and Azure CLI launch an AKS cluster with the default configurations, make sure the node pool has the desired size to host your application.

Step 4 - Once you have cloned the repository in the VM and your AKS cluster is ready get the credentials and update the context to connect it with kubectl.

Step 5 - Now apply the service and deployment files using the kubectl command:
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml

Step 6 - Finally your deployment and service are created and applied in the AKS cluster and after 2 to 3 minutes your external IP should be visible and you can access your application (Super Mario)
kubectl get all


Step 7 - Finally terminate or delete all the resources so that you don't get billed.


