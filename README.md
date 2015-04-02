# fds-grunt

执行服务器端的grunt脚本。

## Getting Started

安装 [fd-server](https://github.com/SBFE/fd-server)

```shell
npm install fds-grunt --save-dev
```

配置服务器的 hosts 和 vhosts.

获取这个文件 "fds-grunt.node" 的线上地址.

在浏览器中访问。

## Example

假设你的项目目录是：

/User/work/project/

gruntfile.js 在这个地址：

/User/work/project/tools/gruntfile.js

node_modules 地址：

/User/work/project/tools/node_modules

在 fd-server 配置 hosts 能够访问这个目录的域名：

test.myproject.com

那么该插件安装完毕后，其线上地址为：

http://test.myproject.com/tools/node_modules/fds-grunt.node

直接在浏览器中访问该文件，相当于直接执行服务器上的 grunt 默认任务。

如果要执行独立任务，例如名为 "deploy" 的任务，修改参数即可：

http://test.myproject.com/tools/node_modules/fds-grunt.node?task=deploy

## 参数说明

#### task
Default: `''`

任务名称，为空时执行 grunt 的默认任务。

#### grunt
Default: `'../../'`

文件 fds-grunt.node 相对于 gruntfile.js 的路径。

#### timeout
Default: `10000`

设置任务超时时间。




