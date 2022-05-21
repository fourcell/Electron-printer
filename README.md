# 热敏打印dome
使用 `print` 插件实现将 `ESCPOT` 指令转为打印驱动的程序

## 依赖安装&&启动
```
yanr || cnpm install      //依赖安装
yarn start || npm run start //项目启动
```

## 开发环境 

### 打印配置
在开发前，请确定保证本地开发电脑已经装好打印驱动并可以打印（只需能将打印驱动程序能发送到打印机即可）
### 开发环境
`print` 插件是使用 c 和 Python 开发完成的，在本地开发请确保本地安装好 Python 2.7 版本。
且 `print`插件需要转换才能在`electron`中使用，所以 print的包在`node_modules`中上传到github

## 桌面应用和页面间的通信
本项目是使用 `websocket` 实现页面和桌面应用的通信，electron 为服务端接受 网页客户端的信息，在客户端对
`websocket` 进行封装应用，页面或数据转为 `ESCPOT` 可以使用第三方插件实现，也可参考官方 `ESCPOT`

## 参考文档
[https://juejin.cn/post/6844903778827649032#heading-0] 如果实现一个桌面应用打印程序
[https://github.com/theturtle32/WebSocket-Node] webSocket 插件
[https://wenku.baidu.com/view/78fffaf32a4ac850ad02de80d4d8d15abe2300da.html] ESCPOT 打印指令
[https://www.kancloud.cn/qnit/web_front/800193] canvas 打印处理
