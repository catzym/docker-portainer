## 安装
### docker-compose 命令：
>
> git clone https://github.com/catzym/docker-portainer.git docker-portainer
> 
> cd docker-portainer
> 
> docker-compose up -d

### docker run 命令：
>
> docker run -d --name portainer --restart always -p 9000:9000 -v /var/run/docker.sock:/var/run/docker.sock -v /data/docker-portainer/portainer_data:/data -v /public:/public portainer/portainer

## 关闭
> docker-compose down

## 汉化包
> public文件夹，放到\根目录下

## 升级流程
> docker-compose 升级镜像：
>
> 1、docker-compose down 停止服务
>
> 2、docker-compose pull 更新image
>
> 3、docker-compose up -d 启动服务
>
> 4、docker image prune 删除旧的镜像