** 1. docker架构
<img width="766" height="407" alt="image" src="https://github.com/user-attachments/assets/5e744fea-fc78-4f70-a916-d3a4baa4cd5d" />
- 将资源打包成镜像，并存储在registry镜像仓库中，在镜像仓库中拉取镜像并存入本地，在本地通过 docker run 等命令运行镜像

** 2. 安装镜像
<img width="1443" height="868" alt="image" src="https://github.com/user-attachments/assets/dee270fe-1198-4d01-b313-a359a8b86e8d" />
- 安装完docker以后可以直接通过docker images和docker search来搜取镜像
<img width="664" height="223" alt="image" src="https://github.com/user-attachments/assets/0f5205dd-bc75-4710-a433-1ae19e11d49f" />

- 相关的属性如上图所示

- 使用pull命令拉取镜像
<img width="729" height="235" alt="image" src="https://github.com/user-attachments/assets/26baf843-66c3-4bd6-86f5-7b41a9c9cdec" />

- docker rmi可以删除镜像
<img width="1537" height="280" alt="image" src="https://github.com/user-attachments/assets/826d1acc-efa2-43b8-a5d5-f19de5035690" />

- 默认网卡是docker0，这是一个桥接的网卡，容器利用这一网卡与宿主机通信
<img width="1105" height="592" alt="image" src="https://github.com/user-attachments/assets/eef6a2d2-b940-4f3c-91dc-42c355d2d136" />

- 还有一些其他的模式：
<img width="1039" height="597" alt="image" src="https://github.com/user-attachments/assets/bedab045-160a-4b59-9e09-a1d6d2e2e729" />


** 3. dockerfile与构建镜像
- 在dockerfile中添加nginx所在的路径，.代表当前路径，打包一个镜像并运行，可以看到镜像已经成功运行
<img width="757" height="248" alt="image" src="https://github.com/user-attachments/assets/6f07f8a4-0ad9-4a39-9558-8cb759941329" />
<img width="588" height="58" alt="image" src="https://github.com/user-attachments/assets/f4225816-4828-4132-9b59-7f38be5c18df" />

<img width="681" height="256" alt="image" src="https://github.com/user-attachments/assets/5a93dd0d-630f-482d-a2c5-bc7881205fef" />
- 接着使用docker build来构建镜像
<img width="1026" height="591" alt="image" src="https://github.com/user-attachments/assets/4257a676-0bfe-413d-92c5-0220f3f81b34" />
<img width="1680" height="546" alt="image" src="https://github.com/user-attachments/assets/88423f2e-7e8f-4978-917b-00a5f7706770" />

- 可以直接执行docker run，在配置中心地址拉取配置












