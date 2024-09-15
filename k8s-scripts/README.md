If you want to test that KubeDNS is working as expected and hosts are resolving and can connect:\
kubectl run -i --tty --rm debug --image=busybox --restart=Never -- sh\
Execute\
wget -qO- http://<CLUSTER-IP>\
Acts as a load on the service
while true; do wget -q -O- http://10.105.134.226/maven-web-application; done
