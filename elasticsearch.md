# Elasticsearch notes

## Setup

有两张方式
* stand alone 
* as a linux service

### stand alone

只要下载zip包，解压就可以，配置plugins, config/elasticsearch.yml,
系统ulimits参数等就可以启动

### as linux service

下载linux 发行版对应的pkg安装

启动服务和系统相关的设置, 默认的配置文件在 /etc/default/elasticsearch,
在该文件中可以配置一些启动参数，环境变量等。

es配置文件在/etc/elasticsearch/elasticsearch.yml，该文件中可以对elasticsearch本身的功能进行配置，
比如配置一些analyzer, tokenizer等等

init script => /etc/init.d/elasticsearch

ES_HOME => /usr/share/elasticsearch

plugins 安装在 ES_HOMES/plugins 下面


## 中文版本

https://github.com/medcl/elasticsearch-rtf

需要的一些插件可以按照从这个版本中获取

## 插件列表页

http://www.elasticsearch.org/guide/en/elasticsearch/reference/current/modules-plugins.html
