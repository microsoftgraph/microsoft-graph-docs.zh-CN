---
title: 在 Microsoft Graph 中处理服务通信 API
description: 可以使用 Microsoft 服务通信 API 访问Graph运行状况和消息中心帖子Microsoft 服务"。
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: 1c5690d3cb7eafa6a4914b22687993a1e145cc0a
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2021
ms.locfileid: "53109101"
---
# <a name="working-with-service-communications-api-in-microsoft-graph"></a>在 Microsoft Graph 中处理服务通信 API
服务通信 API 提供与租户订阅的 Microsoft 云服务相关的服务运行状况和消息中心帖子。 可以获取 Microsoft 服务实例的当前和历史 (，例如，Exchange Online服务关闭) 。 在致电支持人员或花时间进行故障排除之前，你可以检查服务运行状况以确定问题是否被跟踪且正在解决。 通过消息中心帖子，你可以跟踪即将进行的更改，包括新功能、更新和 (例如，Exchange Online获取新功能) 。

## <a name="authorization"></a>Authorization
Microsoft Graph允许应用程序获得对运行状况的授权访问权限，并更改有关租户订阅的 Microsoft 云服务的通信。 借助相应的委派权限或应用程序权限[](/graph/permissions-reference#service-communications-permissions)，应用可以代表登录用户或者没有租户中任何登录用户的情况下访问通信数据。 这些权限的委派和应用程序类型都仅由管理员授予。

有关访问令牌、应用注册以及委派和应用程序权限详细信息，请参阅身份验证 [和授权基础知识](/graph/auth/auth-concepts)。

### <a name="access-service-communications-api-on-behalf-of-signed-in-user"></a>代表登录用户访问服务通信 API

代表登录用户访问服务通信 API 需要委派权限。 面向客户的画布应用程序（如 [Microsoft 365 管理中心](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/homepage) (仅可供管理员角色) 访问）可以代表登录用户调用服务通信 API，获取登录用户租户的服务运行状况和服务通知 _数据。_ 用户可以查明其订阅的订阅服务器是否正常或是否有问题。 他们还可以了解影响租户的任何当前服务问题。 

### <a name="access-service-communications-api-without-user"></a>无需用户即可访问服务通信 API

在没有登录用户的情况下访问服务通信 API 需要应用程序权限。 作为后端服务（如监控或警报服务）运行的应用程序可以使用自己的标识（而不是代表用户）调用服务通信 API。 这些后端服务可以构建自定义监视/警报管道并调用服务通信 API，获取服务运行状况和服务通知数据。 


## <a name="common-use-cases-and-required-permissions"></a>常见用例和所需权限

|用例|API 请求| 所需权限| 支持的权限类型|
|:--------|:--------|:--------|:--------|
| 列出租户的运行状况概述 | [列出 healthOverviews](/graph/api/serviceannouncement-list-healthoverviews?view=graph-rest-beta&preserve-view=true) | _ServiceHealth.Read.All_ | 委托和应用程序 | 
| 获取租户的特定服务运行状况信息 | [获取 serviceHealth](/graph/api/servicehealth-get?view=graph-rest-beta&preserve-view=true) | _ServiceHealth.Read.All_ | 委托和应用程序 |
| 列出租户的所有服务问题 | [列出问题](/graph/api/serviceannouncement-list-issues?view=graph-rest-beta&preserve-view=true) | _ServiceHealth.Read.All_ | 委托和应用程序 |
| 获取租户的特定服务问题 | [获取问题](/graph/api/servicehealthissue-get?view=graph-rest-beta&preserve-view=true) | _ServiceHealth.Read.All_ | 委托和应用程序 |
| 获取租户的事件后审阅报告 | [获取事件报告](/graph/api/servicehealthissue-incidentreport?view=graph-rest-beta&preserve-view=true)| _ServiceHealth.Read.All_ | 委托和应用程序 |
| 列出租户的所有服务消息 | [列出邮件](/graph/api/serviceannouncement-list-messages?view=graph-rest-beta&preserve-view=true) | _ServiceMessage.Read.All_ | 委托和应用程序 |
| 获取租户的特定服务消息 | [获取邮件](/graph/api/serviceupdatemessage-get?view=graph-rest-beta&preserve-view=true) | _ServiceMessage.Read.All_ | 委托和应用程序 |
| 更新已登录用户的服务消息状态 | 有关状态操作的列表，请参阅 [serviceUpdateMessage](/graph/api/resources/serviceupdatemessage?view=graph-rest-beta&preserve-view=true)。| _ServiceMessageViewpoint.Write_ | 委派 |

## <a name="whats-new"></a>最近更新
了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。

## <a name="next-steps"></a>后续步骤

服务通信 API 可以开启与用户互动的新方式：

- [访问 Microsoft 服务中的服务运行状况和通信Graph](/graph/service-communications-concept-overview)
- 请尝试 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中的 API。

需要更多灵感？请参阅[我们的一些合作伙伴如何使用 Microsoft Graph](https://developer.microsoft.com/en-us/graph/partners)。