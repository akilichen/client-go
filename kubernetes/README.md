## 列表用处
- 提供 ClientSet 客户端。

## 功能
ClientSet 客户端在 RESTClient 的基础上封装了对资源和版本的管理方法。每个资源可以理解为一个客户端，而 ClientSet 则是多个客户端的集合，每一个资源和版本都以函数的方式暴露给开发者。

具体使用方法，可参考官方示例：https://link.zhihu.com/?target=https%3A//github.com/kubernetes/client-go/tree/master/examples/create-update-delete-deployment
