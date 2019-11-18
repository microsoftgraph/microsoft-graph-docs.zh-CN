---
title: Microsoft Graph 新增功能
description: Microsoft Graph 新增功能
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: f1fe26cf74a99e0b94bdb8adf9c0ae36d24621c2
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/15/2019
ms.locfileid: "38656492"
---
# <a name="whats-new-in-microsoft-graph"></a>Microsoft Graph 新增功能

查看 Microsoft Graph 中的新增功能要点，并查看你可如何[分享你的想法](#want-to-stay-in-the-loop)。 有关 API 更新的完整列表，请参阅 API 更改日志的 [11 月](changelog.md#november-2019)和 [10 月](changelog.md#october-2019)部分。 

> [!IMPORTANT]
> _预览_状态下的功能（包括 API 和工具）可能会发生更改，恕不另行通知，有些功能可能永远不会提升为正式发布 (GA) 状态。 不要在成品应用中使用预览功能。


## <a name="november-2019-new-and-generally-available"></a>2019 年 11 月：新版本和正式版

### <a name="identity-and-access"></a>身份和访问

注册通过 Azure Active Directory (Azure AD) 进行身份验证的[应用程序](/graph/api/resources/application?view=graph-rest-1.0)。 根据需要使用委派的[权限](/graph/permissions-reference#application-resource-permissions)（即 Application.Read.All 和 Application.ReadWrite.All）或应用程序权限（即 Application.Read.All）。


## <a name="november-2019-new-in-preview"></a>2019 年 11 月：预览版中的新增功能

### <a name="calendar"></a>日历

[为](/graph/api/place-update?view=graph-rest-beta)[会议室](/graph/api/resources/room?view=graph-rest-beta)和[会议室列表](/graph/api/resources/roomlist?view=graph-rest-beta)的丰富位置类型设置属性。

### <a name="devices-and-apps"></a>设备和应用
Intune [11 月](changelog.md#november-2019)更新

### <a name="notifications"></a>通知
使用新的轻量级通知 [Web SDK](https://aka.ms/GNSDK) 代替 [Project Rome SDK](https://github.com/Microsoft/project-rome)，以利用改进的身份验证模型和对使用 Web 推送的 Web 应用的支持。 

### <a name="people-and-workplace-intelligence"></a>人员和工作场所智能

首次推出的[配置文件](/graph/api/resources/profile?view=graph-rest-beta)资源，这是 Microsoft 服务中下一代人脉实体的丰富表示形式。 此资源与常见和切实可行的人脉属性有关，包括任何有意义的日期（如[周年纪念日](/graph/api/resources/personanniversary?view=graph-rest-beta)）的信息、[教育](/graph/api/resources/educationalactivity?view=graph-rest-beta)、[就业岗位](/graph/api/resources/workposition?view=graph-rest-beta)、[兴趣](/graph/api/resources/personinterest?view=graph-rest-beta)、[语言](/graph/api/resources/languageproficiency?view=graph-rest-beta)和[技能](/graph/api/resources/skillproficiency?view=graph-rest-beta)熟练程度、[项目参与](/graph/api/resources/projectparticipation?view=graph-rest-beta)、[网站关联](/graph/api/resources/personwebsite?view=graph-rest-beta)以及其他[帐户](/graph/api/resources/useraccountinformation?view=graph-rest-beta)和联系人信息。


### <a name="search"></a>搜索
首次推出的 [Microsoft 搜索 API](search-concept-overview.md)，它使应用用户可以获得由 Microsoft Graph 支持的更多最新、个性化和相关的搜索结果。 使用[查询](/graph/api/search-query?view=graph-rest-beta)功能，该功能默认情况下在 Microsoft 云中搜索 Outlook 邮件和事件以及 OneDrive 和 SharePoint 文件。 使用 [Microsoft Graph 连接器库](/microsoftsearch/connectors-gallery)中的[连接器](/microsoftsearch/connectors-overview)，将搜索数据包括在 Microsoft 云外部。 或者，[生成自己的连接器](/graph/api/resources/indexing-api-overview?view=graph-rest-beta#common-use-cases)、索引外部自定义项目和文件以及查询特定外部数据源。


## <a name="october-2019-new-and-generally-available"></a>2019 年 10 月：新版本和正式版

### <a name="identity-and-access"></a>身份和访问
- 在生产应用中使用[组织联系人](/graph/api/resources/orgcontact?view=graph-rest-1.0)。 组织联系人由组织管理员管理，可以从本地 Active Directory 或 Exchange Online 同步。
- 在[组织](/graph/api/resources/organization?view=graph-rest-1.0)中配置[基于证书的身份验证](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-certificate-based-authentication-get-started)。
- 为[应用程序](/graph/api/resources/application?view=graph-rest-1.0)添加和删除[密码凭据](/graph/api/resources/passwordcredential?view=graph-rest-1.0)。

### <a name="mail"></a>邮件
使用新的 **message** 参数更新[回复](/graph/api/message-reply?view=graph-rest-1.0)邮件时任何可写的 [message](/graph/api/resources/message?view=graph-rest-1.0) 属性，例如，[将收件人添加到回复](/graph/api/message-reply#example?view=graph-rest-1.0)。

### <a name="microsoft-graph-data-connect"></a>Microsoft Graph 数据连接
开发人员和数据科学家现在可以使用[工具将 Office 365 数据转换为通用数据模型格式](https://github.com/OfficeDev/MS-Graph-Data-Connect/blob/master/Common-Data-Model/README.md)，从而使其与其他支持开放数据倡议 (ODI) 的数据集大致保持一致。 


### <a name="microsoft-graph-sdks"></a>Microsoft Graph SDK
- 使用 JavaScript SDK 中的混乱处理程序来验证应用程序是否可以应对棘手的服务器故障。
- 了解有关[使用 SDK 进行 API 调用](/graph/sdks/create-requests)的信息。

### <a name="users"></a>用户
- [获取](/graph/api/user-get-mailboxsettings?view=graph-rest-1.0)或[设置](/graph/api/user-update-mailboxsettings?view=graph-rest-1.0)[用户邮箱](/graph/api/resources/mailboxsettings?view=graph-rest-1.0)的用户首选日期和时间格式设置。 
- 跟踪[用户](/graph/api/resources/user?view=graph-rest-1.0)上一次密码更改的日期/时间。

## <a name="october-2019-new-in-preview"></a>2019 年 10 月：预览版中的新增功能

### <a name="calendar"></a>日历
- 会议组织者可以[允许被邀请者提议备选会议时间](outlook-calendar-meeting-proposals.md)。 当收到包含建议的备选时间的会议响应时，组织者可以决定接受该建议并[更新](/graph/api/event-update?view=graph-rest-beta)会议时间。
- 编程日历共享与 Outlook 用户体验的奇偶校验更加接近。 除了跟踪日历的当前用户权限和共享状态之外：
  - 对于每个[日历](/graph/api/resources/calendar?view=graph-rest-beta)，你现在可以管理与之共享日历的每个用户的[权限](/graph/api/resources/calendarpermission?view=graph-rest-beta)。 
  - 对于每个[邮箱](/graph/api/resources/mailboxsettings?view=graph-rest-beta)，你现在可以指定代理人、邮箱所有者，还是两者同时接收会议邮件和会议响应。 
- 其他在线会议支持：
  - 对于每个**日历**，指定允许的和默认的在线会议提供程序。
  - 创建或更新[事件](/graph/api/resources/event?view=graph-rest-beta)以使其在线可用，并提供详细信息供与会者加入在线会议。 
  - 具体来说，使用**事件**的新 **onlineMeetingProvider** 和 **onlineMeeting** 属性来将 Microsoft Teams 设置或标识为在线会议提供程序，这是 **onlineMeetingUrl** 属性的[已知问题](known-issues.md#onlinemeetingurl-property-support-for-microsoft-teams)的解决方法。

### <a name="devices-and-apps"></a>设备和应用
Intune [10 月](changelog.md#october-2019)更新

### <a name="graph-explorer"></a>Graph 浏览器
尝试使用[下一版本的 Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer/preview)，并在新的“权限”****、“身份验证”**** 和“代码片段”**** 选项卡中查看权限、访问令牌和 SDK 代码片段等便捷的上下文信息。 使用“预览”**** 滑块在[生产](https://developer.microsoft.com/graph/graph-explorer)和 Graph Explorer 的新预览版本之间切换。

### <a name="groups"></a>组
- 使用 **hideFromAddressLists** 和 **hideFromOutlookClients** 属性在 Outlook 用户界面的某些部分或 Outlook 客户端中控制[组](/graph/api/resources/group?view=graph-rest-beta)的可见性。
- [分配](/graph/api/group-assignlicense?view=graph-rest-beta)或删除[组](/graph/api/resources/group?view=graph-rest-beta)中用户的许可证。

### <a name="identity-and-access"></a>标识和访问
- 使用[条件访问策略](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta)自定义组织的访问规则。 这些规则会考虑有关用户或设备标识（如用户或组成员身份、IP 位置）的信号，以及尝试访问特定应用程序等行为和有风险的登录行为。
- 使用[权利管理](/graph/api/resources/entitlementmanagement-root?view=graph-rest-beta)来管理组织内外的用户对组、应用程序和 SharePoint Online 网站的访问。
- 为[应用程序](/graph/api/resources/application?view=graph-rest-beta)和[服务主体](/graph/api/resources/serviceprincipal?view=graph-rest-beta)添加和删除[密码凭据](/graph/api/resources/passwordcredential?view=graph-rest-beta)。
- 管理 Azure AD B2C [信任框架策略密钥](/graph/api/resources/trustframeworkkeyset?view=graph-rest-beta)。
- 定义 Azure AD B2C [用户流](/graph/api/resources/identityuserflow?view=graph-rest-beta)策略，用于登录、注册、合并注册和登录、密码重置和配置文件更新。
- 配置[信息保护标签](/graph/api/resources/informationprotectionlabel?view=graph-rest-beta)以对用户或租户的敏感度进行分类。
- 将 API 用于[标识风险事件](/graph/api/resources/identityriskevent?view=graph-rest-beta)的现有应用应转换为适用于 Azure AD Identity Protection 中[风险检测](/graph/api/resources/riskdetection?view=graph-rest-beta)的应用。 有关更多详细信息和弃用时间线，请参阅相关的[博客文章](https://developer.microsoft.com/graph/blogs/deprecatation-of-the-identityriskevents-api/)。


### <a name="mail"></a>邮件
通过创建[上载会话](/graph/api/resources/uploadsession?view=graph-rest-beta)，[将高达 150MB 的大文件附加到](outlook-large-attachments.md) [message](/graph/api/resources/message?view=graph-rest-beta) 实例，并迭代上载文件的范围，直至文件的所有字节都已上载。 

### <a name="microsoft-graph-security-api"></a>Microsoft Graph 安全性 API
- 预览版与 RSA NetWitness、ServiceNow 和 Splunk 集成，以关联和同步[警报](/graph/api/resources/security-api-overview?view=graph-rest-beta#alerts)，并改善威胁防护和响应。
- 已将新触发器添加到适用于逻辑应用和流的 [Microsoft Graph 安全连接器](https://docs.microsoft.com/connectors/microsoftgraphsecurity/)和 [playbook](https://docs.microsoft.com/azure/security-center/security-center-playbooks) 中。 请参阅 [playbook 示例](https://github.com/microsoftgraph/security-api-solutions/tree/master/Playbooks)。
- 支持向 Microsoft Defender ATP 发送[威胁指示器](/graph/api/resources/security-api-overview?view=graph-rest-beta#threat-indicators-preview)，以使用其自己的智能源阻止威胁或发出威胁警报。 通过与 ThreatConnect 等合作伙伴集成，客户能够直接从威胁智能和自动化解决方案发送指示器。 

### <a name="notifications"></a>通知
- [创建通知并将其发送给用户登录的所有设备终结点上的所有应用程序客户端](/graph/api/user-post-notifications?view=graph-rest-beta)，而无需管理用户委派的权限。
- 在用户[通知](/graph/api/resources/notification?view=graph-rest-beta)上使用[目标策略终结点](/graph/api/resources/targetpolicyendpoints?view=graph-rest-beta)，以便专门针对 Windows、iOS、Android 或 WebPush 平台投放通知。
- 在 iOS 终结点的通知上指定[回退策略](/graph/api/resources/fallbackpolicy?view=graph-rest-beta)，以便发送由于平台特定的限制（如节电模式）而可能无法传递到设备的高优先级原始通知。

 
### <a name="powershell-sdk"></a>PowerShell SDK 
开发人员和 IT 专业人员会注意到推出了 [Microsoft Graph Powershell SDK](https://github.com/microsoftgraph/msgraph-sdk-powershell)，该 SDK 将生成包含用于发出 Microsoft Graph REST API 请求的 cmdlet 的模块。

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

