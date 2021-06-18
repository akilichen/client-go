## 列表用处
- 提供 DynamicClient 动态客户端。

### 具体
- DynamicClient 是一种动态客户端，它可以动态的指定资源的组，版本和资源。因此它可以对任意 K8S 资源进行 RESTful 操作，包括 CRD 自定义资源。它封装了 RESTClient。所以同样提供 RESTClient 的各种方法。

- 具体使用方法，可参考官方示例，dynamic-create-update-delete-deployment => https://link.zhihu.com/?target=https%3A//github.com/kubernetes/client-go/tree/master/examples/dynamic-create-update-delete-deployment。

- 注意: 该官方示例是基于集群外的环境，如果你需要在集群内部使用（例如你需要在 container 中访问），你将需要调用 rest.InClusterConfig() 生成一个 configuration。具体的示例请参考 in-cluster-client-configuration => https://link.zhihu.com/?target=https%3A//github.com/kubernetes/client-go/tree/master/examples/in-cluster-client-configuration。
