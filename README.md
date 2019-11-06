基于 MNS 与 OSS 实现人脸图片识别

### Broker
```
kubectl label namespace default knative-eventing-injection=enabled
```

### Service Account and Secret

```
kubectl apply --filename source/mnss-pre.yaml
```

### MnsOssSource

```
kubectl apply --filename source/mnsosssource.yaml
```


### Knative Service

```
kubectl apply --filename face-service.yaml
```

### Trigger

```
kubectl apply --filename face-trigger.yaml
```