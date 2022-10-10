# docker images
# gcr镜像同步

FROM quay.io/cephcsi/cephcsi:v3.5.1
FROM k8s.gcr.io/sig-storage/csi-node-driver-registrar:v2.4.0
FROM k8s.gcr.io/sig-storage/csi-resizer:v1.4.0
FROM k8s.gcr.io/sig-storage/csi-provisioner:v3.1.0
FROM k8s.gcr.io/sig-storage/csi-snapshotter:v5.0.1
FROM k8s.gcr.io/sig-storage/csi-attacher:v3.4.0
FROM quay.io/ceph/ceph:v16.2.7
FROM quay.io/mobz/elasticsearch-head
FROM k8s.gcr.io/ingress-nginx/controller:v1.1.1
FROM k8s.gcr.io/ingress-nginx/kube-webhook-certgen:v1.1.1
FROM k8s.gcr.io/ingress-nginx/defaultbackend-amd64:1.5
FROM k8s.gcr.io/prometheus-adapter/prometheus-adapter:v0.9.1
