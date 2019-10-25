# mongodb-k8s

      kubectl get nodes
      git clone https://github.com/ksravikumar2005/mongodb-k8s.git
      cd mongodb-k8s/
      cat mongodb-datadb-pv.yaml 
      mkdir -p /tmp/uservolumes/mongo-datadb
      chown -R 1000:1000 /tmp/uservolumes/mongo-datadb
      kubectl create -f mongodb-datadb-pv.yaml 
      kubectl describe persistentvolume/mongodb-datadb-pv
      kubectl get pv
      cat mongodb-datadb-pvc.yaml 
      kubectl create -f mongodb-datadb-pvc.yaml 
      kubectl get pvc
      kubectl create -f mongodb-pod-definition.yaml 
      kubectl get pods
      kubectl describe pod/mongodb
      docker ps
