[200~kind create cluster --config=kind-config.yaml 
Creating cluster "kind" ...
 ✓ Ensuring node image (kindest/node:v1.29.2) 🖼 
  ✓ Preparing nodes 📦 📦 📦 📦  
   ✓ Writing configuration 📜 
    ✓ Starting control-plane 🕹️ 
     ✓ Installing StorageClass 💾 
      ✓ Joining worker nodes 🚜 
      Set kubectl context to "kind-kind"
      You can now use your cluster with:

      kubectl cluster-info --context kind-kind

      Have a nice day! 👋
      root@instance-20240305-124116:/home/laplastech# cat kind-config.yaml 
      kind: Cluster
      apiVersion: kind.x-k8s.io/v1alpha4
      nodes:
      - role: control-plane
      - role: worker
      - role: worker
      - role: worker
      networking:
        disableDefaultCNI: true
        root@instance-20240305-124116:/home/laplastech# 

`kind create cluster --config=kind-config.yaml`




