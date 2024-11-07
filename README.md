# LAB1

## Các bước thực hiện
### Tạo file yaml
Viết file `lab1.yaml` để tạo `service` và  `Deployment`.
### Trước khi tạo `Deployment` ta kiểm tra cụm:
![This is an alt text.](https://i.imgur.com/T4vK9Qu.png "This is a sample image.")
### Tạo Service và Deployment với câu lệnh:
```
kubectl apply -f lab1.yaml

```
#### Sau khi tạo ta kiểm tra hoạt động của Service và các Pod đã được tạo:
![This is an alt text.](https://i.imgur.com/dB4LC2g.png "This is a sample image.")
### Sử dụng lệnh để khởi động `Service`
```
minikube service nginx-default-service

```
#### Minikube tự động mở trình duyệt mặc định:
 ![This is an alt text.](https://i.imgur.com/VMraf3E.png "This is a sample image.")
 ![This is an alt text.](https://i.imgur.com/DV5NrMu.png "This is a sample image.")
#### Ta có thể truy cập Pod Nginx thông qua câu lệnh curl `http://<node-IP>:NodePort `nếu cụm của bạn có EXTERNAL-IP
#### Ở đây do sử dụng cụm minikube nên ta sử dụng lệnh: 
```
curl http://127.0.0.1:80

```
