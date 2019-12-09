---
title: Microsoft Graph 新增功能
description: Microsoft Graph 新增功能
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: ae0ec1d070a163cbb093dfabfb36edf2b034f441
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895491"
---
# <a name="whats-new-in-microsoft-graph"></a>Microsoft Graph 新增功能

查看 Microsoft Graph 中的新增功能要点，并查看你可如何[分享你的想法](#want-to-stay-in-the-loop)。 有关 API 更新的完整列表，请参阅 API 更改日志的 [12 月](changelog.md#december-2019)和 [11 月](changelog.md#november-2019)部分。 

> [!IMPORTANT]
> _预览_状态下的功能（包括 API 和工具）可能会发生更改，恕不另行通知，有些功能可能永远不会提升为正式发布 (GA) 状态。 不要在成品应用中使用预览功能。


## <a name="december-2019-new-in-preview"></a>2019年12月：预览版新增功能

### <a name="teamwork"></a>团队合作
- 针对[chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta)资源在 Microsoft 团队频道和聊天中[设置包含资源数据的更改通知](webhooks-with-resource-data.md)。
- 针对新的或已更改的[频道消息或聊天消息](/graph/api/resources/chatmessage?view=graph-rest-beta)[订阅通知](/graph/api/resources/subscription?view=graph-rest-beta)。

## <a name="november-2019-new-and-generally-available"></a>2019 年 11 月：新版本和正式版

### <a name="groups"></a>组
- 使用委派或应用程序权限GroupMember.Read.All和GroupMember.ReadWrite.Al，来列出组、读取基本组属性，读取（并更新，如有读写权限）能够访问应用程序组的成员身份。
- 使用应用程序权限Group.Create，创建不含已登录用户的组。
- 对于指定的 [组](/graph/api/resources/group?view=graph-rest-1.0)，在其它组或目录角色中[检查成员身份](/graph/api/group-checkmemberobjects?view=graph-rest-1.0)。

### <a name="identity-and-access"></a>身份和访问
- 注册通过 Azure Active Directory (Azure AD) 进行身份验证的[应用程序](/graph/api/resources/application?view=graph-rest-1.0)。 根据需要使用委派的[权限](/graph/permissions-reference#application-resource-permissions)（即 Application.Read.All 和 Application.ReadWrite.All）或应用程序权限（即 Application.Read.All）。
- 对于指定的 [设备](/graph/api/resources/device?view=graph-rest-1.0)，在其它组或目录角色中[检查成员身份](/graph/api/device-checkmemberobjects?view=graph-rest-1.0)。

### <a name="mail"></a>邮件
- 使用 **conversationIndex** 属性可获取邮件在 Outlook 电子邮件对话中的位置。
- 使用委派权限Mail.ReadBasic和应用程序权限Mail.ReadBasic.All，来获取[邮件](/graph/api/resources/message?view=graph-rest-1.0)或[邮件文件夹](/graph/api/resources/mailfolder?view=graph-rest-1.0)资源，跟踪更改，并针对邮件的更改通知管理[订阅](/graph/api/resources/subscription?view=graph-rest-1.0)。

### <a name="users"></a>用户
- 针对指定的[用户](/graph/api/resources/user?view=graph-rest-1.0)，[检查组成员身份](/graph/api/user-checkmemberobjects?view=graph-rest-1.0)。
- 使用 **creationType** 属性查找用户帐户的创建方式，例如，是将帐户创建为普通学校或工作帐户还是作为外部帐户等。

## <a name="november-2019-new-in-preview"></a>2019 年 11 月：预览版中的新增功能

### <a name="calendar"></a>日历
- [使用 Outlook 组织或参加联机会议](outlook-calendar-online-meetings.md)。
- [为](/graph/api/place-update?view=graph-rest-beta)[会议室](/graph/api/resources/room?view=graph-rest-beta)和[会议室列表](/graph/api/resources/roomlist?view=graph-rest-beta)的丰富位置类型设置属性。

### <a name="cloud-communication"></a>云通信
[呼叫](/graph/api/resources/call?view=graph-rest-beta) 资源类型支持以下附加功能：

- [传入呼叫上下文](/graph/api/resources/incomingcontext?view=graph-rest-beta)
- 参与者的终结点类型，例如语音邮件或Skype for Business
- [更新](/graph/api/call-updaterecordingstatus?view=graph-rest-beta)[参与者](/graph/api/resources/participant?view=graph-rest-beta)[录制](/graph/api/resources/recordinginfo?view=graph-rest-beta)信息的能力

### <a name="devices-and-apps"></a>设备和应用
Intune [11 月](changelog.md#november-2019)更新

### <a name="education"></a>教育
管理员能够通过与[类](/graph/api/resources/educationclass?view=graph-rest-beta)相关的[团队](/graph/api/resources/team?view=graph-rest-beta)  **classSettings** 属性启用全类设置。 .当前没有关于向监护人通知每周分配的设置。

### <a name="identity-and-access"></a>身份和访问
- 使用应用程序权限Policy.Read.All 读取组织的条件访问策略和命名位置，无需登录用户存在。
- 允许 [条件访问策略](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta) 处于仅报告状态，`enabledForReportingButNotEnforced`。
- 使用委派权限ThreatAssessment.ReadWrite.All 或应用程序权限ThreatAssessment.Read.All，来读取（或创建，如果有读写权限）组织威胁存取请求。

### <a name="mail"></a>邮件
使用委派权限Mail.ReadBasic和应用程序权限Mail.ReadBasic.All，来管理更改[消息](/graph/api/resources/message?view=graph-rest-beta)资源更改通知的[订阅](/graph/api/resources/subscription?view=graph-rest-beta) 。

### <a name="notifications"></a>通知
使用新的轻量级通知 [Web SDK](https://aka.ms/GNSDK) 代替 [Project Rome SDK](https://github.com/Microsoft/project-rome)，以利用改进的身份验证模型和对使用 Web 推送的 Web 应用的支持。 

### <a name="people-and-workplace-intelligence"></a>人员和工作场所智能
首次推出的[配置文件](/graph/api/resources/profile?view=graph-rest-beta)资源，这是 Microsoft 服务中下一代人脉实体的丰富表示形式。 此资源与常见和切实可行的人脉属性有关，包括任何有意义的日期（如[周年纪念日](/graph/api/resources/personanniversary?view=graph-rest-beta)）的信息、[教育](/graph/api/resources/educationalactivity?view=graph-rest-beta)、[就业岗位](/graph/api/resources/workposition?view=graph-rest-beta)、[兴趣](/graph/api/resources/personinterest?view=graph-rest-beta)、[语言](/graph/api/resources/languageproficiency?view=graph-rest-beta)和[技能](/graph/api/resources/skillproficiency?view=graph-rest-beta)熟练程度、[项目参与](/graph/api/resources/projectparticipation?view=graph-rest-beta)、[网站关联](/graph/api/resources/personwebsite?view=graph-rest-beta)以及其他[帐户](/graph/api/resources/useraccountinformation?view=graph-rest-beta)和联系人信息。

### <a name="search"></a>搜索
首次推出的 [Microsoft 搜索 API](search-concept-overview.md)，它使应用用户可以获得由 Microsoft Graph 支持的更多最新、个性化和相关的搜索结果。 使用[查询](/graph/api/search-query?view=graph-rest-beta)功能，该功能默认情况下在 Microsoft 云中搜索 Outlook 邮件和事件以及 OneDrive 和 SharePoint 文件。 使用 [Microsoft Graph 连接器库](/microsoftsearch/connectors-gallery)中的[连接器](/microsoftsearch/connectors-overview)，将搜索数据包括在 Microsoft 云外部。 或者，[生成自己的连接器](/graph/api/resources/indexing-api-overview?view=graph-rest-beta#common-use-cases)、索引外部自定义项目和文件以及查询特定外部数据源。

### <a name="teamwork"></a>团队合作
使用以下 HTTP 请求语法获取与[团队](/graph/api/resources/team?view=graph-rest-beta)和[频道](/graph/api/resources/channel?view=graph-rest-beta)相关的[文件](/graph/api/resources/driveitem?view=graph-rest-beta)资源：

```http
GET /teams/{teamId}/channels/{channelId}/filesFolder
```

### <a name="users"></a>用户
使用 **creationType** 属性查找用户帐户的创建方式，例如，是将帐户创建为普通学校或工作帐户还是作为外部帐户等。

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

