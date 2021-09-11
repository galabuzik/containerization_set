**ConfigMaps and Secrets**

1. kubectl create configmap my-config --from-file=my-config.txt --from-literal=extra-param=extra-value --from-literal=another-param=another-value - _Create a config map from a file and add sample key value pairs._

![image](https://user-images.githubusercontent.com/19956502/132955792-1ec24587-94b8-4927-bed6-5c24725965df.png)

2.kubectl get configmaps my-config -o yaml - _Get YAML object for the conig map that you have created._

![image](https://user-images.githubusercontent.com/19956502/132955806-2664475b-60e6-478c-969f-1b26629b23b0.png)

![image](https://user-images.githubusercontent.com/19956502/132955830-c2189bf3-8db3-4999-ba7b-be93fc23ea9a.png)

