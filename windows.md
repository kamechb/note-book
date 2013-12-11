#Windows下端口映射

## 有时公司发里laptop用来链接内网，访问内网的服务，当需要从其他机器访问内网的服务时，可以通过laptop进行端口映射，就能很方便的在其他机器上访问内网服务了

### 命令
netsh interface portproxy add v4tov4 listenport=laptopport listenaddress=laptopaddress
connectport=targetport connectaddress=targethost

### 举例
netsh interface portproxy add v4tov4 listenport=3000
connectport=3000 connectaddress=xx.xx.xx.xx
