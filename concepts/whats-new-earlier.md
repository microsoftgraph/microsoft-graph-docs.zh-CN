---
title: Microsoft Graph 早期版本的亮点
description: Microsoft Graph 早期版本中的新增功能
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 3d22924a867e55459b57c63e6563bd66e79f9c75
ms.sourcegitcommit: cea768f767cf27a938b72bb26892d70e3dedaf2e
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/08/2020
ms.locfileid: "41865856"
---
# <a name="highlights-of-earlier-releases"></a>早期版本的亮点

## <a name="december-2019-new-and-generally-available"></a>2019 年 12 月：新版本和正式版

### <a name="cloud-communications"></a>云通信
云通信 API 已正式发布，适用于[呼叫](/graph/api/resources/call?view=graph-rest-1.0)和[联机会议](/graph/api/resources/onlinemeeting?view=graph-rest-1.0)的 API [在 v1.0 中可用](/graph/api/resources/communications-api-overview?view=graph-rest-1.0)。

### <a name="education"></a>教育
使用 **classSettings** 属性管理课程专属设置，例如启用发送每周作业摘要的操作。 当团队表示[教育课程](/graph/api/resources/educationclass?view=graph-rest-1.0)时，此属性可在[团队](/graph/api/resources/team?view=graph-rest-1.0)资源中使用。

