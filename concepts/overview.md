# <a name="overview-of-microsoft-graph"></a>Microsoft Graph 概述

可以使用 Microsoft Graph API 在 Microsoft 云中与数百万用户的数据交互。使用 Microsoft Graph 为组织和消费者生成应用，此类应用与所有这些资源、关系以及情报通过单个终结点相连接：`https://graph.microsoft.com`。

## <a name="whats-in-the-graph"></a>Graph 有哪些功能？

Microsoft Graph 由各种资源组成，这些资源通过关系相连接。例如，用户可通过 [memberOf](../api-reference/v1.0/api/user_list_memberof.md) 关系连接到某个组，也可以通过 [manager](../api-reference/v1.0/api/user_list_manager.md) 关系连接到其他用户。你的应用可以遍历这些关系来访问这些连接的资源，并通过 API 对其执行操作。

还可以从 Microsoft Graph 中获取与数据相关的有价值的见解和情报。例如，你可以获得特定用户[常用的](../api-reference/beta/resources/insights_trending.md)文件，或者获取与用户最为相关的[人员](../api-reference/beta/api/user_list_people.md)。

在 Microsoft Graph 中发现关系的可能性。

![显示作为 Graph 一部分的主要资源和关系的图片](images/microsoft_graph.png)

## <a name="what-can-you-do-with-microsoft-graph"></a>可以使用 Microsoft Graph 执行哪些操作？ 

可以使用 Microsoft Graph 为用户构建独特的周围环境体验，帮助他们提高工作效率。假设一个应用可以...

- 查看下一次会议，并可通过提供与会者的个人资料信息帮助你准备会议，包括他们的职务、工作伙伴以及最近处理的文档和项目信息。
- 扫描你的日历，并为下一次团队会议提出最佳时间建议。
- 从 OneDrive 中的 Excel 文件获取最新销售预测图表，让你可以实时更新趋势预测，这一切通过手机就可以实现。
- 订阅日历更改、当你在会议中花费太长时间发出警报，还可以根据与会者和你的相关性，为可能错过或委托的会议提供建议。
- 帮助你整理手机上的个人和工作信息；例如，对应当归到个人 OneDrive 的照片和应当归到 OneDrive for Business 的业务收据进行分类。

使用 Microsoft Graph API，你可以实现这些功能及其他更多功能。

## <a name="next-steps"></a>后续步骤

- 查看某些[精选方案](../concepts/featured_scenarios.md)。
- 请尝试 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中的示例请求。
- 使用[快速入门](https://developer.microsoft.com/graph/quick-start)设置准备运行的示例应用。
- 了解如何在你的应用中[获取身份验证令牌](../concepts/auth_overview.md)。
- 开始[使用 API](../concepts/use_the_api.md)。

## <a name="feedback"></a>有反馈？

我们非常重视你的反馈意见。请在 [Stack Overflow](http://stackoverflow.com/questions/tagged/office365+or+microsoftgraph) 上与我们联系。使用 [MicrosoftGraph] 标记出你的问题。

