unable to attach or mount volume: unmounted volumes=[wordpress-data], unattached volumes=[wordpress-data kube-api-access-2vtq7]: time out waiting for the condition

MountVolume.NewMounter initalization failed for volume "wordpress-pv" : path "/data" does not exist

goto the the node and create directory /data where the pod is running by describing the pod

mkdir /data

kubectl rollout restart deployment wordpress

kubectl get pod