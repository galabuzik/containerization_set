**ConfigMaps and Secrets**

1. kubectl create configmap my-config --from-file=my-config.txt --from-literal=extra-param=extra-value --from-literal=another-param=another-value - _Create a config map from a file and add sample key value pairs._

![image](https://user-images.githubusercontent.com/19956502/132955792-1ec24587-94b8-4927-bed6-5c24725965df.png)

2.kubectl get configmaps my-config -o yaml - _Get YAML object for the conig map that you have created._

![image](https://user-images.githubusercontent.com/19956502/132955806-2664475b-60e6-478c-969f-1b26629b23b0.png)

3. kubectl create secret generic kuard-tls --from-file=kuard.crt --from-file=kuard.key - _Create a secret from two files, the kuard.crt and kuard.key file._

![image](https://user-images.githubusercontent.com/19956502/132956622-74554b94-0c19-4f52-a10d-bd0a5d9f5ddf.png)

4. kubectl describe secrets kuard-tls - _Get information about a Secret._

![image](https://user-images.githubusercontent.com/19956502/132956661-1be4a7dc-d80e-432a-8ee2-76184f961fcc.png)

5. kubectl get secrets - _List all secrets in the current namespace._

![image](https://user-images.githubusercontent.com/19956502/132960719-3d56307d-3d93-4ee1-a46c-002f44b57190.png)

6. kubect get configmaps - _List all configmaps in a namepsace._

![image](https://user-images.githubusercontent.com/19956502/132960736-c3b17399-a143-41df-830c-515157eac556.png)



