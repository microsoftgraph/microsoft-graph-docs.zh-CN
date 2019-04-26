---
title: Microsoft Graph 概述
description: Microsoft Graph 是 Microsoft 365 中数据和智能的网关。 Microsoft Graph 提供了统一的可编程性模型，通过该模型可利用 Office 365、企业移动性 + 安全性和 Windows 10 中的大量数据。
author: jthake-msft
localization_priority: Priority
ms.openlocfilehash: b8256cebe9e8e706a655221c3e1acc5947f9eecd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32558006"
---
# <a name="overview-of-microsoft-graph"></a>Microsoft Graph 概述

Microsoft Graph 是 Microsoft 365 中数据和智能的网关。 Microsoft Graph 提供了统一的可编程性模型，通过该模型可利用 Office 365、企业移动性 + 安全性和 Windows 10 中的大量数据。 

Microsoft Graph API 可用于为组织和消费者生成应用，与数百万用户的数据进行交互。 使用 Microsoft Graph，可以与丰富的资源、关系和智能相连接，所有这些均通过单个终结点实现：`https://graph.microsoft.com`。

## <a name="whats-in-the-graph"></a>Graph 中有什么？
Microsoft Graph 公开了 REST API 和客户端库，用于访问以下数据：

- Azure Active Directory
- Office 365 服务：SharePoint、OneDrive、Outlook/Exchange、Microsoft Teams、OneNote、Planner 和 Excel
- 企业移动性和安全性服务：Identity Manager、Intune、高级威胁分析和高级威胁防护。
- Windows 10 服务：活动和设备
- 教育

要了解更多内容，请参阅 [Microsoft Graph 中的主要服务和功能](overview-major-services.md)。

Microsoft Graph 通过关系连接这些服务中的所有资源。 例如，用户可通过 [memberOf](/graph/api/user-list-memberof?view=graph-rest-1.0) 关系连接到某个组，也可以通过 [manager](/graph/api/user-list-manager?view=graph-rest-1.0) 关系连接到其他用户。 你的应用可以遍历这些关系来访问这些连接的资源，并通过 API 对其执行操作。

此外，你还可以从 Microsoft Graph 中获取与数据相关的有价值的见解和情报。 例如，你可以获得特定用户的[常用](/graph/api/resources/insights-trending?view=graph-rest-beta)文件，或者获取与用户相关度最高的[人员](/graph/api/user-list-people?view=graph-rest-beta)。

在 Microsoft Graph 中发现关系的可能性。

![显示作为 Graph 一部分的主要资源和关系的图片](images/microsoft-graph.png)

## <a name="what-can-you-do-with-microsoft-graph"></a>可以使用 Microsoft Graph 执行哪些操作？ 

可以使用 Microsoft Graph 为用户构建独特的周围环境体验，帮助他们提高工作效率。想象一下，一个应用可以...

- 查看你的下一次会议，并通过提供与会者的个人资料信息帮助你准备会议，包括他们的职务、工作伙伴以及关于最近处理的文档和项目的信息。
- 扫描你的日历，并为下一次团队会议提出最佳时间建议。
- 从 OneDrive 中的 Excel 文件获取最新销售预测图表，让你可以实时更新趋势预测，这一切通过手机就可以实现。
- 订阅日历更改、当你在会议上花费太长时间时发出警报，还可以根据与会者和你的相关度，为可能错过或委派的会议提供建议。
- 帮助你整理手机上的个人和工作信息；例如，对应当归到个人 OneDrive 的照片和应当归到 OneDrive for Business 的业务收据进行分类。

使用 Microsoft Graph API，你可以实现这些功能及其他更多功能。

>**注意：** 使用 Microsoft Graph API 时，表示你同意 [Microsoft Graph 使用条款](https://developer.microsoft.com/graph/docs/misc/terms-of-use)和 [Microsoft 隐私声明](https://go.microsoft.com/fwlink/?LinkId=521839)。

### <a name="popular-requests"></a>常见请求

查看可与 Microsoft Graph API 结合使用的某些常见方案。 这些链接可带你前往 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)。

