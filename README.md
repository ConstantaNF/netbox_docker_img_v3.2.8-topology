# ****Образ netbox_docker_img_v3.2.8-topology c установленным плагином netbox-topology-views v2.0.3**** #

Версия helm chart <https://github.com/netbox-community/netbox-chart/tree/4.1.1>

Версия плагина <https://github.com/netbox-community/netbox-topology-views/tree/v2.0.3>

Разворачивал через helm командой

```
helm install kube-netbox --version 4.1.1 --values values1.yaml bootc/netbox
```

В случае необходимости добавления pvc для media 

```
kubectl apply -f netbox-media-pvc.yaml
```

В случае необходимости добавления pvc для static

```
kubectl apply -f netbox-static-pvc.yaml
```
