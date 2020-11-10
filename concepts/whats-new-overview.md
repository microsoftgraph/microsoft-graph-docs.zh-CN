---
title: Microsoft Graph 新增功能
description: Microsoft Graph 新增功能
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: c0399ce4b171224225c570e88b9fbd094e9d2c8d
ms.sourcegitcommit: 4e7830a22b440bbbcfa795937af85d8542e5525b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48982693"
---
# <a name="whats-new-in-microsoft-graph"></a>Microsoft Graph 新增功能

查看 Microsoft Graph 中的最近两个月新增功能要点、[以前增加的内容](whats-new-earlier.md)以及如何[分享你的想法](#want-to-stay-in-the-loop)。 有关 API 级更新的详细列表，请参见 [API更改日志](changelog.md)。 

> [!IMPORTANT]
> _预览_ 状态下的功能（包括 API 和工具）可能会发生更改，恕不另行通知，有些功能可能永远不会提升为正式发布 (GA) 状态。 不要在成品应用中使用预览功能。

## <a name="november-2020-new-and-generally-available"></a>2020年 11 月：新版本和正式版

### <a name="teamwork"></a>团队合作
- 特定资源 GA 允许（RSC）权限。 RSC 权限允许团队所有者向生产应用授予精确同意，以便访问和/或修改团队的特定数据，例如读取团队的设置，或者修改频道的名称、说明及其他设置。
- 适用于 [频道](/graph/api/resources/channel) 或频道内的邮件 Api 的 GA。 Api 包括：
  - [创建](/graph/api/conversationmember-add) 或 从频道中[删除](/graph/api/conversationmember-delete) 对话成员。
  - [更新频道中成员](/graph/api/conversationmember-update) 的角色。
  - 获取频道中的特定邮件或所有邮件。
  - 获取频道中的特定回复或所有回复。
  - [在频道中跟踪新增的或者已更新的邮件](/graph/api/chatmessage-delta)。

## <a name="november-2020-new-in-preview-only"></a>2020 年 11 月：仅限预览版的新增功能

### <a name="devices-and-apps--cloud-printing"></a>设备和应用 | 云打印
在 [打印任务定义](/graph/api/resources/printtaskdefinition?view=graph-rest-beta&preserve-view=true)上[订阅更改通知](webhooks.md)。

### <a name="search"></a>搜索
可以聚合数值或字符串类型的搜索结果，[Microsoft Graph 连接器](/microsoftsearch/connectors-overview)导入这些结果，并将其在[架构](/graph/api/resources/schema?view=graph-rest-beta&preserve-view=true)中设置为可精简。 查看更多有关 [使用聚合优化搜索结果](search-concept-aggregation.md)的详细信息。

## <a name="october-2020-new-and-generally-available"></a>2020年 10 月：新版本和正式版

### <a name="application"></a>应用程序
- 使用[主页领域发现](/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#home-realm-discovery)策略，允许将[电子邮件作为 Azure AD 的备用登录 ID](/azure/active-directory/authentication/howto-authentication-use-email-signin)。 当用户提供登录 ID 后，无论是否提示用户进行身份验证，主页领域发现策略都会确定。 在这种情况下，设置 [homeRealmDiscoveryPolicy](/graph/api/resources/homerealmdiscoverypolicy) 资源的 **AlternateIdLogin** 属性，可使用户使用电子邮件地址登录。
- 获取 [应用程序](/graph/api/resources/application)或 [servicePrincipal](/graph/api/resources/serviceprincipal) 的经过验证的发布者信息，并为 **应用程序**[设置](/graph/api/application-setverifiedpublisher)或 [删除](/graph/api/application-unsetverifiedpublisher)经过验证的发布者信息。

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
