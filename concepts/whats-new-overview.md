---
title: Microsoft Graph 新增功能
description: Microsoft Graph 新增功能
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 9da26e00f398ec29ce138a598d9bc7d1faba8bbf
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2020
ms.locfileid: "48849121"
---
# <a name="whats-new-in-microsoft-graph"></a>Microsoft Graph 新增功能

查看 Microsoft Graph 中的最近两个月新增功能要点、[以前增加的内容](whats-new-earlier.md)以及如何[分享你的想法](#want-to-stay-in-the-loop)。 有关 API 级更新的详细列表，请参见 [API更改日志](changelog.md)。 

> [!IMPORTANT]
> _预览_ 状态下的功能（包括 API 和工具）可能会发生更改，恕不另行通知，有些功能可能永远不会提升为正式发布 (GA) 状态。 不要在成品应用中使用预览功能。

## <a name="october-2020-new-and-generally-available"></a>2020年 10 月：新版本和正式版

### <a name="application"></a>应用程序
- 使用[主页领域发现](/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#home-realm-discovery)策略，允许将[电子邮件作为 Azure AD 的备用登录 ID](/azure/active-directory/authentication/howto-authentication-use-email-signin)。 当用户提供登录 ID 后，无论是否提示用户进行身份验证，主页领域发现策略都会确定。 在这种情况下，设置 [homeRealmDiscoveryPolicy](/graph/api/resources/homerealmdiscoverypolicy) 资源的 **AlternateIdLogin** 属性，可使用户使用电子邮件地址登录。
- 获取 [应用程序](/graph/api/resources/application)或 [servicePrincipal](/graph/api/resources/serviceprincipal) 的经过验证的发布者信息，并为 **应用程序**[设置](/graph/api/application-setverifiedpublisher)或[删除](/graph/api/application-unsetverifiedpublisher)经过验证的发布者信息。

### <a name="change-notifications"></a>更改通知
现在，产品应用可订阅 Outlook [消息](/graph/api/resources/message)、 [事件](/graph/api/resources/event)和[联系人](/graph/api/resources/contact)的生命周期通知以及 Teams [chatMessage](/graph/api/resources/chatmessage)，以便[减少订阅丢失和更改通知](webhooks-lifecycle.md)。

### <a name="identity-and-access"></a>身份和访问
- 目录对象上的高级 OData 系统查询选项（`$count`、 `$search`和 `$filter`）的 GA。
- 查看显示目录对象上的 OData 转换的示例。
- 有关增强 API 的列表，请参阅更改日志 [10](changelog.md#october-2020) 月更新的标识和访问部分。

### <a name="teamwork"></a>团队合作
- [conversationMember](/graph/api/resources/conversationmember) 和 [aadUserConversationMember](/graph/api/resources/aaduserconversationmember)的完整 CRUD 操作集的 GA。 这些资源代表聊天或频道对话中的一个成员，可能是也可能不是 Azure AD 中的用户。
- Teams [chatMessage](/graph/api/resources/chatmessage) 资源的生命周期通知的 GA， [减少缺失的订阅和更改通知](webhooks-lifecycle.md)。

### <a name="to-do-tasks"></a>待办任务
[Microsoft for API 的 GA](/graph/api/resources/todo-overview?view=graph-rest-1.0&preserve-view=true) - 使用产品应用中的待办 API 创建和管理属于用户工作流的任务，例如创建电子邮件的任务。  

### <a name="users"></a>用户
获取适用于公司员工的[用户](/graph/api/resources/user)新属性：聘用日期、组织协会（如分部和成本中心）和员工类型（如顾问、合同工或供应商）。 这些属性需要在 GET 操作中指定 `$select`OData 查询参数。

## <a name="october-2020-new-in-preview-only"></a>2020 年 10 月：仅限预览版中的新增功能

### <a name="cloud-communications--online-meeting"></a>云通信 | 联机会议
- 通过使用 [meetingParticipantInfo](/graph/api/resources/meetingParticipantInfo?view=graph-rest-beta&preserve-view=true) 类型的 **role** 属性，将 [在线会议](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true)中的参与者区分为与会者或报告者。
- [筛选会议的 joinWebUrl 属性](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true#example-3-retrieve-an-online-meeting-by-joinweburl)，获取 [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true)。

### <a name="devices-and-apps--cloud-printing"></a>设备和应用 | 云打印

- 不支持 **uploadData** 操作，支持 [创建上传会话](/graph/api/printdocument-createuploadsession?view=graph-rest-beta&preserve-view=true) [将文档](upload-data-to-upload-session.md)上传到打印机或打印机共享。
- 不支持 [printDocument](/graph/api/resources/printdocument?view=graph-rest-beta&preserve-view=true) 的 **configuration** 属性，支持 [printJob](/graph/api/resources/printjob?view=graph-rest-beta&preserve-view=true) 上类似的 **configuration** 属性。
- 使用 **redirectedFrom** 或 **redirectedTo** 属性获取要重定向的 **printJob** 的资源或目标工作 URL。
- 使用 **state** 属性和全新 **details** 属性获取 **printJob** 的当前状态。
- 使用 **分享** 关系获取与 [打印机](/graph/api/resources/printer?view=graph-rest-beta&preserve-view=true)关联的打印机共享的集合。 
- 不支持 **打印机** 的 **processingStateReasons** 属性，支持 **status** 属性。 **status** 属性为键入 [打印机状态](/graph/api/resources/printerstatus?view=graph-rest-beta&preserve-view=true)，并公开 **details** 属性。 使用 **details** 属性识别打印机处于当前状态的原因。
- 不支持 [printerCapabilities](/graph/api/resources/printercapabilities?view=graph-rest-beta&preserve-view=true) 的 **feedDirections** 属性，支持 **feedOrientations** 属性，以获取打印机支持的源方向。
- 有关 API 和属性的重命名和其他不支持的部分，请参阅更改日志 [10 月](changelog.md#october-2020)更新的云打印部分。

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理
Intune beta 版 [10 月](changelog.md#october-2020)更新。

### <a name="files"></a>文件
[撤销](/graph/api/permission-revokegrants?view=graph-rest-beta&preserve-view=true)通过共享链接授予的 [driveItem](/graph/api/resources/listitem?view=graph-rest-beta&preserve-view=true) 或 [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta&preserve-view=true) 的访问权限。

### <a name="identity-and-access--identity-and-sign-in"></a>身份和访问 | 身份和登录
- 管理[身份验证方法](/graph/api/resources/authenticationmethodspolicies-overview?view=graph-rest-beta&preserve-view=true)策略，以识别可以使用特定多重身份验证方法登录 Azure Active Directory 的用户。 配置策略以定义以下内容：
  - 可以在 Azure AD 租户中使用的 FIDO2 安全密钥类型。
  - 允许使用 FIDO2 安全密钥或无密码电话登录来登录 Azure AD 的用户或用户组。
- 为用户配置[电子邮件身份验证方法](/graph/api/resources/emailauthenticationmethod?view=graph-rest-beta&preserve-view=true)，以自助重置密码。
- 使用 [Azure AD B2C](/azure/active-directory-b2c/overview) 并[选择一种机制来配置并允许最终用户通过本地帐户进行身份验证](/graph/api/resources/b2cauthenticationmethodspolicy?view=graph-rest-beta&preserve-view=true)。
- 使用 `Policy.ReadWrite.AuthenticationMethod` 来读取或写入组织的身份验证方法策略，作为代表已登录用户的委托权限或不存在已登录用户的情况下的应用程序权限。
- 在[授权策略](/graph/api/resources/authorizationpolicy?view=graph-rest-beta&preserve-view=true)中指定是否以及谁可以邀请外部用户加入组织。

### <a name="people-and-workplace-intelligence--insights"></a>人脉和工作场所智能 | 见解 
管理员可以查看[使用 PowerShell cmdlet 的示例](insights-customize-item-insights-privacy.md#how-to-configure-item-insights-setting-via-powershell)，为组织自定义项目见解设置。

### <a name="teamwork"></a>团队合作
- 使用实例属性 **channelCreationMode** 表明正在创建 [通道](https://docs.microsoft.com/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true#instance-attributes)以服务数据迁移。 使用 [completeMigration](/graph/api/channel-completemigration?view=graph-rest-beta&preserve-view=true) 表明迁移已结束，以便成员可以发布和阅读邮件。
- 使用实例属性 **teamCreationMode** 表明正在创建 [团队](https://docs.microsoft.com/graph/api/resources/team?view=graph-rest-beta&preserve-view=true#instance-attributes)以服务迁移。 使用 [completeMigration](/graph/api/team-completemigration?view=graph-rest-beta&preserve-view=true) 表明迁移已结束，以便成员可以操作和发布邮件。


## <a name="september-2020-new-and-generally-available"></a>2020 年 9 月：新版本和正式版

### <a name="calendar"></a>日历
[事件](/graph/api/resources/event)资源的 **transactionId** 属性 GA，可选择由客户端应用程序设置，以避免客户端重试创建相同事件时出现多余的 POST 操作。 当低网络连接性导致客户端在从服务器中收到客户端先前创建事件请求的响应之前超时时，此功能很有用。

### <a name="cloud-communications"></a>云通信
[从[通话](/graph/api/resources/call)中删除参与者](/graph/api/participant-delete)。 即使在有必要删除活动通话的参与者的情况下，也可以使用此操作。

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理
Intune [v 1.0 版的 9 月](changelog.md#september-2020) 更新。

### <a name="identity-and-access--directory-management"></a>身份和访问 | 目录管理
GA [管理单元 API](/graph/api/resources/administrativeunit) ，允许组织细分其 Azure Active Directory、管理这些细分并将管理职责委派给这些细分。 这些细分项可以代表区域、部门、成本中心等。

### <a name="reports"></a>报告
[获取含 Outlook 2019 和 Outlook for Microsoft 365 唯一用户的计数报告](/graph/api/reportroot-getemailappusageversionsusercounts)。

### <a name="teamwork"></a>团队合作
- 获取 **lastEditedDateTime** 属性，确定发件人上次编辑 [聊天](/graph/api/resources/chatmessage)邮件的时间。
- 获取 **lastModifiedDateTime** 属性，确定发件人何时创建聊天邮件，或者任何人以其他方式修改邮件，包括添加或删除反应。 
- [获取有关[聊天邮件](/graph/api/resources/chatmessage)中](webhooks.md)更改的通知。
- [更新](/graph/api/chatmessage-update?view=graph-rest-beta&preserve-view=true)[频道](/graph/api/resources/channel&preserve-view=true)或 [聊天](/graph/api/resources/chat&preserve-view=true)内 [chatMessage](/graph/api/resources/chatmessagepreserve-view=true) 的 **policyViolation** 属性，从而启用数据丢失防护 (DLP) 应用，以监控 [聊天邮件策略冲突](/graph/api/resources/chatmessagepolicyviolation?preserve-view=true) ，防止包含用户不应发送的数据的邮件。

### <a name="use-the-sdks"></a>使用 SDK
[Microsoft Graph PowerShell SDK](https://github.com/microsoftgraph/msgraph-sdk-powershell) 的 GA 版可通过直接和一致的方式访问 Microsoft Graph 的整个表面。

### <a name="use-the-toolkit"></a>使用工具包
尝试使用 Microsoft Graph 工具包的全新分步入门教程，并体验工具包带来的方便性：
- [使用 JavaScript 构建 Web 应用程序](./toolkit/get-started/build-a-web-app.md)
- [构建 SharePoint Web 部件](./toolkit/get-started/build-a-sharepoint-web-part.md)
- [构建 Microsoft Teams 选项卡](./toolkit/get-started/build-a-microsoft-teams-tab.md)
- [使用 React 的工具包](./toolkit/get-started/use-toolkit-with-react.md)
- [使用 Angular 的工具包](./toolkit/get-started/use-toolkit-with-angular.md)

### <a name="users"></a>用户
除通过“ **邮件** 属性” 获取 [用户](/graph/api/resources/user) 的 SMTP 地址之外，你现在可以设置该属性并更新用户的电子邮件地址。 

## <a name="september-2020-new-in-preview-only"></a>2020 年 9 月：仅限预览版的新增功能

### <a name="application"></a>应用程序
创建、列出或删除[服务主体](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true)公开的[委派权限分类](/graph/api/resources/delegatedpermissionclassification?view=graph-rest-beta&preserve-view=true)。 将委派权限分类与[用户同意设置](/azure/active-directory/manage-apps/configure-user-consent)结合使用可以对允许最终用户向应用授予同意的条件进行限制。

### <a name="cloud-communications"></a>云通信
- 弃用了 [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true)的 **autoAdmittedUsers** 属性。 使用新的 **lobbyBypassSettings** 属性和 [值](/graph/api/resources/lobbybypasssettings?view=graph-rest-beta&preserve-view=true#lobbybypassscope-values)取而代之。
- 使用宣布呼叫者加入或离开联机会议的其他设置（ **isEntryExitAnnounced** 属性），并允许在会议中使用特定演示者（ **allowedPresenters** 属性）。

### <a name="devices-and-apps--cloud-printing"></a>设备和应用 | 云打印
- [应用 `$expand` [OData 系统查询选项](/graph/api/printer-list-jobs?view=graph-rest-beta&preserve-view=true#optional-query-parameters)获取每个与打印机相关联的打印作业的文档](/graph/api/printer-list-jobs?view=graph-rest-beta&preserve-view=true)。 
- 应用 `$filter` [OData 系统查询选项](/graph/api/printer-list-jobs?view=graph-rest-beta&preserve-view=true#optional-query-parameters)筛选创建打印作业的用户。

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理
Intune beta 版[ 9 月](changelog.md#september-2020)更新。

### <a name="identity-and-access--directory-management"></a>身份和访问 | 目录管理
- [代表登录的用户（设备所有者或相应的角色）获取 BitLocker 恢复密钥](/graph/api/bitlockerrecoverykey-get?view=graph-rest-beta&preserve-view=true)。 获取恢复密钥会生成与最终用户体验存在奇偶校验的[审核日志](/azure/active-directory/reports-monitoring/concept-audit-logs)。
- 通过 **directorySizeQuota** 属性，获得 [组织](/graph/api/resources/organization?view=graph-rest-beta&preserve-view=true)的 [目录配额](/graph/api/resources/directorysizequota?view=graph-rest-beta&preserve-view=true)的总量和已使用量。

### <a name="identity-and-access--governance"></a>身份和访问 | 治理
在请求或删除 [给用户的访问权限包](/graph/api/resources/accesspackageassignment?view=graph-rest-beta&preserve-view=true)（用于指定对组、应用程序或 Microsoft Office SharePoint Online 网站的访问权限）时，可包括[计划](/graph/api/resources/requestschedule?view=graph-rest-beta&preserve-view=true)。

### <a name="identity-and-access--identity-and-sign-in"></a>身份和访问 | 身份和登录
组织可[获取](/graph/api/continuousaccessevaluationpolicy-get?view=graph-rest-beta&preserve-view=true)或[更新](/graph/api/continuousaccessevaluationpolicy-update?view=graph-rest-beta&preserve-view=true)[持续存取评估策略](/graph/api/resources/continuousAccessEvaluationPolicy?view=graph-rest-beta&preserve-view=true) 来实时管理身份验证会话。

### <a name="search"></a>搜索

- 在[适用于 OneDrive、SharePoint、Microsoft Graph 连接器的 Microsoft 搜索 API](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true) 中使用其他功能： 

  - 获取来自 OneDrive 和 SharePoint 的 [附加类型](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true#scope-search-based-on-entity-types)内容： **驱动器** 、 **列表** 、 **listItem** 和 **网站** 。 
  - 搜索结果中的范围属性设为[所选属性](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true#get-selected-properties)。 
  - 获取 [listItem](/graph/api/resources/listitem?view=graph-rest-beta&preserve-view=true) 资源的自定义属性。
  - 对任何可排序属性上的 OneDrive 和 SharePoint 搜索结果进行[排序](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true#sort-search-results)。
  - [使用针对 OneDrive 和 SharePoint 的聚合](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true#refine-results-using-aggregations)优化结果。
- 查询通过 Microsoft Graph 连接器跨越[多个连接](./search-concept-custom-types.md)摄取的外部数据。
- 充分利用 Microsoft Graph 连接器的增强内容，了解：
  - [管理连接](search-index-manage-connections.md)
  - [管理架构](search-index-manage-schema.md)
  - [管理项目](search-index-manage-items.md)
- 跟踪 Microsoft Graph [连接](/graph/api/resources/externalconnection?view=graph-rest-beta&preserve-view=true)的状态。
- 定义[外部组](/graph/api/resources/externalgroup?view=graph-rest-beta&preserve-view=true)以设置添加到 Microsoft Graph [连接](/graph/api/resources/externalconnection?view=graph-rest-beta&preserve-view=true)的[外部项目](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) 对象的权限。 外部组可以表示非 Azure Active Directory 组或类似组的构造（例如业务单元），它们确定对外部数据源中的内容的权限。

### <a name="teamwork"></a>团队合作
- 获取 Teams [频道](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true)或[团队](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true)的创建日期/时间。


## <a name="want-to-stay-in-the-loop"></a>保持循环

我们可以通过以下方式进行参与：

- 是否有希望 Microsoft Graph 支持的方案？ 在 [Microsoft Graph 用户心声](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)中建议新功能并进行投票。
    某些新功能来源于开发人员社区的热门请求。 Microsoft Graph 团队会定期评估客户需求，并按以下顺序发布新功能：

    1. 处于 **_预览_** 状态的 Debut。 任何相关的 REST API 更新都在 beta 终结点 (`https://graph.microsoft.com/beta`) 中。  

    2. 如果有足够的反馈表明具有可行性，则提升为 **_正式发布_ (GA)** 状态。 任何相关的 REST API 更新都添加到 v1.0 终结点 (`https://graph.microsoft.com/v1.0`)。 
- 成为 Microsoft Graph 社区中的活跃成员! [参与](https://aka.ms/microsoftgraphcall)Microsoft Graph 社区每月通话。
- 注册 [Microsoft 365 开发人员计划](https://developer.microsoft.com/office/dev-program)，免费订阅 Microsoft 365, 然后开始开发! 


## <a name="see-also"></a>另请参阅
- 定期查看 [Microsoft Graph 开发人员博客](https://developer.microsoft.com/graph/blogs/), 了解发布公告和有帮助的资源。 
- 浏览 Microsoft Graph API 新增功能的详细信息, 以及[changelog](changelog.md)中的 API 行为更新。
- 查找[早期版本的重点内容](whats-new-earlier.md)。
- 了解有关 [Microsoft Graph 的版本控制、支持和中断性变更策略](versioning-and-support.md)。
