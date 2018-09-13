# <a name="use-the-microsoft-graph-security-api"></a>使用 Microsoft Graph Security API

Microsoft Graph 安全 API 提供统一的接口和架构，与来自 Microsoft 和生态系统合作伙伴的安全解决方案集成。 这使客户能够简化安全性操作和更好地防御增加网络威胁。 Microsoft Graph Security API 可以作为联合的安全聚合服务，用于向所有登记的安全提供程序提交查询以获取聚合响应。 使用 Microsoft Graph Security API 来构建应用程序，从而：

- 合并和关联多个来源的安全警告
- 解除上下文数据锁定来告知调查
- 自动化安全操作以提高效率
- 提供安全数据的可见性，以启用主动风险管理

Microsoft Graph Security API 包括以下主要实体。

## <a name="alerts"></a>警报

警报是客户租户内的潜在安全问题，Microsoft 或合作伙伴安全解决方案已经确定并标记需要操作或通知的安全问题。 借助 Microsoft Graph Security [alerts](alert.md) 实体，您可以统一并简化跨所有集成解决方案的安全问题。 这还允许应用程序关联警报和上下文，从而改进威胁保护和响应。 通过缩短调查时间和解决事件的时间，这可解锁安全运营效率。 使用警报更新功能，可以通过更新 alerts 实体，跨 Microsoft Graph Security API 集成的不同安全产品和服务同步特定警报的状态。 [ ](alert.md)

Microsoft Graph Security 集成解决方案将收到来自下列安全提供程序的警报：

- Azure 安全中心
- Azure Active Directory 标识保护
- Azure 信息保护
- Microsoft 云应用程序安全性
- Windows Defender 高级威胁防护
- Microsoft Intune（个人预览版）
- Office 365（即将推出）
- 合作伙伴解决方案，如 Palo Alto Networks 应用框架

> **注意：** 新的提供程序正加入 Microsoft Graph Security 生态系统。

## <a name="common-use-cases"></a>常见用例

下面是一些有关使用 Microsoft Graph Security API 的最常用请求：

| **用例**   | **REST 资源** | **在 Graph 浏览器中试用** |
|:---------------|:--------|:----------|
| 列出警报 | [列出警报](../api/alert_list.md) | [https://graph.microsoft.com/v1.0/security/alerts](https://developer.microsoft.com/en-us/graph/graph-explorer?request=security/alerts&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com) |
| 更新通知 | [更新警报](../api/alert_update.md) | [https://graph.microsoft.com/v1.0/security/alerts/{alert-id}](https://developer.microsoft.com/en-us/graph/graph-explorer?request=security/alerts/{alert-id}&method=PATCH&version=v1.0&GraphUrl=https://graph.microsoft.com) |

您可以使用 Microsoft Graph [webhooks](../../../concepts/webhooks.md) 订阅和接收有关 Microsoft Graph Security 实体的更新通知。

## <a name="resources"></a>资源

代码并参与到这些 Microsoft Graph Security API 示例：

- [ASP.NET (C#) 示例](https://github.com/microsoftgraph/aspnet-security-api-sample)
- [Python 示例](https://github.com/microsoftgraph/python-security-rest-sample)
- [Node.js (JavaScript) 示例](https://github.com/microsoftgraph/nodejs-security-sample)

参与社区：

- [加入技术社区](https://aka.ms/graphsecuritycommunity)
- [在 StackOverflow 上讨论](https://stackoverflow.com/questions/tagged/microsoft-graph-security)

## <a name="next-steps"></a>后续步骤

Microsoft Graph Security API 可以打开新的方式，让您可以使用来自 Microsoft 和合作伙伴的不同安全解决方案。 按照以下步骤开始：

- 向下钻取到 [通知](alert.md)。
- 尝试 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中的 API。 在**查询示例**下，选择**显示更多示例**，并将安全类别设置为**开**。
- 尝试在实体更改[订阅和接收通知](../../../concepts/webhooks.md) 。

需要更多想法？请参阅[我们的一些合作伙伴如何使用 Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners)。