| **操作** | **URL** |
|:--------------------------|:----------------------------------------|
|   获取我的个人资料 |    [`https://graph.microsoft.com/v1.0/me`](https://developer.microsoft.com/graph/graph-explorer/?request=me&version=v1.0) |
|   获取我的文件 | [`https://graph.microsoft.com/v1.0/me/drive/root/children`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fdrive%2Froot%2Fchildren&version=v1.0) |
|   获取我的照片	 | [`https://graph.microsoft.com/v1.0/me/photo/$value`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fphoto%2F%24value&version=v1.0) |
|   获取我的邮件 |   [`https://graph.microsoft.com/v1.0/me/messages`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fmessages&version=v1.0) |
|   获取我的高重要性的邮件 | [`https://graph.microsoft.com/v1.0/me/messages?$filter=importance%20eq%20'high'`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fmessages%3F%24filter%3Dimportance%2520eq%2520'high'&version=v1.0) |
|   获取我的日历事件 |    [`https://graph.microsoft.com/v1.0/me/events`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fevents&version=v1.0) |
|   获取我的经理  | [`https://graph.microsoft.com/v1.0/me/manager`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fmanager&version=v1.0) |
|   获取上一个修改文件 foo.txt 的用户 |  [`https://graph.microsoft.com/v1.0/me/drive/root/children/foo.txt/lastModifiedByUser`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fdrive%2Froot%2Fchildren%2Ffoo.txt%2FlastModifiedByUser&version=v1.0) |
|   获取我所属的 Office365 组| [`https://graph.microsoft.com/v1.0/me/memberOf/$/microsoft.graph.group?$filter=groupTypes/any(a:a%20eq%20'unified')`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2FmemberOf%2F%24%2Fmicrosoft.graph.group%3F%24filter%3DgroupTypes%2Fany(a%3Aa%2520eq%2520'unified')&version=v1.0) |
|   获取我组织中的用户     | [`https://graph.microsoft.com/v1.0/users`](https://developer.microsoft.com/graph/graph-explorer/?request=users&version=v1.0) |
|   获取我组织中的组 | [`https://graph.microsoft.com/v1.0/groups`](https://developer.microsoft.com/graph/graph-explorer/?request=groups&version=v1.0) |
|   获取与我相关的人员    | [`https://graph.microsoft.com/v1.0/me/people`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fpeople&version=beta)  |
|   获取我常用的项目 |  [`https://graph.microsoft.com/beta/me/insights/trending`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Finsights%2Ftrending&version=beta) |
|   获取我的笔记 |  [`https://graph.microsoft.com/v1.0/me/onenote/notebooks`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fonenote%2Fnotebooks&version=beta) |

## <a name="access-microsoft-graph-at-scale"></a>批量访问 Microsoft Graph


Microsoft Graph 数据连接提供了对 Office 365 数据的批量访问权限，而不是传统的事务访问权限。 借助批量 Office 365 数据，可使用 Azure 工具生成具有以下功能的智能应用：

- 为你在组织中查找与某主题最相关的专家 
- 自动执行知识库创建
- 分析会议请求，以提供会议室利用率方面的见解
- 检测生产力和通信数据欺诈

## <a name="when-should-i-use-microsoft-graph-data-connect"></a>我应何时使用 Microsoft Graph 数据连接？

使用 Microsoft Graph 数据连接，可以一种新方式与通过 Microsoft Graph API 公开的数据进行交互。 除了提供对 Office 365 数据的可缩放访问权限以外，Microsoft Graph 数据连接还提供一组独特功能，用于简化智能应用的生成过程，所有这些都是在 Microsoft 云中完成。

|**功能**| **Microsoft Graph API** | **Microsoft Graph 数据连接** |
|:----------|:------------------------|:--------------------------------------|
| **访问范围** | 单个用户或整个租户 | 多个用户或组 |
| **访问模式** | 实时 | 定期重复 |
| **数据操作** | 对主数据执行操作 | 对数据缓存执行操作 |
| **数据保护** | 保护 Microsoft 365 中的数据 | 数据保护延伸至 Azure 订阅中的数据缓存 |
| **用户同意** | 自我<br>资源类型 | 无 |
| **管理员同意** | 整个组织<br>资源类型 | 选择用户组<br>资源类型和属性<br>排除用户 |
| **访问工具** | RESTful Web 查询 | Azure 数据工厂 |

若要详细了解 Microsoft Graph 数据连接，请参阅 [Microsoft Graph 数据连接](data-connect-overview.md)。 首先，请参阅 [Microsoft Graph 数据连接概述](data-connect-concept-overview.md)。 

## <a name="next-steps"></a>后续步骤

- 查看某些[精选应用场景](https://developer.microsoft.com/graph/examples)。
- 尝试 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中的示例请求。
- 使用[快速入门](https://developer.microsoft.com/graph/quick-start)设置即可运行的示例应用。
- 在目录的**了解**下，阅读有关你可在应用场景中使用的服务和功能。 
- 了解如何在你的应用中[获取身份验证令牌](auth-overview.md)。
- 开始[使用 API](use-the-api.md)。


