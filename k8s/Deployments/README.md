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


6.kubectl describe deployments nginx-deployment -> _Get details about your Kubernetes deployment._

![image](https://user-images.githubusercontent.com/19956502/130783632-48abb4a1-308f-46b9-a42b-f8074eac93c2.png)

7.kubectl apply -f nginx-deployment.yaml -> _Apply changes to current deployment after modifying the updated deployment yaml manifest._

![image](https://user-images.githubusercontent.com/19956502/131026613-f7594d7a-dace-41ff-a931-89e56275d89b.png)

8.kubectl rollout status deployments nginx-deployment -> _Check the status of a previously rolled out Kubernetes deployment._

![image](https://user-images.githubusercontent.com/19956502/131027127-229aa3af-3304-4498-ae6f-f39a907c2a26.png)

9.kubectl get replicasets -o wide -> _Get current replicasets._

![image](https://user-images.githubusercontent.com/19956502/131027330-b3c08804-2453-4d3f-8de8-7cc8c966c7d2.png)

10. kubectl rollout pause deployments nginx-deployment -> _Pause a Kubernetes Deployment incase of any issues._

![image](https://user-images.githubusercontent.com/19956502/131027754-76e9c0c8-52c4-4c11-a3c2-cbb3ec69bcca.png)

11. kubectl rollout resume deployments nginx-deployment -> _Resume a Kubernetes Deployment._

![image](https://user-images.githubusercontent.com/19956502/131027952-495d45c8-373a-4908-b5db-89d12b5aa517.png)

12.kubectl rollout history deployment nginx-deployment -> _View rollout history_

![image](https://user-images.githubusercontent.com/19956502/131087965-b86e0599-bebc-41f5-a0a5-a6d173b91bf9.png)

13. kubectl rollout history deployment nginx-deployment --revision=1 -> _View the details of a specific revision._

![image](https://user-images.githubusercontent.com/19956502/131088226-67f77ca9-1e00-4d9c-abc0-a52abfea7a3d.png)

14.kubectl rollout undo deployments nginx-deployment -> _Roll back to a previous deployment._

![image](https://user-images.githubusercontent.com/19956502/131088805-bcef461d-7d18-484d-83db-43e96d0851f2.png)




















