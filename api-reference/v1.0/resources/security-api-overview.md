# <a name="use-the-microsoft-graph-security-api"></a>使用 Microsoft Graph 安全 API

Microsoft Graph 安全 API 提供统一的接口和集成使用经 Microsoft 和生态系统的合作伙伴的安全解决方案的架构。 这使客户能够简化安全性操作和更好地防御增加网络威胁。 Microsoft Graph 安全 API 可以作为联盟的安全聚合服务，用于向所有 onboarded 安全提供程序获取聚合的响应提交查询。 使用 Microsoft Graph 安全 API 来构建应用程序的：

- 合并和关联多个来源的安全警告
- 解除锁定上下文数据来告知调查
- 自动化安全操作以提高效率
- 提供的可见性安全数据，以启用主动风险管理

Microsoft Graph 安全 API 包括以下主要实体。

## <a name="alerts"></a>警报

通知是潜在客户的租户的 Microsoft 或合作伙伴的安全解决方案已经确定并标记的操作或通知中的安全问题。 与 Microsoft Graph 安全[警报](alert.md)实体，您可以统一并简化跨所有集成的解决方案的安全问题。 这还允许应用程序关联的通知和上下文改进威胁保护和响应。 通过减少调查时间和时间的事件的分辨率，这些解锁安全运营效率。 使用通知更新功能中，可以跨不同安全产品和服务与 Microsoft Graph 安全 API 通过更新[通知](alert.md)实体集成同步特定警报的状态。

Microsoft Graph 安全集成解决方案将收到来自下列安全提供程序的通知：

- Azure 安全中心
- Azure Active Directory 标识保护
- Azure 信息保护
- Microsoft 云应用程序安全性
- Windows Defender 高级威胁保护
- Microsoft Intune （专用预览）
- Office 365 （即将推出）
- （即将推出） azure 高级威胁保护
- 合作伙伴解决方案，如帕洛阿尔托市网络应用程序框架

> **注意：** 新的提供程序持续是加入到 Microsoft Graph Security 生态系统。

## <a name="common-use-cases"></a>常见用例

下面是一些有关使用 Microsoft Graph 安全 API 的最常用请求：

| **用例**   | **REST 资源** | **尝试在图资源管理器** |
|:---------------|:--------|:----------|
| 列出警报 | [列出警报](../api/alert_list.md) | [https://graph.microsoft.com/v1.0/security/alerts](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com) |
| 更新通知 | [更新警报](../api/alert_update.md) | [https://graph.microsoft.com/v1.0/security/alerts/{alert-id}](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts/{alert-id}&method=PATCH&version=v1.0&GraphUrl=https://graph.microsoft.com) |

您可以使用 Microsoft Graph [webhooks](../../../concepts/webhooks.md)订阅和接收有关 Microsoft Graph Security 实体更新通知。

## <a name="resources"></a>Resources

代码并参与到这些 Microsoft Graph 安全 API 示例：

- [ASP.NET (C#) 示例](https://github.com/microsoftgraph/aspnet-security-api-sample)
- [Python 示例](https://github.com/microsoftgraph/python-security-rest-sample)
- [Node.js (JavaScript) 示例](https://github.com/microsoftgraph/nodejs-security-sample)

社区的使用：

- [加入技术社区](https://aka.ms/graphsecuritycommunity)
- [讨论在 StackOverflow 上](https://stackoverflow.com/questions/tagged/microsoft-graph-security)

## <a name="next-steps"></a>后续步骤

您可以使用不同的安全解决方案来自 Microsoft 和合作伙伴进行新的方法可以打开 Microsoft Graph 安全 API。 按照以下步骤开始：

- 向下钻取到[通知](alert.md)。
- 尝试 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中的 API。 下**的示例查询**，选择**显示更多示例**，并设置为**上**的安全类别。
- 尝试在实体更改[订阅和接收通知](../../../concepts/webhooks.md)。

需要更多灵感？请参阅[我们的一些合作伙伴如何使用 Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners)。
