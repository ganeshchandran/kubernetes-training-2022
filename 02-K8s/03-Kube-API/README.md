```
   27  kubectl  get pods -n kube-system
   28  cat /etc/kubernetes/
   29  ls
   30  cd /etc/kubernetes/
   31  ls
   32  cd manifests/
   33  ks
   34  ls
   35  vim kube-apiserver.yaml 
   36  cd 
   37  ls
   38  cd docker-kubernetes-ericsson-20-Dec-2021/
   39  ls
   40  cd 02-K8s/
   41  ls
   42  cat 00-Setup/install-k8s-master-node.sh 
   43  ls
   44  kubectl cluster-info
   45  kubectl version 
   46  kubectl api-versions 
   47  kubectl api-resources 
   48  curl http://172.31.0.100:6443
   49  curl https://172.31.0.100:6443
   50  curl -k https://172.31.0.100:6443
   51  kubectl proxy --address='172.31.0.100' --port=8080 --accept-hosts='.' --accept-paths='.' &
   52  curl  http://172.31.0.100:8080
   53  curl  http://172.31.0.100:8080/api
   54  curl  http://172.31.0.100:8080/apis
   55  kubectl  get pods -o wide 
   56  ls
   57  kubectl config view
   58  kubectl config get-contexts
   59  ls
   60  mkdir 03-Kube-API
   61  history > 03-Kube-API/README.md
```
