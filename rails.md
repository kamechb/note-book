### 创建需要版本的rails的项目

一般情况下，我们可能会安装了好几个版本的rails，包括最新的rails版本，所以这种情况下，
rails new [project-name] 会用最新版本的rails 去创建,
但是当你想要创建需要的版本的rails项目是怎么办呢？可以在自己的/home/bin
目录下创建如下脚本 myrails：

    #!/usr/bin/env ruby
    gem 'rails', '3.2.13' # 假设需要3.2.13版本
    require "rails/cli"

然后设置可执行权限

    $> chmod a+x ~/bin/myrails

然后就可以创建需要版本的rails项目了

    $> myrails new [project-name]


### Grape在Rails下的自动加载

Grape在Rails 3 下无法在开发环境下自动加载，在Rails 4 下可以自动加载
