apiVersion: v1
kind: Pod
metadata: 
 name: nginx 
spec:
 containers:
 - name: nginx 
   image: nginx:1.7.9 
   ports: 
   - containerPort: 80
 - name: springapp
   image: yanivomc/spring-music:latest
   ports: 
   - containerPort: 8080