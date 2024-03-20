# K8s-Deployment of httpd pod

# STEP 1
 create pv and pvc through yaml

# STEP 2
 create pod1 and pod2 through yaml

# STEP 3
  Now, create a index.html which you are going to deploy

# STEP 4
  Get acces to the cluster, install kubernetes or use killarcoda 

# STEP 5 
 make a dir where you have to store your index.html file and this location should be as simillar to the path we mention while creating pv

# STEP 6
 Use git clone to clone all your codes and files. After that apply all the codes by using below syntax
        kubectl apply -f .

# STEP 7 
 Now, cp index.html to /usr/local/apache2/htdocs/index.html on both the pods
        kubectl cp index.html my-pod1:/usr/local/apache2/htdocs/index.html             .... for pod1
        kubectl cp index.html my-pod1:/usr/local/apache2/htdocs/index.html             .... for pod2

# STEP 8
 Now check the pods use command as below
         kubectl get pods
         kubectl get pods -o wide

# STEP 9 
 Now curl the ip of the pods

