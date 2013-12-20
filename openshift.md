### Openshift bash profile
* $OPENSHIFT_DATA_DIR/.bash_profile文件类似普通$HOME/.bash_profile,
所以可以在这里指定一些ENV

### Openshift port
openshift 可以访问8000端口

### cloud9
cloud9在启动的时候，需要指定smith.io port，不然在openshift上请求smith
server的时候，会默认用启动的端口(默认8080)，而启动的端口是没法直接访问的，需要openshift
代理才能访问，如果指定到8000端口就能访问, 因为openshift 8000端口也是可以访问的
