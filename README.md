# go-restful
- 基于 [go-gin](https://github.com/gin-gonic/gin) 的 json restful 风格的golang基础库

1、 目录结构说明

- ./service/config/MyIni.go 中添加新的配置项
- ./service/router/router.go 中添加路由及回调处理函数
- ./service/view 中添加逻辑代码


2、api接口说明

### 支持3种接口模式

- 1.  func(*gin.Context) //gogin 原始接口
- 2. func(*api.Context) //自定义的context类型
- 3. func(*api.Context,req) //自定义的context类型,带request 请求参数
     func(*gin.Context,*req)
     ...... 等接口模式

