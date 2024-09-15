If you want to test that KubeDNS is working as expected and hosts are resolving and can connect:\
kubectl run -i --tty --rm debug --image=busybox --restart=Never -- sh\
Execute\
wget -qO- http://<CLUSTER-IP>

