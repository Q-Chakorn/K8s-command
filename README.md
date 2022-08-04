# K8s-command

deploy file yaml
- kubectl apply -f <filename>
- kubectl apply -f . <allfile>
- kubectl delete -f <filename>
- kubectl delete -f . <allfile>

- kubectl get nodes
- kucectl get pods -A
- kubectl get service -n <namespace>
- kubectl get configmap -n <namespace>


- kucectl get pods -n <namespace> <แสดง pods ใน namespace>
- kubectl describe pods <namepods> -n <namespace> <แสดงdetailในpods>

- kubectl get deployment -n <namespace> <deployname> <แสดง deployment ใน namespace>
- kubectl describe deployment -n <namespace> <deployname> <เแสดงdetailในdeployment>

- kubectl get pvc -n <namespace>
- kubectl describe pvc <name> -n <namespace> <เแสดงdetailใน pvc>

- kubectl logs <namepod> -n <namespace>


- kubectl exec -it -n <namespace> <namepods> -- sh <เข้าไปภายในpods>

- kubectl create configmap center-http-config --from-file=httpd.conf -o yaml --dry-run | kubectl replace -f - -n mocha-center
