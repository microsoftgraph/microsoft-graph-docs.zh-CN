# <a name="sovereign-cloud-deployments"></a>Sovereign 云部署


本文提供了有关 Microsoft Graph 的不同 sovereign 云实例和它们可供开发人员使用的功能信息。 


## <a name="microsoft-graph-operated-by-21vianet-in-china"></a>由中国世纪互联运营的 Microsoft Graph

本节提供了有关由世纪互联运营的 Microsoft Graph 和它们可供开发人员使用的功能信息。 

### <a name="microsoft-graph-service-root-endpoints"></a>Microsoft Graph 服务根终结点
| 由世纪互联运营的 Microsoft Graph | Microsoft Graph|
|---------------------------|----------------|
| https://microsoftgraph.chinacloudapi.cn | https://graph.microsoft.com|

### <a name="microsoft-graph-explorer"></a>Microsoft Graph 资源管理器
| Microsoft Graph 资源管理器（中国） | Microsoft Graph 资源管理器|
|---------------------------|----------------|
|https://developer.microsoft.com/zh-cn/graph/graph-explorer-china| https://developer.microsoft.com/graph/graph-explorer|

### <a name="azure-openid-connect-and-oauth20"></a>Azure OpenID Connect 和 OAuth 2.0
用于获取登录令牌或调用由世纪互联运营的 Microsoft Graph 的终结点与其他产品的终结点不同。 

| 由世纪互联运营的 Microsoft Graph | Microsoft Graph|
|---------------------------|----------------|
| https://login.chinacloudapi.cn | https://login.microsoftonline.com|
 
使用 https://login.chinacloudapi.cn/common/oauth2/authorize 对用户进行身份验证，并使用 https://login.chinacloudapi.cn/common/oauth2/token 为您的应用获取用于调用由世纪互联运营的 Microsoft Graph 的令牌。

> **注意：**最新的 [v2.0 授权和令牌终结点](https://azure.microsoft.com/en-us/documentation/articles/active-directory-appmodel-v2-overview/)不可用于由世纪互联运营的 Microsoft Graph。 

>应用只能通过 **https://microsoftgraph.chinacloudapi.cn** 终结点访问组织数据，而不能访问消费者数据。应用应使用 **https://graph.microsoft.com** 终结点来访问消费者数据。

### <a name="service-capabilities-offered-by-microsoft-graph-operated-by-21vianet"></a>由世纪互联运营的 Microsoft Graph 提供的服务功能
以下 Microsoft Graph 功能已全面推出（在 `/v1.0` 终结点上）：

* 用户
* 组
* 文件
* 邮件
* 日历
* 个人联系人 
* 创建、读取、更新和删除 (CRUD) 操作
* 跨域资源共享 (CORS) 支持。

预览版中也提供以下 Microsoft Graph 功能（在 `/beta` 终结点上）：

* 组织联系人
* 应用程序
* 服务主体
* 目录架构扩展
* Webhooks