### <a name="identity-and-access"></a>标识和访问 
[尝试使用有限权限获取容器对象会返回部分数据](permissions-reference.md#limited-information-returned-for-inaccessible-member-objects)。 例如，与[用户](/graph/api/resources/user?view=graph-rest-1.0)、另一个**组**和[设备](/graph/api/resources/device?view=graph-rest-1.0)关联的[组](/graph/api/resources/group?view=graph-rest-1.0)实例。 只有 User.Read.All 和 Group.Read.All 权限且正在尝试访问此**组**实例的应用将获取**用户**和**组**实例，但获得的**设备**对象数据有限（仅限数据类型和对象 ID，不包括属性值）。

### <a name="people-and-workplace-intelligence"></a>人员和工作场所智能
见解 API 已正式发布。 在生产应用中使用此 API 确定具有以下特征的相关文档：

- 用户的[常用文档](/graph/api/insights-list-trending?view=graph-rest-1.0)
- 用户[使用的](/graph/api/insights-list-used?view=graph-rest-1.0)文档
- [与用户共享由用户共享的](/graph/api/insights-list-shared?view=graph-rest-1.0)文档

### <a name="reports"></a>报告
要使用用户委派的权限获取 Office 365 使用情况报告，管理员必须向该用户分配 Azure AD 受限管理员角色。 可以是以下角色之一：公司管理员、Exchange 管理员、SharePoint 管理员、Lync 管理员、全局读取者或报告读取者。 有关详细信息，请参阅[授权 API 读取 Office 365 使用情况报告](reportroot-authorization.md)。

### <a name="toolkit"></a>工具包
Microsoft Graph 工具包 v1.1 已发布。 有关增强功能和 bug 修复的列表，请参阅更改日历的[“2019 年 12 月”部分](changelog.md#december-2019)。

## <a name="december-2019-new-in-preview"></a>2019年12月：预览版新增功能

### <a name="cloud-communications"></a>云通信
- 使用新的[状态](/graph/api/resources/presence?view=graph-rest-beta)资源了解一名或多名用户的忙闲状态和当前活动。
- [删除](/graph/api/onlinemeeting-delete?view=graph-rest-beta)[联机会议](/graph/api/resources/onlinemeeting?view=graph-rest-beta)资源的实例。
- 要重命名和删除[呼叫](/graph/api/resources/call?view=graph-rest-beta)和[联机会议](/graph/api/resources/onlinemeeting?view=graph-rest-beta)资源的几个成员以便与这些资源的 v1 版本一致，请参阅更改日志的[“2019 年 12 月”部分](changelog.md#december-2019)。

### <a name="devices-and-apps"></a>设备和应用
Intune [12 月](changelog.md#december-2019)更新

### <a name="identity-and-access"></a>标识和访问 
- 修复了 [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta) 上 **appRoleAssignments** 和 **appRoleAssignedTo** 关系的行为。
- 使用 [Azure AD 权利管理](/graph/api/resources/entitlementmanagement-root?view=graph-rest-beta)中的 [accessPackageResourceRequest](/graph/api/resources/accesspackageresourcerequest?view=graph-rest-beta) 来请求将资源添加到 [目录](/graph/api/resources/accesspackagecatalog?view=graph-rest-beta)中，以便可在[访问包](/graph/api/resources/accesspackage?view=graph-rest-beta)中使用该资源的角色。
- 使用[威胁评估 API](/graph/api/resources/threatassessment-api-overview?view=graph-rest-beta) 帮助管理员报告可疑电子邮件、网络钓鱼 URL、电子邮件附件或其他文件。 然后，线程扫描判定会通知他们相应地调整组织策略。

### <a name="teamwork"></a>团队合作
- 针对[chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta)资源在 Microsoft 团队频道和聊天中[设置包含资源数据的更改通知](webhooks-with-resource-data.md)。
- 针对新的或已更改的[频道消息或聊天消息](/graph/api/resources/chatmessage?view=graph-rest-beta)[订阅通知](/graph/api/resources/subscription?view=graph-rest-beta)。
- 借助 [shiftPreferences](/graph/api/resources/shiftpreferences?view=graph-rest-beta) 资源，可在[日程安排](/graph/api/resources/schedule?view=graph-rest-beta)中将用户的忙线状态指定为“已分配排班”。 作为用户的[设置](/graph/api/resources/usersettings?view=graph-rest-beta)的一部分获取或设置此信息。


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

## <a name="september-2019-new-and-generally-available"></a>2019 年 9 月：新版本和正式版

### <a name="calendar-mail-and-group"></a>日历、邮件和组
[获取文件的原始内容或项目的 MIME 内容](/graph/api/attachment-get?view=graph-rest-1.0#get-the-raw-contents-of-a-file-or-item-attachment)，该项目已作为[附件](/graph/api/resources/attachment?view=graph-rest-1.0)添加到[事件](/graph/api/resources/event?view=graph-rest-1.0)、[邮件](/graph/api/resources/message?view=graph-rest-1.0)或组[帖子](/graph/api/resources/post?view=graph-rest-1.0)。

### <a name="calendar-mail-outlook-task-personal-contact"></a>日历、邮件、Outlook 任务、个人联系人
使用 [translateExchangeId](/graph/api/user-translateexchangeids?view=graph-rest-1.0) 函数在受支持的[格式](/graph/api/user-translateexchangeids?view=graph-rest-1.0#exchangeidformat-values)之间转换 Outlook 项目 ID，包括 Microsoft Graph 默认 ID 格式和不可变的 ID 格式。 

以下资源支持 ID 格式转换：

- [附件](/graph/api/resources/attachment?view=graph-rest-1.0)
- [联系人](/graph/api/resources/contact?view=graph-rest-1.0)
- [事件](/graph/api/resources/event?view=graph-rest-1.0)
- [eventMessage](/graph/api/resources/eventmessage?view=graph-rest-1.0)
- [邮件](/graph/api/resources/message?view=graph-rest-1.0)
- [outlookTask](/graph/api/resources/outlooktask?view=graph-rest-1.0)

### <a name="mail"></a>邮件
[获取邮件的 MIME 内容](outlook-get-mime-message.md)。

### <a name="microsoft-graph-toolkit"></a>Microsoft Graph 工具包
使用 [Microsoft Graph 工具包](toolkit/overview.md)开发生产应用，该应用提供一致的 Microsoft 365 外观，可以节省从 Microsoft Graph 进行身份验证和访问数据的时间。

## <a name="september-2019-new-in-preview"></a>2019 年 9 月：预览版中的新增功能

> [!IMPORTANT]
> _预览_状态下的功能（包括 API 和工具）可能会发生更改，恕不另行通知，有些功能可能永远不会提升为 GA 状态。 请不要在成品应用中使用它们。

### <a name="devices-and-apps"></a>设备和应用
Intune [9 月](changelog.md#september-2019)更新

### <a name="files"></a>文件
- 增强的同步支持：

  - 使用新的 **pendingOperations** 属性标识可能影响 [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) 的二进制内容的操作。
  - [还原](/graph/api/driveitem-restore?view=graph-rest-beta)已删除的 **driveItem**。 
- 使用安全哈希算法 (SHA-256) 增强[文件](/graph/api/resources/file?view=graph-rest-beta)数据安全性和完整性。
- 获取或设置[照片](/graph/api/resources/photo?view=graph-rest-beta)的方向。 OneDrive 个人版上支持设置。

### <a name="identity-and-access"></a>标识和访问
- 使用新的 **identities** 属性并获取[用户](/graph/api/resources/user?view=graph-rest-beta)可用于登录帐户的标识。 这些标识可由组织或诸如 Facebook、Google 和 Microsoft 等社交标识提供者提供。
- 用于在租户的云应用程序中[同步标识](/graph/api/resources/synchronization-overview?view=graph-rest-beta)的增强功能：

  - 存储[同步作业](/graph/api/resources/synchronization-synchronizationjob?view=graph-rest-beta)的设置
  - 指定对同步作业施加[隔离](/graph/api/resources/synchronization-quarantine?view=graph-rest-beta)的原因

### <a name="teamwork"></a>团队合作
使用[团队](/graph/api/resources/team?view=graph-rest-beta)的**常规**频道或自定义[成员设置](/graph/api/resources/teammembersettings?view=graph-rest-beta)，让团队成员在**团队**中创建专用频道。

### <a name="users"></a>用户
- 获取或更新[用户](/graph/api/resources/user?view=graph-rest-beta)用于登录帐户的标识。 这些标识可由商业组织或诸如 Facebook、Google 和 Microsoft 等社交标识提供者提供。
- 获取或更新用户的[邮箱首选日期和时间格式设置](/graph/api/resources/mailboxsettings?view=graph-rest-beta)。


## <a name="august-2019-new-and-generally-available"></a>2019 年 8 月：新版本和正式版 

### <a name="reports"></a>报告
- 获取与已删除项计数和大小相关的更多[邮箱使用情况数据](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-1.0)。
- 在[获取组活动详细信息](/graph/api/reportroot-getoffice365groupsactivitydetail?view=graph-rest-1.0)时，跟踪 Office 365 组 ID。
- 在获取 [OneDrive 使用帐户详细信息](/graph/api/reportroot-getonedriveusageaccountdetail?view=graph-rest-1.0)和 [SharePoint 网站使用情况详细信息](/graph/api/reportroot-getsharepointsiteusagedetail?view=graph-rest-1.0)时，跟踪所有者主体名称。
- 在[获取每 Office 365 服务的用户计数报告](/graph/api/reportroot-getoffice365servicesusercounts?view=graph-rest-1.0)时，获取 Office 365 上的活动和非活动用户数。

### <a name="security"></a>安全性
- 使用新的[适用于 Splunk 的 Microsoft Graph 安全性 API 加载项](https://aka.ms/graphsecuritysplunkaddon)将多个合作伙伴产品的安全警报和看法传输至 Splunk，从而更轻松地实时关联其安全性数据。 有关详细信息，请参阅[公告](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Introducing-the-new-Microsoft-Graph-Security-API-add-on-for/ba-p/815972)。 
- [查看由 Microsoft 或者与安全性 API 相关的 Microsoft 合作伙伴构建的其他解决方案和连接器列表](security-integration.md)，使你以统一的格式使用数据。


## <a name="august-2019-new-in-preview"></a>2019 年 8 月：预览版新增功能

> [!IMPORTANT]
> _预览_状态下的功能（包括 API 和工具）可能会发生变更，恕不另行通知；一些功能可能永远不会升级为 GA 状态。 请不要在成品应用中使用它们。

### <a name="devices-and-apps"></a>设备和应用
Intune [8 月](changelog.md#august-2019)更新

### <a name="education"></a>教育版
- 将[教师](/graph/api/resources/educationuser?view=graph-rest-beta)或[作业](/graph/api/resources/educationassignment?view=graph-rest-beta)与[评分标准](/graph/api/resources/educationrubric?view=graph-rest-beta)相关联，以解释特定作业质量和等级。 质量示例为拼写和语法，等级示例为“良好”和“不良”。 可以进一步将点数和权重与评分标准相关联。 有关详细信息，请参阅[教育版评分标准概述](education-rubric-overview.md)。
- 评估作业并从[反馈](/graph/api/resources/educationfeedbackoutcome?view=graph-rest-beta)、[数字等级](/graph/api/resources/educationpointsoutcome?view=graph-rest-beta)或[评分标准](/graph/api/resources/educationrubricoutcome?view=graph-rest-beta)方面展示结果。

### <a name="files"></a>文件
到目前为止，你已可以[关注](/graph/api/driveitem-follow?view=graph-rest-beta) [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta)，以便能够便捷访问或方便执行移动、复制和另存为等操作。 现在可以使用[取消关注](/graph/api/driveitem-unfollow?view=graph-rest-beta)操作来停止关注此类驱动器项。

### <a name="identity-and-access"></a>身份和访问
- 基于角色的访问控制 (RBAC) 提供商可以在 Azure Active Director 中[管理角色](/graph/api/resources/rolemanagement?view=graph-rest-beta)，方法是[定义可以在特定资源上执行的角色操作](/graph/api/resources/unifiedroledefinition?view=graph-rest-beta)，基于这些角色定义为用户[分配角色](/graph/api/resources/unifiedroleassignment?view=graph-rest-beta)，为他们授权相应的资源访问权限。
- 管理员可以[列出访问审查](/graph/api/accessreview-list?view=graph-rest-beta)，以高效地审核组成员身份、企业应用程序访问权限和角色分配。 定期访问审查可确保只有相应的人员才能继续以特定方式访问资源。

### <a name="social-and-workplace-intelligence"></a>社交和工作场所智能
最终用户可以使用 Office 365 [MyAnalytics](social-intel-concept-overview.md#why-integrate-with-document-based-insights) 应用获取与管理时间、工作协作和工作生活平衡有关的见解。 现在，你可以使用[分析 API](/graph/api/resources/social-overview?view=graph-rest-beta#help-users-gain-insights-into-their-work-patterns) 整合与工作活动（如呼叫、聊天和电子邮件）所花时间相关的数据、以帮助提高用户的工作效率和幸福感。 


## <a name="july-2019-new-and-generally-available"></a>2019 年 7 月：新版本和正式版 

### <a name="example-code-snippets"></a>代码片段示例
现在 v1.0 和 beta 参考中的所有 API 主题中提供了 Objective-C 代码片段。 请参阅[获取事件](/graph/api/event-get?view=graph-rest-1.0&tabs=objective-c#example)的 Objective-C 示例。

### <a name="group"></a>组
- 使用 [validateProperties](/graph/api/group-validateproperties?view=graph-rest-1.0) 函数确保现有 Office 365 组的显示名称和邮件昵称符合命名策略。
- 或者，在创建组之前，可以为 [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0) 使用 [validateProperties](/graph/api/directoryobject-validateproperties?view=graph-rest-1.0) 函数来首先验证名称。

### <a name="identity-and-access"></a>身份和访问
- 使用[新的委派和应用程序权限](permissions-reference.md#organization-permissions)、_Organization.Read.All_ 和 _Organization.ReadWrite.All_ 来访问[组织](/graph/api/resources/organization?view=graph-rest-1.0)和相关资源，例如[订阅的 SKU](/graph/api/resources/subscribedsku?view=graph-rest-1.0)。
- 使用[新的委派和应用程序权限](permissions-reference.md#role-management-permissions)、_RoleManagement.Read.Directory_ 和 _RoleManagement.ReadWrite.Directory_，对于公司目录中的与角色的访问控制 (RBAC)：

  - 使用读取/写入权限来首先[激活](/graph/api/directoryrole-post-directoryroles?view=graph-rest-1.0)目录角色。 
  - 激活角色之后，可以使用读取权限来[读取目录角色](/graph/api/directoryrole-list?view=graph-rest-1.0)、[列出角色成员](/graph/api/directoryrole-list-members?view=graph-rest-1.0)和[列出目录角色模板](/graph/api/directoryroletemplate-list?view=graph-rest-1.0)。 
  - 还可以使用读取/写入权限来[添加](/graph/api/directoryrole-post-members?view=graph-rest-1.0)和[删除](/graph/api/directoryrole-delete-member?view=graph-rest-1.0)角色成员。


## <a name="july-2019-new-in-preview"></a>2019 年 7 月：预览版新增功能

> [!IMPORTANT]
> _预览_状态下的功能（包括 API 和工具）可能会发生更改，恕不另行通知，有些功能可能永远不会提升为 GA 状态。 请不要在生产应用中使用它们。

### <a name="calendar"></a>日历 
按照 Exchange Online 管理员的设置，使用新的[位置 API](/graph/api/resources/place?view=graph-rest-beta) 来使用诸如 [room](/graph/api/resources/room?view=graph-rest-beta) 和 [room list](/graph/api/resources/roomlist?view=graph-rest-beta) 之类的富位置类型。

### <a name="devices-and-apps"></a>设备和应用
Intune [7 月](changelog.md#july-2019)更新

### <a name="files"></a>文件 
在为文件、文件夹或其他 [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) [创建共享链接](/graph/api/driveitem-createlink?view=graph-rest-beta)时，应用到期日期/时间或密码。

### <a name="identity-and-access"></a>标识和访问
- 使用[新的应用程序权限](/graph/permissions-reference?#accessreviews-permissions) _AccessReview.ReadWrite.Membership_ 对[访问权限审阅](/graph/api/resources/accessreviews-root?view=graph-rest-beta)执行 CRUD 操作。 
- 使用[新的委派和应用程序权限](permissions-reference.md#administrative-units-permissions)、_AdministrativeUnit.Read.All_ 和 _AdministrativeUnit.ReadWrite.All_，以分别读取或写入（包括创建、更新、删除或管理成员身份）[管理单元](/graph/api/resources/administrativeunit?view=graph-rest-beta)资源。
- 使用[新的委派和应用程序权限](permissions-reference.md#organization-permissions)、_Organization.Read.All_ 和 _Organization.ReadWrite.All_ 来访问[组织](/graph/api/resources/organization?view=graph-rest-beta)和相关资源，例如[订阅的 SKU](/graph/api/resources/subscribedsku?view=graph-rest-beta)。
- 使用新的 [discover](/graph/api/directorydefinition-discover?view=graph-rest-beta) 函数查找最新的目录[同步架构](/graph/api/resources/synchronization-synchronizationschema?view=graph-rest-beta)，以便将目录对象、属性及类型同步到应用。
- 使用[功能推出策略](/graph/api/resources/featureRolloutPolicy?view=graph-rest-beta)帮助租户管理员在为整个组织启用一些功能之前，针对特定组试用这些功能。

### <a name="mail"></a>邮件
使用更精确的应用程序权限 _Mail.ReadBasic.All_ 来读取用户邮箱（邮件正文除外）、预览正文、附件和扩展属性，不包括搜索邮箱。 现适用于 [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-beta) 以及针对[邮件](/graph/api/resources/message?view=graph-rest-beta) 和 **mailFolder** 的[更改跟踪](delta-query-overview.md)

### <a name="reports"></a>报告
- 获取与已删除的项目计数和大小相关的其他[邮箱使用情况数据](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-beta)。

### <a name="teamwork"></a>团队合作
- 为用户[安装](/graph/api/user-add-teamsappinstallation?view=graph-rest-beta)、[卸载](/graph/api/user-delete-teamsappinstallation?view=graph-rest-beta)、[升级](/graph/api/user-upgrade-teamsappinstallation?view=graph-rest-beta)和[列出已安装的 Microsoft Teams 应用](/graph/api/user-list-teamsappinstallation?view=graph-rest-beta)。
- 使用仅应用访问权限来读取频道消息、频道消息回复以及聊天中的消息。 [请求和批准](teams-protected-apis.md)此类访问。

## <a name="may---june-2019-new-and-generally-available"></a>2019 年 5 月 - 7 月：新版本和正式版

### <a name="calendar-mail-and-personal-contacts"></a>日历、邮件和个人联系人
Exchange 管理员可以向应用程序授予应用程序权限, 并[限制该应用仅访问邮箱 ](auth-limit-mailbox-access.md) 的子集, 而不是默认的访问组织中的所有邮箱。 此类受限访问适用于授予[日历](permissions-reference.md#calendars-permissions)、 [联系人](permissions-reference.md#contacts-permissions)及[邮件和邮箱设置](permissions-reference.md#mail-permissions)的应用的任何应用程序权限。 查看相关的[博客公告](https://developer.microsoft.com/graph/blogs/scoping-microsoft-graph-application-permissions-to-specific-exchange-online-mailboxes/)。

### <a name="mail"></a>邮件
使用[邮件搜索文件夹](/graph/api/resources/mailsearchfolder?view=graph-rest-1.0) API 来搜索邮件, 并访问 Outlook 电子邮件搜索结果。 查看相关的[博客公告](https://developer.microsoft.com/graph/blogs/mail-search-folder-support-for-microsoft-graph-apis/)。

### <a name="postman"></a>Postman
除 Graph 资源管理器外, 请在[Microsoft Graph Postman 集合](use-postman.md)中试用 Microsoft Graph API, 了解 API 行为并加速应用程序开发。

### <a name="tutorials"></a>教程
尝试使用新[教程构建 Java 控制台应用](/graph/tutorials/java) , 以获取有关用户日历的信息。

### <a name="user"></a>用户
管理员或用户可以[吊销](/graph/api/user-revokesigninsessions?view=graph-rest-1.0)用户的所有已颁发的刷新令牌。 通常用于防止已丢失或被盗设备上的应用访问组织的数据。


## <a name="may---june-2019-new-in-preview"></a>2019 年 5 月 - 7 月：预览版新增功能

> [!IMPORTANT]
> _预览_状态下的功能（包括 API 和工具）可能会发生更改，恕不另行通知，有些功能可能永远不会提升为 GA 状态。 请不要在成品应用中使用它们。

### <a name="devices-and-apps"></a>设备和应用
- Intune [5月](changelog.md#may-2019)更新 
- Intune [6月](changelog.md#june-2019)更新

### <a name="education"></a>教育
- [educationSchool](/graph/api/resources/educationschool?view=graph-rest-beta)的增量查询。
- [educationClass](/graph/api/resources/educationclass?view=graph-rest-beta) 和 [educationUser](/graph/api/resources/educationuser?view=graph-rest-beta)的增量查询和属性添加。 

### <a name="group"></a>组
获取[敏感度标签](/graph/api/resources/assignedlabel?view=graph-rest-beta) , 帮助保护 Office 365 组的敏感数据并满足合规性策略。 这些标签是[assignedLabel](/graph/api/resources/assignedlabel?view=graph-rest-beta)对象，由 Microsoft 365 安全与合规性中心的管理员发布，作为 Microsoft 信息保护功能的一部分。 

### <a name="identity-and-access"></a>身份和访问控制
- 获取[应用程序](/graph/api/resources/applicationtemplate?view=graph-rest-beta)的实例，或将 Azure AD 应用程序库中的实例作为模板添加到目录中。
- 获取租户中所有[预配事件](/graph/api/resources/provisioningobjectsummary?view=graph-rest-beta)目录的列表。
- 获取有关 Azure AD 环境中[检测到的用户或登录风险](/graph/api/resources/riskdetection?view=graph-rest-beta)的信息。 此风险检测功能是 Azure AD 标识保护的一部分。

### <a name="mail"></a>邮件
使用更精确的代理权限 _Mail.ReadBasic_ 来读取用户邮箱（邮件正文除外）、预览正文、附件和扩展属性，不包括搜索邮箱。 可用于读取 [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-beta) 方法和更改 [message](/graph/api/resources/message?view=graph-rest-beta) 和 **mailFolder** 的 [跟踪](delta-query-overview.md)。

### <a name="microsoft-graph-toolkit"></a>Microsoft Graph 工具包
[Microsoft Graph 工具包](/graph/toolkit/overview)是一组框架不可知的 web 组件和帮助器, 提供对 Microsoft Graph 中的数据进行身份验证和访问的便利。  由于 Microsoft Graph 工具包处于预览状态，请仅在非生产应用中使用工具包提供程序和组件。

### <a name="reports"></a>报告
- 获取组织中用户采用的[身份验证方法的报告](/graph/api/resources/authenticationmethods-usage-insights-overview?view=graph-rest-beta)，例如自助服务密码重置和多因素身份验证 (MFA).。

### <a name="sites"></a>网站
让用户[关注](/graph/api/site-follow?view=graph-rest-beta)或[取消关注](/graph/api/site-unfollow?view=graph-rest-beta) SharePoint 网站。

### <a name="teamwork"></a>团队合作
- 在 Microsoft 团队[聊天消息](/graph/api/resources/chatmessagehostedimage?view=graph-rest-beta)中存储[图像](/graph/api/resources/chatmessage?view=graph-rest-beta)。 
- 支持[配置](/graph/api/resources/teamdiscoverysettings?view=graph-rest-beta)私人团队的发现方式。


## <a name="january---april-2019-new-and-generally-available"></a>2019 年 1 月 - 4 月：新版本和正式版

[Microsoft Graph 数据连接](data-connect-concept-overview.md)

### <a name="calendar"></a>日历
[获取忙/闲日程安排](outlook-get-free-busy-schedule.md)

### <a name="identity-and-access"></a>身份和访问控制
[身份提供程序](/graph/api/resources/identityprovider?view=graph-rest-1.0)
[改进的身份验证指南](/graph/auth)
[将应用从 Azure AD Graph 迁移到 Microsoft Graph](migrate-azure-ad-graph-overview.md)

### <a name="sdks"></a>SDK
[SDK 指南](/sdks/sdks-overview.md) API 片段（[示例](/graph/api/user-get?view=graph-rest-1.0&tabs=cs#sdk-sample-code)）

### <a name="security"></a>安全性
[租户安全功能分数](/graph/api/resources/securescore?view=graph-rest-1.0)

## <a name="january---april-2019-new-in-preview"></a>2019 年 1 月 - 4 月：预览版中的新功能

### <a name="calendar-group-mail-to-do-tasks"></a>日历、群组、邮件、待办任务
[获取事件、消息、Outlook 任务或组帖子中文件或项目附件的原始/MIME 内容](/graph/api/attachment-get?view=graph-rest-beta#get-the-raw-contents-of-a-file-or-item-attachment)

### <a name="change-notifications"></a>更改通知
[减少 Outlook 资源的缺失更改通知](webhooks-outlook-authz.md)

### <a name="devices-and-apps"></a>设备和应用
- Intune [1 月](changelog.md#january-2019)更新 
- Intune [2 月](changelog.md#february-2019)更新
- Intune [3 月](changelog.md#march-2019)更新
- Intune [4 月](changelog.md#april-2019)更新

### <a name="files"></a>文件
[共享邀请](/graph/api/driveitem-invite?view=graph-rest-beta)包含过期时间和密码

### <a name="financials"></a>财务
[Dynamics 365 Business Central](dynamics-business-central-concept-overview.md)

### <a name="identity-and-access"></a>身份和访问控制
[访问评审](/graph/api/resources/accessreviews-root?view=graph-rest-beta)支持应用程序权限[审核和登录日志](/graph/api/resources/azure-ad-auditlog-overview?view=graph-rest-beta)
[Azure AD B2C 中的自定义注册和登录](/graph/api/resources/trustframeworkpolicy?view=graph-rest-beta)
[存在风险的用户](/graph/api/resources/riskyuser?view=graph-rest-beta)和[历史记录](/graph/api/resources/riskyuserhistoryitem?view=graph-rest-beta)

### <a name="mail"></a>邮件
[获取消息的 MIME 内容](outlook-get-mime-message.md)

### <a name="reports"></a>报表
[应用程序登录报表](/graph/api/resources/applicationsigninsummary?view=graph-rest-beta)

### <a name="security"></a>安全性
[安全操作](/graph/api/resources/securityaction?view=graph-rest-beta)
[威胁指示器](/graph/api/resources/tiindicator?view=graph-rest-beta)

### <a name="teamwork"></a>团队合作
[一对一聊天](/graph/api/resources/chat?view=graph-rest-beta)
[排班管理](/graph/api/resources/shift?view=graph-rest-beta)

## <a name="see-also"></a>另请参阅
- 请参阅 Microsoft Graph 中的[新增功能](whats-new-overview.md)。
- 定期查看 [Microsoft Graph 开发人员博客](https://developer.microsoft.com/graph/blogs/), 了解发布公告和有帮助的资源。 
- 浏览 Microsoft Graph API 新增功能的详细信息, 以及[changelog](changelog.md)中的 API 行为更新。