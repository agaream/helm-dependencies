
kubectl create ns helmtest
kubectl create ns helmtest2

helm upgrade --install jurisdiction-helm jurisdiction -n helmtest
helm uninstall jurisdiction-helm jurisdiction -n helmtest

helm upgrade --install jurisdiction-helm jurisdiction2 -n helmtest2
helm uninstall jurisdiction-helm jurisdiction2 -n helmtest2