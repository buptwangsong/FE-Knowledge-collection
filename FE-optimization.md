## 前端优化

> 前端是一种远程部署，运行时增量下载的GUI软件

前端应用没有安装过程，其所需程序资源都部署在远程服务器上，用户使用浏览器访问不同的页面来加载不同的资源，随着访问页面的增加，渐进式的将整个程序加载到本地，
`增量下载`是前端在工程上区别于GUI软件的根本原因。

根据`增量原则`，我们应该精心规划每个页面的资源加载策略，使得用户访问那个页面，就能按需加载该页面所需资源，没有访问的页面不加载，加载过的资源可以缓存复用，
最终带来流畅的用户体验

`增量原则`引申出的前端优化技巧几乎成为web性能优化的核心，有加载相关的*按需加载*、*延迟加载*、*预加载*、*请求合并*策略等等，有缓存相关的*浏览器缓存*、
*缓存更新*、*缓存共享*、*非覆盖式发布方案*等等。