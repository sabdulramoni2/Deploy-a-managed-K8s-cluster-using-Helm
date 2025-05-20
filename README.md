# Helm-Demo-Managed-K8s-cluster


## **Project Overview**
This project demonstrates deploying a managed K8s cluster on Linode Kubernetes engine, deployed a replicated database and configure its persistence and make it accessible through a UI client browser using ingress.

---

## **Features**
- Linode K8 cluster set up
  - Created K8 cluster on Linode engine.
  -	Downloaded the kubeconfig.yaml file to your laptop to access the cluster remotely.
  - Set the correct permission on the file using, chmod 400 “file name”.
  - Set kubeconfig.yaml file as an environmental variable. 
  - Export KUBECONFIG= kubeconfig. yaml (LINUX OS).
  -	Set KUBECONFIG= kubeconfig. yaml (WINDOWS OS).
  -	Run kubectl get node.
- SECOND STEP
  -	Deploy MongoDB StatefulSet into the cluster using Helm chart.
  -	Install Helm into the environment.
  - Add the repository that have the helm chart. 
  -	Search the repository (helm search repo “repo name”).
  - Search the repository (helm search repo bitnami/mongodb).
  - The chart allows you to overwrite some values using the values files.
      -	Architecture: replicaset
      - Persistence: Storage class
      - Auth : rootPassword: Secret
  - Run “ helm install our name –values [values file name] [chart name = repository/resource name]”
  - Run helm install mongodb –values helm-mongo.yaml bitnami/mongodb.
  - Run “kubectl get pod” to see the pods.
  - Check to see if all components are created; services, StatefulSets, volume. 
  - Now we have a Mongodb with a persistent volume in the cluster.
  - THIRD STEP (Deployment of MongoExpress)




## **Features**
- Created K8s cluster on Linode Kubernetes Engine
- Deployed replicated MongoDB (StatefulSet using Helm Chart) and configured Data Persistence with Linode Block Storage
- Deployed MongoExpress (Deployment and Service)
- Deployed NGINX Ingress Controller as Loadbalancer (using Helm Chart)
- Configured Ingress rule
 
---

## **Features**
- Created K8s cluster on Linode Kubernetes Engine

  ![image](https://github.com/user-attachments/assets/40763b09-0f0d-4f7b-82fa-7e1cf76deaab)

- Set permission on the kubeconfig file and set as evn
  

  ![image](https://github.com/user-attachments/assets/a98825b5-6626-4b8d-a9d2-b000ec45250b)
  

  ![image](https://github.com/user-attachments/assets/f2c1112e-7120-482b-aac1-def74a2c73a4)



- Deployed replicated MongoDB (StatefulSet using Helm Chart) and configured Data Persistence with Linode Block Storage

  ![image](https://github.com/user-attachments/assets/ffdc8208-f02a-4e4b-a2c1-00fa64bffee4)
  

  ![image](https://github.com/user-attachments/assets/cc1482b5-115b-4610-88c4-7c829010a158


  ![image](https://github.com/user-attachments/assets/ab71e687-0cd9-4b33-bf98-c606006e9b54)



- Deployed MongoExpress (Deployment and Service)

  ![image](https://github.com/user-attachments/assets/4a8d4d42-5c02-4ed2-a958-57ad0bd7facd)

- Deployed NGINX Ingress Controller as Loadbalancer (using Helm Chart)

  ![image](https://github.com/user-attachments/assets/b970bc50-153f-48bd-92ed-331a0ed3c6b4)

- Configured Ingress rule

  ![image](https://github.com/user-attachments/assets/626eb546-c9cc-4960-ad31-e7dd2b326c35)


  ![image](https://github.com/user-attachments/assets/c3ed9756-83b8-4bf5-996f-5124265fab37)
  

  ![image](https://github.com/user-attachments/assets/a31547e3-db42-4f2f-93f2-9c179db2a82c)


  ![image](https://github.com/user-attachments/assets/b83f3765-eaa9-4863-9aea-163aaa198746)


  ![image](https://github.com/user-attachments/assets/b2b40fb6-45e1-47d4-9b9b-97beae060e06)





 
---
