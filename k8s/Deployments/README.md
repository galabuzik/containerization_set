**K8S Deployments Basics**

1. kubectl create -f nginx-deployment.yaml -> _Create a Deployment using the Deployment YAML file_

2. kubectl get deployments - _Get all deployments_

![image](https://user-images.githubusercontent.com/19956502/130780431-662b3422-2091-4c43-b216-300de6b69fd9.png)

3. kubectl get deployments nginx-deployment -o jsonpath --template {.spec.selector.matchLabels} -> _Get label and label selector of a deployment_

![image](https://user-images.githubusercontent.com/19956502/130780873-4e4c2567-e4b6-4403-a7f5-e57b709d2c07.png)


4. kubectl get replicasets --selector=app=nginx -> _Get the specific replicaset from a deployment_
_The example below will get the replicaset that is part of the app:nginx deployment that we fecthed above._

![image](https://user-images.githubusercontent.com/19956502/130781083-67353ff7-8de5-4ec1-8633-dfde967cf9e3.png)

5. kubectl scale deployments nginx-deployment --replicas=2 -> _Scale the replicasets within a deployment to 2_

![image](https://user-images.githubusercontent.com/19956502/130782040-2c0b1b17-90f9-4bda-a497-52b55dede2d6.png)


6.kubectl describe deployments nginx-deployment - _Get details about your Kubernetes deployment._

![image](https://user-images.githubusercontent.com/19956502/130783632-48abb4a1-308f-46b9-a42b-f8074eac93c2.png)
















