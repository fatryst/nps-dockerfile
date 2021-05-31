# nps
  - `docker run -d --name nps --net=host -v <本机conf目录>:/conf zengfa/nps`
  
# npc

- 无配置文件：`docker run -d --name npc --net=host zengfa/npc -server=<ip:port> -vkey=<web界面中显示的密钥> <以及一些其他参数> `

- 配置文件：`docker run -d --name npc --net=host -v <本机conf目录>:/conf zengfa/npc -config=/conf/npc.conf`
