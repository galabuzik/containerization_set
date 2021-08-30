**DaemonSets**

1. kubectl get daemonset --namespace kube-system -> _Get all daemon sets running in the kube-system namespace._

![image](https://user-images.githubusercontent.com/19956502/131334426-f50f53b5-5de8-4f4b-a656-0eece9be106b.png)

2. kubectl describe daemonset fluentd --namespace kube-system -> _Describe the daemon set fluentd in the kube-system namespace._

![image](https://user-images.githubusercontent.com/19956502/131334672-820a8f32-bf7b-485b-b810-8fc17166f448.png)

3. kubectl get pods -o wide --namespace kube-system -> _Get all pods running in the kube-system namespace._

![image](https://user-images.githubusercontent.com/19956502/131334807-a1137cda-bb13-4262-9ffe-1700b4811ea2.png)

4. kubectl get nodes -> _Get nodes on the cluster._

![image](https://user-images.githubusercontent.com/19956502/131362280-67b99273-f41c-4c83-a1fe-5bce87742b63.png)

5. kubectl label nodes master-node ssd=true -> _Label the master node to have a label of ssd=true._

![image](https://user-images.githubusercontent.com/19956502/131362425-2724c05e-7439-46d9-b0a8-cad7a91eaa7e.png)

6. kubectl get nodes --selector ssd=true -> _Get nodes where by the label is ssd=true._

![image](https://user-images.githubusercontent.com/19956502/131362559-72a732a2-9a64-453b-84f0-a734d250d4f7.png)






