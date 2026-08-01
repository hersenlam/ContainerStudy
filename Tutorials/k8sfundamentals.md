#https://www.youtube.com/watch?v=9AKSLbfen6w

install rancher desktop to get a cluster up and running as a beginner on whatever OS / machine 

Command to keep on refreshing / live feed of your pods:

`
watch -n 0.2 "kubectl get pods"
`

# Kubernetes networking @11:57

`
k get pods -o wide

k delete pod <podname>

k get pods -o wide
`

This shows that the IP is constantly changing. So there's no way you can point smt at the IP.
--> solved in Kubernetes by using services, which will route traffic to the pods (clusterIP service).

Now you can deploy your first service by:

`
kubectl expose deployment my-nginx --port=80
k get service my-ngninx
`

That will be an IP that will always be stable. 

To access:
`
k port-forward svc/my-nginx 8080:80 
`

if you go now to localhost:8080 in your browser, you can see nginx say welcome!

# Kubernetes scaling
`
kubectl scale deployment my-nginx --replicas=10
k get pods | wc -l
`

this last command will show the amount of lines the k get pods command returns (all the pods + top line that indicates the columns)

`
k get deployments.apps
`

# clean-up
`
k get svc
kubectl delete service my-nginx
k get deployments.apps
kubectl delete deployemnts.apps my-nginx
k get pods
`


