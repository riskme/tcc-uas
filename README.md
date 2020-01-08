# Kubernetes dengan Python-Flask

Langkah2 :
1. Membuat file pyhton yang akan di gunakan, dan menjadikan nya docker images di hub.docker
 
 file app.py

 ![](img/app.png)

 file requirement.txt

 ![](img/req.png)

 file Dockerfile

 ![](img/dockerfile.png)

2. Mengakses katacoda

Membuat cluster mikicube, dan menjalankan dashboard minikube

 

3. Membuat Pod dari Docker images yang ada di docker hub

kubectl create deployment python-flask --image=riskme/python-flask

![](img/1.png)

4. melihat Deployments

kubectl get deployments

![](img/2.png)

5. Melihat Pods

kubectl get pods

![](img/3.png)

6. Melihat cluster

kubectl get events

![](img/4.png)


7. melihat kubectl configuration

kubectl config view

![](img/5.png)

8. melihat hasil nya

kubectl expose deployment python-flask --type=LoadBalancer --port=8080

![](img/6.png)
