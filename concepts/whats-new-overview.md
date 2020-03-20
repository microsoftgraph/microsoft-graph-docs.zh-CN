---
title: Microsoft Graph 新增功能
description: Microsoft Graph 新增功能
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 88cb0ba1570cd0f90fe4cc199eee3ce550c17781
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42729029"
---
# <a name="whats-new-in-microsoft-graph"></a>Microsoft Graph 新增功能

查看 Microsoft Graph 中的新增功能要点，并查看你可如何[分享你的想法](#want-to-stay-in-the-loop)。 有关 API 更新的完整列表，请参阅 API 更改日志的 [3 月](changelog.md#march-2020)和 [2 月](changelog.md#february-2020)部分。 

> [!IMPORTANT]
> _预览_状态下的功能（包括 API 和工具）可能会发生更改，恕不另行通知，有些功能可能永远不会提升为正式发布 (GA) 状态。 不要在成品应用中使用预览功能。

## <a name="march-2020-new-and-generally-available"></a>2020 年 3 月：新版本和正式版

### <a name="reports"></a>报告
将 Teams 服务管理员和 Teams 通信管理员用作接受的用户角色，允许应用代表用户以[用户委派的授权的形式](reportroot-authorization.md)读取 Office 365 服务使用情况报告。 

## <a name="march-2020-new-in-preview-only"></a>2020 年 3 月：仅限预览版中的新增功能

### <a name="calendar"></a>日历
- 使用 **calendarGroupId** 属性可获取创建[日历](/graph/api/resources/calendar?view=graph-rest-beta)的[日历组](/graph/api/resources/calendargroup?view=graph-rest-beta)。
- 使用 **isDraft** 属性可将[事件](/graph/api/resources/event?view=graph-rest-beta)标识为用户已在 Outlook 中更新但尚未发送给更新与会者的会议。

### <a name="identity-and-access"></a>身份和访问
使用 [Azure 资源的 Privileged Identity Management (PIM)](/graph/api/resources/privilegedidentitymanagement-resources?view=graph-rest-beta) 的 `PrivilegedAccess.Read.AzureResources` 应用程序级别权限为管理组、订阅、资源组和资源级别的 Azure 基础结构角色设置实时访问工作流。

### <a name="teamwork"></a>团队合作
使用 `ChannelMessage.Read.All` 应用程序级别权限，在没有登录用户的情况下读取频道中的 [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta) 实例。

## <a name="february-2020-new-and-generally-available"></a>2020 年 2 月：新版本和正式版

### <a name="calendar"></a>日历
浏览“[在共享或委派日历中创建事件](outlook-create-event-in-shared-delegated-calendar.md)”示例，或浏览可用于此流程期间的代理人、受邀者和日历所有者的操作与属性。

### <a name="identity-and-access"></a>身份和访问
- 为了提升在订阅“[更改用户通知](webhooks.md)”的安全性，强制在通知流程中使用的客户端和网站服务器上[强制执行传输层安全性（TLS）1.2](https://docs.microsoft.com/configmgr/core/plan-design/security/enable-tls-1-2)或更高。 新要求自 2020 年 2 月 15 日起分阶段推出。 到 2020 年 5 月 15 日，所有通知端点必须符合新的 TLS 要求。 [找出推出阶段](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/)，如有必要，请使用新的 **latestSupportedTlsVersion** 属性作为临时解决方法，以避免订阅失败，然后再完成 TLS 升级。
- 使用相应类型的[威胁评估请求](/graph/api/resources/threatAssessmentRequest?view=graph-rest-1.0)跟踪[邮件](/graph/api/resources/mailassessmentrequest?view=graph-rest-1.0)、[电子邮件文件](/graph/api/resources/emailfileassessmentrequest?view=graph-rest-1.0)（.EML 文件）、[电子邮件附件文件](/graph/api/resources/fileassessmentrequest?view=graph-rest-1.0)（文本、Word 或二进制文件）或 [URL](/graph/api/resources/urlassessmentrequest?view=graph-rest-1.0) 中的威胁。

### <a name="users"></a>用户
[重新处理](/graph/api/user-reprocesslicenseassignment?view=graph-rest-1.0)[用户](/graph/api/resources/user?view=graph-rest-1.0)的所有基于组的许可证分配。


## <a name="february-2020-new-in-preview-only"></a>2020 年 2 月：仅限预览版中的新增功能

### <a name="calendar"></a>日历
参看“[管理日历共享和委派的预览版 API 所支持的任务](outlook-share-or-delegate-calendar.md)”。

### <a name="cloud-communications"></a>云通信

- 使用新的[通话记录](/graph/api/resources/callrecord?view=graph-rest-beta)资源，在 Microsoft Teams 和 Skype for Business 上为组织获取通话和联机会议的元数据。
- 对于会议中的参与者，请使用 **initiator** 属性获取[记录](/graph/api/resources/recordinginfo?view=graph-rest-beta)（如果有）的发起人的标识信息。

### <a name="devices-and-apps"></a>设备和应用
Intune [2 月](changelog.md#february-2020)更新。

### <a name="groups"></a>组
使用 [assignLicense](/graph/api/group-assignlicense?view=graph-rest-beta) 方法将产品（如 Office 365 或企业移动性 + 安全性）的许可证分配给组。 由于 Azure AD 可确保将许可证分配给组的成员，因此加入或离开组的成员不再需要单独级别的许可证管理。

### <a name="identity-and-access"></a>身份和访问
- 创建[访问包分配策略](/graph/api/resources/accesspackageassignmentpolicy?view=graph-rest-beta)时设置请求程序、审批和审阅设置。
- 使用 `/policies` URL 段并指定策略类型，访问[组织的特定类型的策略](/graph/api/resources/policy-overview?view=graph-rest-beta)。 例如，组织可以强制实施 Web 会话在一段时间不活动后自动从该会话注销用户的策略；请参阅 [activityBasedTimeoutPolicy](/graph/api/resources/activitybasedtimeoutpolicy?view=graph-rest-beta) 的实例的 CRUD 操作。 这是一项[重大更改](https://developer.microsoft.com/identity/blogs/breaking-changes-policy-api-microsoft-graph-beta/)，可以通过对 `/policies` 段下所有类型的策略进行分组，以便更易于发现所有策略。 采用类似的方法访问其他类型的策略：[claimsMappingPolicy](/graph/api/resources/claimsmappingpolicy?view=graph-rest-beta)、[homeRealmDiscoveryPolicy](/graph/api/resources/homerealmdiscoverypolicy?view=graph-rest-beta)、[tokenLifetimePolicy](/graph/api/resources/tokenlifetimepolicy?view=graph-rest-beta) 和 [tokenIssuancePolicy](/graph/api/resources/tokenissuancetimepolicy?view=graph-rest-beta)。 
- 使用应用程序级和委派的 `Policy.ReadWrite.ApplicationConfiguration` 权限，以读取和写入有关前一项中所述的应用程序配置[策略](/graph/api/resources/policy-overview?view=graph-rest-beta)的操作。

### <a name="teamwork"></a>团队合作
- 在组织中的所有频道消息或所有聊天消息中使用[更改通知](/graph/api/resources/webhooks?view=graph-rest-beta)。
- [拒绝](/graph/api/swapshiftschangerequest-decline?view=graph-rest-beta)与[团队](/graph/api/resources/team?view=graph-rest-beta)中的其他用户[换班的请求](/graph/api/resources/swapshiftschangerequest?view=graph-rest-beta)。

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

