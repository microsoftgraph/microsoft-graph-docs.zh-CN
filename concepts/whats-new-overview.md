---
title: Microsoft Graph 新增功能
description: Microsoft Graph 新增功能
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 403466a154e279b9a41f0f513f80ff77db299884
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681618"
---
# <a name="whats-new-in-microsoft-graph"></a>Microsoft Graph 新增功能

查看 Microsoft Graph 中的新增功能要点，并查看你可如何[分享你的想法](#want-to-stay-in-the-loop)。 有关 API 更新的完整列表，请参阅 API 更改日志的和[六月和六月份](changelog.md#june-2020)[部分。](changelog.md#may-2020) 

> [!IMPORTANT]
> _预览_状态下的功能（包括 API 和工具）可能会发生更改，恕不另行通知，有些功能可能永远不会提升为正式发布 (GA) 状态。 不要在成品应用中使用预览功能。


## <a name="june-2020-new-and-generally-available"></a>2020年6月：新的和普遍可用的

### <a name="cloud-communications--online-meeting"></a>云通信 | 联机会议
- `Accept-Language`[创建联机会议](/graph/api/application-post-onlinemeetings?view=graph-rest-1.0)时使用 HTTP 标头，以提供基于区域设置的联接信息。
- 使用[createOrGet](/graph/api/onlinemeeting-createorget?view=graph-rest-1.0)返回具有指定的**externalId**值的联机会议; 或者，如果尚不存在，则创建一个，以便简化在第三方日历中嵌入结果会议。


## <a name="june-2020-new-in-preview-only"></a>2020年6月：仅预览中的新内容
### <a name="cloud-communications--presence"></a>云通信 |Shell
[获取](/graph/api/presence-get?view=graph-rest-beta)组织中的所有用户或组织中的特定用户的状态。


## <a name="may-2020-new-and-generally-available"></a>5月2020：新的和普遍可用的

### <a name="calendar--place"></a>日历 | 位置
在 v1.0 中的[位置 API](/graph/api/resources/place) GA-在生产应用程序中使用此 api 来获取、更新或删除租户中的[会议室](/graph/api/resources/room)或[会议室列表](/graph/api/resources/roomlist)。 了解有关位置 API 的[详细](outlook-calendar-concept-overview.md#build-apps-with-location-awareness-and-provide-intelligent-context)信息。

### <a name="change-notifications"></a>更改通知
- 在 Microsoft 云中的美国政府版中订阅更改通知。

### <a name="cloud-communications--call-records"></a>云通信 | 通话记录
- 公开的[呼叫记录 API](/graph/api/resources/callrecords-api-overview?view=graph-rest-1.0) -使用[CallRecord](/graph/api/resources/callrecord?view=graph-rest-1.0)资源在 Microsoft 团队和 Skype 中获取呼叫和联机会议的元数据。
- 订阅[更改通知](/graph/webhooks)，以获取组织中所有**callRecord**资源的更改通知。
- [列出](/graph/api/callrecords-session-list?view=graph-rest-1.0) **callRecord**中的会话，并根据需要[展开每个会话以](/graph/api/callrecords-session-list?view=graph-rest-1.0#example-2-get-session-list-with-segments)在呼叫记录中列出分段。
- 对 `frequency60GHz` 网段中媒体终结点的 60-GHz （）和 `unknownFutureValue` WiFi 频带值的支持。
- 在通信[段](/graph/api/resources/callrecords-segment)中支持语音邮件作为服务端的一种可能类型的终结点。

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理
Intune[可能会](changelog.md#may-2020)在 v1.0 中更新。

### <a name="graph-explorer"></a>Graph 浏览器
使用[Graph 浏览器](https://developer.microsoft.com/en-us/graph/graph-explorer)的许多新功能，以增强沙盒中的学习和原型。 例如：
- 查看与您输入的 REST API 查询相对应的代码段，以 c #、Java、JavaScript 和客观 C 为依据。
- 使用租户登录，查看并将访问令牌复制到您喜爱的 REST 客户端应用程序。

有关更多详细信息，请参阅[新的 Graph 浏览器现已公开](https://developer.microsoft.com/graph/blogs/new-graph-explorer-is-now-ga/)。

### <a name="groups"></a>组
- 通过 Azure AD Connect 将本地目录同步到 Azure Active Directory 现在，将 **、onpremisesdomainname**、 **onPremisesNetBiosName**和**onPremisesSamAccountName**属性作为[组](/graph/api/resources/group?view=graph-rest-1.0)资源的一部分返回。
- 订阅由世纪互联运营的 Microsoft 云中国[组](/graph/api/resources/group)资源的更改通知。

### <a name="identity-and-access"></a>身份和访问
- 在 v1.0 中使用服务主体 API （GA）-使用生产应用程序中的[servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-1.0)资源以编程方式管理应用程序的实例，并控制应用程序可在租户中执行的操作。 您可以控制哪些用户可以使用应用程序，应用程序有权访问哪些资源，如添加密码凭据、即将过期的证书以及管理委派的权限授予和应用程序角色分配。
- 公开的[appRoleAssignment](/graph/api/resources/appRoleAssignment?view=graph-rest-1.0) API，用于记录[appRole](/graph/api/resources/approle?view=graph-rest-1.0) `roles` 对[用户](/graph/api/resources/user?view=graph-rest-1.0)、[组](/graph/api/resources/group?view=graph-rest-1.0)或[servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-1.0)的 appRole 分配（表示 ID 令牌和访问令牌中的声明）。
- 在 Azure Active Directory 上使用 Facebook 作为标识提供程序。
- 使用的委派或应用程序权限 `AppRoleAssignment.ReadWrite.All` 允许应用管理对任何 API （包括 Microsoft Graph）的应用程序权限和任何应用程序的应用程序分配的授予，分别与或不带登录用户。


### <a name="microsoft-graph-sdks"></a>Microsoft Graph SDK
有关以下内容，请参阅新的 SDK 指导：
- [分页](/graph/sdks/paging)
- [批处理](/graph/sdks/batch-requests)
- [在 OneDrive 上上传大文件](/graph/sdks/large-file-upload)
- [通过 HTTP 中间件组件自定义 SDK 服务客户端](/graph/sdks/customize-client)。

### <a name="teamwork"></a>团队合作
- 如果您的方案涉及团队中的联机会议，请参阅有关如何在[日历 API](outlook-calendar-online-meetings.md)和[云通信 API](cloud-communications-online-meetings.md)中进行[选择](choose-online-meeting-api.md)以创建和加入联机会议的新指导。
- [发送](/graph/api/channel-post-messages?view=graph-rest-1.0)和[回复](/graph/api/channel-post-messagereply?view=graph-rest-1.0)[频道](/graph/api/resources/channel?view=graph-rest-1.0)中的邮件。
- 通过使用**fileFolder**导航属性，获取[频道](/graph/api/resources/channel?view=graph-rest-1.0)的文件的 OneDrive for business 位置。

### <a name="teamwork--shifts"></a>团队合作 | 倒班
V1.0 中的[倒班 API](/graph/api/resources/shift?view=graph-rest-1.0) GA-在生产应用程序中使用此 api 创建、更新和管理 firstline 工作人员的日程安排，以让他们保持联系并有效地进行协作。

### <a name="users"></a>用户
- 订阅由世纪互联运营的 Microsoft 云中国[用户](/graph/api/resources/user)资源的更改通知。
- 使用**用户**资源的**externalUserState**和**externalUserStateChangeDateTime**属性跟踪已被[邀请](/graph/api/invitation-post?view=graph-rest-1.0)加入组织的外部用户的上次状态更改的状态和日期/时间。

## <a name="may-2020-new-in-preview-only"></a>5月2020：仅预览中的新内容

### <a name="change-notifications"></a>更改通知
- 使用正式的架构化类型[changeNotification](/graph/api/resources/changenotification?view=graph-rest-beta)和[changeNotificationCollection](/graph/api/resources/changenotificationcollection?view=graph-rest-beta)处理资源更改通知。 
- 跟踪是否按顺序通知，或者是否在使用**changeNotification**资源上的**sequenceNumber**属性丢失通知。

### <a name="devices-and-apps--cloud-printing"></a>设备和应用 | 云打印
- [打印机](/graph/api/resources/printer?view=graph-rest-beta)和[printerShare](/graph/api/resources/printershare?view=graph-rest-beta)资源现在处于奇偶校验，并且彼此具有相同的属性。
- 打印机共享的一些属性和类型名称清理：
  - 使用 "[打印](/graph/api/resources/print?view=graph-rest-beta)" 的**共享**导航属性获取在租户中注册的打印机共享的列表。 
  - 请参阅[可能](changelog.md#may-2020)更改日志中的详细信息。

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理
Intune[可能会](changelog.md#may-2020)在 beta 中更新。

### <a name="groups"></a>组
- 使用[组](/graph/api/resources/group?view=graph-rest-beta)的现有规则或指定的规则[评估](/graph/api/group-evaluatedynamicmembership?view=graph-rest-beta)用户或设备是否为动态组的成员。 [基于规则的动态成员身份](/azure/active-directory/users-groups-roles/groups-dynamic-membership)可降低添加和删除成员的管理开销。
- 创建 Office 365[组](/graph/api/resources/group?view=graph-rest-beta)时，通过在**resourceBehaviorOptions**属性中指定组的行为来配置这些行为。 例如，允许成员张贴、订阅新成员到对话、禁用欢迎电子邮件以及在 Outlook 体验中隐藏组。
- 指定要在**resourceProvisioningOptions**属性中设置的资源，这些资源通常不是默认[组](/graph/api/resources/group?view=graph-rest-beta)创建的一部分。 目前支持将组设置为具有 Microsoft 团队功能的[团队](/graph/api/resources/team?view=graph-rest-beta)。

### <a name="identity-and-access"></a>身份和访问
- `$count` `$filter` `$search` 在获取派生自[directoryObject]()的实体的集合时应用 OData 系统查询选项（，，）。 您可以在这些实体的**displayName**和**description**属性中[搜索特定令牌](/graph/query-parameters?#using-search-on-directory-object-collections)，并使用 OData 强制转换将**directoryObject**结果修整为特定的派生类型。 有关[使用 $count、$filter、$search 和 $orderby 在 Microsoft Graph 中生成高级查询](https://developer.microsoft.com/en-us/graph/blogs/build-advanced-queries-with-count-filter-search-and-orderby/)的更多详细信息，请参阅。
- 作为[标识保护 API](/graph/api/resources/identityprotection-root?view=graph-rest-beta)的一部分，使用**riskEventType**属性来[获取检测到的风险类型](/graph/api/riskdetection-get?view=graph-rest-beta)，或[获取用户历史记录中的风险类型](/graph/api/riskyuser-list-history?view=graph-rest-beta)。 请勿使用**riskType**属性，因为它已被弃用。
- 在[条件访问策略](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta)的[条件集](/graph/api/resources/conditionalaccessconditionset?view=graph-rest-beta)的**clientAppTypes**属性中指定客户端应用程序类型。
- 使用委派的权限 `EntitlementManagement.Read.All` ，以允许应用代表登录用户读取访问包和相关的权限管理资源。
- 使用的委派或应用程序权限 `Application.Read.All` 并 `Application.ReadWrite.All` 列出组织中的[应用程序](/graph/api/application-list?view=graph-rest-beta)。
- 使用[authorizationPolicy](/graph/api/resources/authorizationpolicy?view=graph-rest-beta)资源类型控制 Azure AD 中的授权设置。

### <a name="teamwork"></a>团队合作
- [支持单一登录（SSO）](/microsoftteams/platform/tabs/how-to/authentication/auth-aad-sso)的团队应用可以 `WebApplicationInfo.id` 在[teamsAppDefinition](/graph/api/resources/teamsappdefinition?view=graph-rest-beta)的**azureADAppId**属性中指定团队应用程序清单中的。
- 使用[更](/graph/permissions-reference#teams-resource-specific-consent-permissions)精细的权限访问[团队](/graph/api/resources/team?view=graph-rest-beta)和[频道](/graph/api/resources/channel?view=graph-rest-beta)资源。




## <a name="want-to-stay-in-the-loop"></a>保持循环

我们可以通过以下方式进行参与：

- 是否有希望 Microsoft Graph 支持的方案？ 在 [Microsoft Graph 用户心声](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)中建议新功能并进行投票。
    某些新功能来源于开发人员社区的热门请求。 Microsoft Graph 团队会定期评估客户需求，并按以下顺序发布新功能：

    1. 处于**_预览_** 状态的 Debut。 任何相关的 REST API 更新都在 beta 终结点 (`https://graph.microsoft.com/beta`) 中。  

    2. 如果有足够的反馈表明具有可行性，则提升为 **_正式发布_ (GA)** 状态。 任何相关的 REST API 更新都添加到 v1.0 终结点 (`https://graph.microsoft.com/v1.0`)。 
- 成为 Microsoft Graph 社区中的活跃成员! [参与](https://aka.ms/microsoftgraphcall)Microsoft Graph 社区每月通话。
- 注册 [office 365 开发人员计划](https://developer.microsoft.com/office/dev-program)，免费订阅 Office 365, 然后开始开发! 


## <a name="see-also"></a>另请参阅
- 定期查看 [Microsoft Graph 开发人员博客](https://developer.microsoft.com/graph/blogs/), 了解发布公告和有帮助的资源。 
- 浏览 Microsoft Graph API 新增功能的详细信息, 以及[changelog](changelog.md)中的 API 行为更新。
- 查找[早期版本的重点内容](whats-new-earlier.md)。
- 了解有关 [Microsoft Graph 的版本控制、支持和中断性变更策略](versioning-and-support.md)。

