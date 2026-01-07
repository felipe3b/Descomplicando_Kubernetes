- Criando POD utilizando aqruivo yaml com "kubectl".


```bash
felipe3b@FELIPE-G3:~/Descomplicando_Kubernetes$ cd day-1/
felipe3b@FELIPE-G3:~/Descomplicando_Kubernetes/day-1$ ls -l
total 8
-rw-r--r-- 1 felipe3b felipe3b  52 Jan  7 10:56 dia-1.md
-rw-r--r-- 1 felipe3b felipe3b 250 Jan  7 10:32 pod.yaml
felipe3b@FELIPE-G3:~/Descomplicando_Kubernetes/day-1$ kubectl apply -f pod.yaml
pod/giropops created
felipe3b@FELIPE-G3:~/Descomplicando_Kubernetes/day-1$ kubectl get pod
NAME       READY   STATUS    RESTARTS   AGE
giropops   1/1     Running   0          7s
felipe3b@FELIPE-G3:~/Descomplicando_Kubernetes/day-1$ kubectl delete pod giropops
pod "giropops" deleted from default namespace
felipe3b@FELIPE-G3:~/Descomplicando_Kubernetes/day-1$
```