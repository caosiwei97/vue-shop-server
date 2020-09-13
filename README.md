# vue-shop-server
基于express+mongoose的后端服务，为前端项目vue-shop提供接口

## 安装MongoDB

如果你系统是Window，请参考[官方文档](https://docs.mongodb.com/manual/tutorial/install-mongodb-on-windows/)

如果端口被占用可以到`<install directory>\bin\mongod.cfg`下修改`network interfaces`:

```bash
net:
  port: 27018
  bindIp: 127.0.0.1
```

同时把项目根目录下的`db/models.js`里的端口换为`27018`，然后重启`mongodb`服务。

注意项目运行在本地，所以没有设置用户名和密码，如有需要可以自行参考[官方文档](https://docs.mongodb.com/manual/tutorial/change-own-password-and-custom-data/)。

## 开始

首先确保mongodb服务是否打开，然后输入以下命令打开后台服务。
```bash
net start mongodb (管理员模式)
```

安装依赖并启动项目
```
npm install
npm start
```

## 后续重构计划

将采用koa2或其他框架来重写后台服务，敬请期待。
