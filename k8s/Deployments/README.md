**K8S Deployments Basics**

kubectl create -f nginx-deployment.yaml - Create a Deployment using the Deployment YAML file

kubectl get deployments - Get all deployments

![image](https://user-images.githubusercontent.com/19956502/130780431-662b3422-2091-4c43-b216-300de6b69fd9.png)

kubectl get deployments nginx-deployment -o jsonpath --template {.spec.selector.matchLabels} - Get label and label selector of a deployment

![image](https://user-images.githubusercontent.com/19956502/130780873-4e4c2567-e4b6-4403-a7f5-e57b709d2c07.png)


kubectl get replicasets --selector=app=nginx - Get the specific replicaset from a deployment
The example below will get the replicaset that is part of the app:nginx deployment that we fecthed above.

![image](https://user-images.githubusercontent.com/19956502/130781083-67353ff7-8de5-4ec1-8633-dfde967cf9e3.png)













