# docker-arm64-resilio-sync
## 描述
    这是一个 arm64 的 resilio sync docker 构建材料  
    闲暇之余可以通过树莓派输入资源 key 将资源同步下载  
    由于官网的sync是分布式的所以没什么安全性，不过是个不错的工具  
    配置文件 docker-compose.yml 默认端口开放是 9999 这个自己可以修改  
    整个项目不难，看看配置文件，看看脚本，再看看目录结构，看定就理解了
    .  
    ├── docker-compose.yml # 这个是 docker-compose.yml 配置文件  
    ├── Dockerfile # 这个是 docker 构建文件  
    ├── package # 这个是二进制文件、脚本、配置文件所在目录  
    │   ├── install.sh # 这个是构建镜像的时候在容器内执行流程的脚本  
    │   ├── rslsync # 这个是通过 arm64 设备安装官网安装包得到的二进制文件  
    │   ├── run_sync # 这个是启动 rslsync 的脚本  
    │   └── sync.conf # 这个是 rslsync 默认配置文件，也可以按照需求配置  
    └── ResilioSyncPro # 这个是就不做介绍了，自行研究吧，你懂的  
        └── ResilioSyncPro.btskey  

    2 directories, 7 files  

## 感谢
resilio sync 官网：https://www.resilio.com/  
Resilio, Inc. ：https://github.com/bt-sync  

## 参考
sync-docker：https://github.com/bt-sync/sync-docker  
