---
title: Microsoft Graph 早期版本的亮点
description: Microsoft Graph 早期版本中的新增功能
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 9cb240474a6df6344c6c4b4ad66f099ff354deb8
ms.sourcegitcommit: b1e1f614299f668453916bd85761ef7b6c8d6eff
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37968487"
---
# <a name="highlights-of-earlier-releases"></a>早期版本的亮点

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
最终用户可以使用 Office 365 [MyAnalytics](social-intel-concept-overview.md#why-integrate-with-document-based-insights-preview) 应用获取与管理时间、工作协作和工作生活平衡有关的见解。 现在，你可以使用[分析 API](/graph/api/resources/social-overview?view=graph-rest-beta#help-users-gain-insights-into-their-work-patterns) 整合与工作活动（如呼叫、聊天和电子邮件）所花时间相关的数据、以帮助提高用户的工作效率和幸福感。 


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