<h2>Kubernetes excercies from day one!</h2>
<div>
This is a simple Go web application to serve "Hello Docker to Kubernetes!".

(You need already installed <a href="https://go.dev/doc/install">Go</a>)

Run this command in console to build a binary of this Go application. 
CGO_ENABLED=0 GOOS=linux GOARCH=amd64 go build -o docker-2-k8s

Build the Docker file by this:
> docker build -t docker-2-k8s:v0.0.1 .

Run it then:
> docker run -p 8080:8080 -d docker-2-k8s:v0.0.1

Optionaly tag it, and push it into your docker hub:
> docker login
> docker tag docker-2-k8s:v0.0.1 <your_DockerHub_username>/docker-2-k8s:v0.0.1
> docker push <your_username>/docker-2-k8s:v0.0.1

</div>  
