```
1177  mkdir 28-Helm-Custom-Charts
 1178  cd 28-Helm-Custom-Charts/
 1179  ls
 1180  helm create mychart
 1181  ls
 1182  cd mychart/
 1183  ls
 1184  cat Chart.yaml
 1185  ls
 1186  cd templates/
 1187  s
 1188  ls
 1189  vim deployment.yaml
 1190  ls
 1191  cd ..
 1192  ls
 1193  vim values.yaml
 1194  ls
 1195  cd ..
 1196  ls
 1197  helm install mynginx mychart --dry-run
 1198  helm install mynginx mychart
 1199  kubectl  get deploy,rs,pod,svc
 1200  helm list
 1201*
 1202  helm create mypychart
 1203  ls
 1204  cd mypychart/
 1205  ls
 1206  vim values.yaml
 1207  ls
 1208  vim templates/deployment.yaml
 1209  ls
 1210  vim values.yaml
 1211  ls
 1212  cd ..
 1213  ls
 1214  helm install mypywebapp mypychart --dry-run
 1215  helm install mypywebapp mypychart
 1216  kubectl  get pods,svc
 1217  kubectl  get pods -o wide
 1218  ls
```
