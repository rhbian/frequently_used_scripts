# 常用的shell

## 基本配置

### 阿里云-webdav

构建阿里云的webdav服务，可以在网页或者使用rclone进行连接
```shell
docker run -d --name=aliyundrive-webdav --restart=always -p 8080:8080 -v /etc/aliyundrive-webdav/:/etc/aliyundrive-webdav/ -v /etc/localtime:/etc/localtime -e TZ=Asia/Shanghai -e REFRESH_TOKEN='fbe038212bf14325aa2c8058480ff7be' -e WEBDAV_AUTH_USER=admin -e WEBDAV_AUTH_PASSWORD=admin messense/aliyundrive-webdav
```

# 内核配置
显卡配置

I2C_NVIDIA_GPU [=n] 无论是否含有nvidia，都需要去掉该选项

