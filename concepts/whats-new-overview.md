---
title: Microsoft Graph 新增功能
description: Microsoft Graph 新增功能
author: angelgolfer-ms
ms.localizationpriority: high
ms.openlocfilehash: 96d68f14255178ad94bd9fdcc88c8358df018cff
ms.sourcegitcommit: a60e5e81cfa04b666a1df1111a1d91f6c11989e9
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/31/2022
ms.locfileid: "62282063"
---
# <a name="whats-new-in-microsoft-graph"></a>Microsoft Graph 新增功能

查看 Microsoft Graph 中的最近两个月新增功能要点、[以前增加的内容](whats-new-earlier.md)以及如何[分享你的想法](#want-to-stay-in-the-loop)。 有关 API 级更新的详细列表，请参见 [API更改日志](https://developer.microsoft.com/graph/changelog/)。 

> [!IMPORTANT]
> 处于 _预览_ 状态的功能（包括 API 和工具）可能会发生更改，恕不另行通知，有些功能可能永远不会提升为正式发布 (GA) 状态。不要在生产应用中使用预览功能。


## <a name="january-2022-new-and-generally-available"></a>2022 年 1 月: 新版本和正式版

### <a name="devices-and-apps--service-health-and-communications"></a>设备和应用|服务运行状况和通信
获取 [服务更新消息](/graph/api/resources/serviceupdatemessage) 中添加的 [服务公告附件](/graph/api/resources/serviceAnnouncementAttachment)。

### <a name="identity-and-access--governance"></a>标识和访问权限 | 治理
- 获取[访问评审审阅者](/graph/api/resources/accessreviewreviewer)资源的集合，这些资源用于定义与[访问审阅实例](/graph/api/resources/accessReviewInstance)联系的审阅者。
- 区分通过 [访问评审决策](/graph/api/resources/accessreviewinstancedecisionitem) 表示其访问权限的 3 种类型的资源:
  - [访问包分配策略](/graph/api/resources/accessReviewInstanceDecisionItemAccessPackageAssignmentPolicyResource) 访问权限由访问评审决策确定。
  - [Azure 资源角色](/graph/api/resources/accessReviewInstanceDecisionItemAzureRoleResource) 访问权限由访问评审决策确定。
  - [服务主体](/graph/api/resources/accessReviewInstanceDecisionItemServicePrincipalResource) 对资源的访问权限由访问评审决策决定。

### <a name="identity-and-access--identity-and-sign-in"></a>标识和访问权限 | 标识和登录
强制执行 [会话控制](/graph/api/resources/conditionalAccessSessionControls) (通过设置 **disableResilienceDefaults** 属性) 来确定 Azure AD 是否应根据中断前收集的信息扩展现有会话。

### <a name="teamwork"></a>Teamwork
使用应用程序权限 [创建聊天](/graph/api/chat-post)。

## <a name="january-2022-new-in-preview-only"></a>2022 年 1 月: 仅限预览版新增功能

### <a name="compliance--ediscovery"></a>合规性 | 电子数据展示
获取保管人的 OneDrive for Business 站点的 URL ([userSource](/graph/api/resources/ediscovery-userSource?view=graph-rest-beta&preserve-view=true) 的 **siteWebUrl** 属性)。

### <a name="devices-and-apps--cloud-pc"></a>设备和应用 | 云电脑
- 获取或更新 [组织的设置](/graph/api/resources/cloudpcorganizationsettings?view=graph-rest-beta&preserve-view=true)，其中包括要在云电脑上预配的 Windows 操作系统版本，以及预配的云电脑上的用户帐户类型。
- [在指定的云电脑上更改用户帐户类型](/graph/api/cloudPC-changeUserAccountType?view=graph-rest-beta&preserve-view=true)。

### <a name="identity-and-access--governance"></a>标识和访问权限 | 治理
- 访问评审的审阅者可以 [记录](/graph/api/accessreviewinstancedecisionitem-recordalldecisions?view=graph-rest-beta&preserve-view=true) 当前用户为审阅者的决策。
- 配置 [用户作为见解最后一次登录的日期和时间](/graph/api/resources/userLastSignInRecommendationInsightSetting?view=graph-rest-beta&preserve-view=true)，以帮助审查员对 [访问审查时间表的定义](/graph/api/resources/accessreviewscheduledefinition?view=graph-rest-beta&preserve-view=true) 做出决定。
- 配置在 [审查实例中对用户或委托人访问权限决定](/graph/api/resources/accessreviewinstancedecisionitem?view=graph-rest-beta&preserve-view=true) 见解时的 [用户最后登录日期和时间](/graph/api/resources/userSignInInsight?view=graph-rest-beta&preserve-view=true)。
- 访问包的请求者可以提供自定义信息作为 [访问包资源](/graph/api/resources/accesspackageresource?view=graph-rest-beta&preserve-view=true) 的一部分，这些资源可用于为访问包做出审批决策。
- 请求者可以在 [访问包分配策略](/graph/api/resources/accesspackageassignmentpolicy?view=graph-rest-beta&preserve-view=true) 中编辑 [问题](/graph/api/resources/accessPackageQuestion?view=graph-rest-beta&preserve-view=true) 的答案。

### <a name="reports--identity-and-access-reports"></a>报告 | 身份和访问报告
- 获取 [为用户注册的身份验证方法](/graph/api/resources/userRegistrationDetails?view=graph-rest-beta&preserve-view=true) 的详细信息，例如多重身份验证、自助式密码重置和无密码身份验证。
- 为组织中的用户或应用程序的 [登录](/graph/api/resources/signIn?view=graph-rest-beta&preserve-view=true) 事件获取以下属性: 
  - 任何有条件的访问 [认证环境](/graph/api/resources/authenticationContext?view=graph-rest-beta&preserve-view=true)。
  - 任何有条件的访问 [会话寿命策略](/graph/api/resources/sessionLifetimePolicy?view=graph-rest-beta&preserve-view=true)。
  - 登录期间访问的 Azure 资源的 ID。
  - 应用程序的联合标识凭据 (如果用于登录) 的标识符。
  - 在登录事件中代表目标资源的服务主体标识符。

### <a name="reports--microsoft-365-usage-reports"></a>报告 | Microsoft 365 使用情况报告
获取美国政府 Microsoft Cloud 的 Outlook、OneDrive 和 SharePoint 使用情况报告。 请参阅 [云部署](/graph/api/resources/report?view=graph-rest-beta&preserve-view=true#cloud-deployments) 的摘要。

### <a name="sites-and-lists"></a>网站和列表
- 使用 [addCopyFromContentTypeHub](/graph/api/contenttype-addcopyfromcontenttypehub?view=graph-rest-beta&preserve-view=true) 操作，将内容类型从内容类型中心添加或同步到 [网站](/graph/api/resources/site?view=graph-rest-beta&preserve-view=true) 或 [列表](/graph/api/resources/list?view=graph-rest-beta&preserve-view=true)。 这使得内容类型或其更新可用于需要它的特定站点或列表。 这是对传统同步基础结构的一项改进，后者将内容类型推送到整个组织中的所有站点，从而减少了发布传播的等待时间。 
- 获取一个或多个在站点或列表上发生的 [丰富的长时间运行的操作](/graph/api/resources/richlongrunningoperation?view=graph-rest-beta&preserve-view=true)，这在同步添加内容类型时可能发生。
- 通过使用 [getCompatibleHubContentTypes](/graph/api/contenttype-getcompatiblehubcontenttypes?view=graph-rest-beta&preserve-view=true)操作，从内容类型中心获取兼容的 [内容类型](/graph/api/resources/contentType?view=graph-rest-beta&preserve-view=true) 资源集合。 

### <a name="teamwork"></a>Teamwork
- 允许用户 [在列出聊天中的消息](/graph/api/chat-list-messages?view=graph-rest-beta&preserve-view=true) 时选择 **LastModifiedDateTime** 或 **CreatedDateTime** 作为排序顺序。
- 当机器人代表用户发送 [聊天消息](/graph/api/resources/chatmessage?view=graph-rest-beta&preserve-view=true) 时，请指定用户属性 (在 **onBehalfOf** 属性中)。
- 将以下类型的成员添加到 [聊天](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true) 中:
  - [匿名来宾](/graph/api/resources/anonymousGuestConversationMember?view=graph-rest-beta&preserve-view=true)
  - [Microsoft 账户用户](/graph/api/resources/microsoftAccountUserConversationMember?view=graph-rest-beta&preserve-view=true)
  - [Skype for Business 用户](/graph/api/resources/skypeForBusinessUserConversationMember?view=graph-rest-beta&preserve-view=true)
  - [Skype 用户](/graph/api/resources/skypeUserConversationMember?view=graph-rest-beta&preserve-view=true)

## <a name="december-2021-new-and-generally-available"></a>2021 年 12 月：新增功能并正式发布

### <a name="cloud-communications--presence"></a>云通信 | 预览版
对指定用户的[状态](/graph/api/resources/presence)[订阅更改通知](/graph/api/subscription-post-subscriptions)。 始终在订阅请求中指定加密证书，因为这些是[包含加密资源数据的丰富通知](webhooks-with-resource-data.md)。


### <a name="compliance--subject-rights-requests"></a>合规性 | 主体权限请求
作为 [Microsoft 365 隐私管理](/privacy/solutions/privacymanagement/privacy-management?view=o365-worldwide&preserve-view=true)的一部分，[主体权限请求 API](/graph/api/resources/subjectrightsrequest) 在 Microsoft Graph 的 v1 和 Beta 版终结点中首次推出。 该 API 允许用户请求查看或管理其组织中的个人数据。 此外，它还允许组织自动执行和扩展管理这些请求，帮助它们更有效地满足行业法规。

### <a name="customer-booking"></a>客户预订
在生产应用中使用适用于 Microsoft Bookings 的 API，并使用以下新功能和更新：
- 通过短信通知你在美国或加拿大的客户[预约](/graph/api/resources/bookingappointment)或是与预约相关联的具体[服务](/graph/api/resources/bookingservice)。
- 为服务启用联机会议，并自动生成预约的 Microsoft Teams 会议链接。
- 允许一个或多个客户参加小组预约，设置服务和预约的最大与会者计数，并跟踪预约中的实际与会者计数。
- 为[企业](/graph/api/resources/bookingbusiness)创建[自定义问题](/graph/api/resources/bookingcustomquestion)，将问题与选项进行关联，将其指定为服务的必需选项，并跟踪预约中的问题和答案。
- 获取或设置预约中的客户或[员工成员](/graph/api/resources/bookingstaffmember)的时区。
- 获取或设置[客户](/graph/api/resources/bookingcustomer)的位置和电话号码。
- 从新的终结点 `https://graph.microsoft.com/v1.0/solutions/` 访问 v1 API。 请注意，Beta API 保留在 `https://graph.microsoft.com/beta` 终结点中。

### <a name="education"></a>教育
- 使用 **addToCalendarAction** 属性指定要添加到仅学生的日历的 [作业](/graph/api/resources/educationassignment)。
- 将带有反馈的[已提交的作业](/graph/api/resources/educationsubmission)[重新分配](/graph/api/educationsubmission-reassign)给学生供其查看。
- [列出 [educationUser](/graph/api/resources/educationuser) 的作业](/graph/api/educationuser-list-assignments)。 

### <a name="identity-and-access--governance"></a>标识和访问权限 | 治理
[更新](/graph/api/accessreviewinstance-update)[访问评审实例](/graph/api/resources/accessreviewinstance)的审阅者和回退审阅者。

### <a name="teamwork"></a>Teamwork
- 通过其 Web URL（通过 **webUrl** 属性）识别 Microsoft Teams 中的 [聊天](/graph/api/resources/chat)。
- 通过从 [chatMessage](/graph/api/resources/chatmessage) 或[聊天](/graph/api/resources/chat)访问 [eventMessageDetail](/graph/api/resources/EventMessageDetail) 来获取聊天、频道或团队中发生事件的详细信息。 例如，添加到频道或聊天的成员以及更新的团队说明。

## <a name="december-2021-new-in-preview-only"></a>2021 年 12 月：仅预览版新增功能

### <a name="cloud-communications--online-meetings"></a>云通信 | 联机会议
使用[外部注册[系统启用](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true)联机会议](/graph/api/resources/externalmeetingregistration?view=graph-rest-beta&preserve-view=true)注册。 

### <a name="cloud-communications--presence"></a>云通信 | 预览版
- 使用 [setUserPreferredPresence](/graph/api/presence-setuserpreferredpresence?view=graph-rest-beta&preserve-view=true) 操作可设置用户的首选空闲状态和活动状态。 用户状态将成为首选状态。
- 使用 [clearUserPreferredPresence](/graph/api/presence-clearuserpreferredpresence?view=graph-rest-beta&preserve-view=true) 操作可清除用户的任何首选空闲状态和活动状态。
- 将 `Presence.ReadWrite` 用作 [setPresence](/graph/api/presence-setpresence?view=graph-rest-beta&preserve-view=true)、 [clearPresence](/graph/api/presence-clearpresence?view=graph-rest-beta&preserve-view=true)、[setUserPreferredPresence](/graph/api/presence-setuserpreferredpresence?view=graph-rest-beta&preserve-view=true) 或 [clearUserPreferredPresence](/graph/api/presence-clearuserpreferredpresence?view=graph-rest-beta&preserve-view=true)的委派权限。
- 将 `Presence.ReadWrite.All` 用作 [setPresence](/graph/api/presence-setpresence?view=graph-rest-beta&preserve-view=true)、 [clearPresence](/graph/api/presence-clearpresence?view=graph-rest-beta&preserve-view=true)、[setUserPreferredPresence](/graph/api/presence-setuserpreferredpresence?view=graph-rest-beta&preserve-view=true) 或 [clearUserPreferredPresence](/graph/api/presence-clearuserpreferredpresence?view=graph-rest-beta&preserve-view=true)的应用程序权限。

### <a name="devices-and-apps--cloud-pc"></a>设备和应用 | 云电脑
- 管理员可以通过指定[云电脑预配策略](/graph/api/resources/cloudpcprovisioningpolicy?view=graph-rest-beta&preserve-view=true)中的设置，并配置云电脑的托管设备体验来启用 [Microsoft 托管桌面](/graph/api/resources/microsoftmanageddesktop?view=graph-rest-beta&preserve-view=true)。
- [重新启动](/graph/api/cloudpc-reboot?view=graph-rest-beta&preserve-view=true)[云电脑](/graph/api/resources/cloudpc?view=graph-rest-beta&preserve-view=true)。
- [重命名](/graph/api/cloudpc-rename?view=graph-rest-beta&preserve-view=true)以更新云电脑的显示名称。
- [排除故障](/graph/api/cloudpc-troubleshoot?view=graph-rest-beta&preserve-view=true)以检查云电脑和会话主机的运行状况。
- 通过 **lastRemoteActionResult** 属性跟踪云电脑上最近的远程操作结果，包括重启、重命名、重新设置、故障排除。
- 通过 **lastLoginResult** 属性跟踪云电脑最近的登录时间戳。
- 通过 **expirationDate** 属性跟踪 [云电脑](/graph/api/resources/cloudpcdeviceimage?view=graph-rest-beta&preserve-view=true)设备映像不可用的日期。
- 通过 **osStatus** 属性跟踪 [云电脑设备映像](/graph/api/resources/cloudpcdeviceimage?view=graph-rest-beta&preserve-view=true)中操作系统的状态。
- 为云电脑 RBAC 提供商[创建](/graph/api/rbacapplication-post-roledefinitions?view=graph-rest-beta&preserve-view=true)、[更新](/graph/api/unifiedroledefinition-update?view=graph-rest-beta&preserve-view=true)和[删除](/graph/api/unifiedroledefinition-delete?view=graph-rest-beta&preserve-view=true) [unifiedRoleDefinition](/graph/api/resources/unifiedroledefinition?view=graph-rest-beta&preserve-view=true) 对象。

### <a name="education"></a>教育
- [跟踪](delta-query-overview.md)对 [educationClass](/graph/api/resources/educationclass?view=graph-rest-beta&preserve-view=true) 和 [educationUser](/graph/api/resources/educationuser?view=graph-rest-beta&preserve-view=true) 资源的更改。
- 使用 **addToCalendarAction** 属性指定要添加到仅学生的日历的 [作业](/graph/api/resources/educationassignment)。

### <a name="identity-and-access--directory-management"></a>身份和访问 | 目录管理
- 通过 **认证** 属性 [获取](/graph/api/application-get?view=graph-rest-beta&preserve-view=true)[应用程序](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true)的认证详细信息。 仅当应用程序是通过 [Microsoft 365 应用符合性计划](/microsoft-365-app-certification/docs/enterprise-app-certification-guide)认证的时，才设置该属性。  
- 通过 [permissionGrantConditionSet](/graph/api/resources/permissionGrantConditionSet?view=graph-rest-beta&preserve-view=true) 的 **certifiedClientApplicationsOnly** 属性，将认证 [包含](/graph/api/permissiongrantpolicy-post-includes?view=graph-rest-beta&preserve-view=true)或 [排除](/graph/api/permissiongrantpolicy-post-excludes?view=graph-rest-beta&preserve-view=true)为 [权限授予策略](/graph/api/resources/permissiongrantpolicy?view=graph-rest-beta&preserve-view=true)中的一个 [条件](/graph/api/resources/permissionGrantConditionSet?view=graph-rest-beta&preserve-view=true)。

### <a name="search--index"></a>搜索 | 索引
使用[更新](/graph/api/externalconnectors-schema-update?view=graph-rest-beta&preserve-view=true)操作更新[连接](/graph/api/resources/externalconnectors-externalconnection?view=graph-rest-beta&preserve-view=true)架构中项目的属性，包括其别名和标签。

### <a name="teamwork"></a>Teamwork
- [列出](/graph/api/teams-list?view=graph-rest-beta&preserve-view=true)组织中的所有团队。

### <a name="to-do-tasks"></a>待办任务
- 若要预期能够在同一位置管理来自多个源的所有任务（如 Outlook 邮件、Teams 聊天、OneDrive 文档）：
  - 使用[最新的待办事项 API](/graph/api/resources/tasks-overview?view=graph-rest-beta&preserve-view=true)，然后从新终结点 `https://graph.microsoft.com/beta/me/tasks/` 进行访问。
  - 使用段 `allTasks` 获取用户的所有任务：`https://graph.microsoft.com/beta/me/tasks/alltasks`。
  - 区分内置任务列表列表（如“**已标记电子邮件**”或“**任务**”）和用户定义的任务列表。 内置任务列表由 [wellKnownTaskList](/graph/api/resources/wellknowntasklist?view=graph-rest-beta&preserve-view=true) 资源表示，用户定义的任务列表由 [taskList](/graph/api/resources/tasklist?view=graph-rest-beta&preserve-view=true) 资源表示。
  - 区分当前定义的任务类型、[任务](/graph/api/resources/task?view=graph-rest-beta&preserve-view=true)与基类型 [baseTask](/graph/api/resources/basetask?view=graph-rest-beta&preserve-view=true) 之间的区别。
- 将更复杂的[任务](/graph/api/resources/task?view=graph-rest-beta&preserve-view=true)分解为更小的、更可行的子任务。 每个子任务都由 [checklistItem](/graph/api/resources/checklistitem?view=graph-rest-beta&preserve-view=true) 资源表示。
- 在不同列表之间[移动](/graph/api/basetask-move?view=graph-rest-beta&preserve-view=true)任务。
- 有关更多详细信息，请参阅这篇[博客文章](https://devblogs.microsoft.com/microsoft365dev/announcing-the-public-preview-of-to-do-tasks-api/)，并将任何使用[更早版本的待办事项 API](/graph/api/resources/todo-overview?view=graph-rest-beta&preserve-view=true) 的现有应用迁移至[最新的待办事项 API](/graph/api/resources/tasks-overview?view=graph-rest-beta&preserve-view=true)。


## <a name="want-to-stay-in-the-loop"></a>保持循环

我们可以通过以下方式进行参与：

- 是否有希望 Microsoft Graph 支持的方案？ 在 [Microsoft 技术社区](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph)中建议新功能并进行投票。
    某些新功能来源于开发人员社区的热门请求。 Microsoft Graph 团队会定期评估客户需求，并按以下顺序发布新功能：

    1. 处于 **_预览_** 状态的初次发布。任何相关的 REST API 更新都在 Beta 终结点 (`https://graph.microsoft.com/beta`) 中。  

    2. 如果有足够的反馈表明具有可行性，则提升为 **_正式发布_ (GA)** 状态。 任何相关的 REST API 更新都添加到 v1.0 终结点 (`https://graph.microsoft.com/v1.0`)。 
- 成为 Microsoft Graph 社区中的活跃成员! [参与](https://aka.ms/microsoftgraphcall)Microsoft Graph 社区每月通话。
- 注册 [Microsoft 365 开发人员计划](https://developer.microsoft.com/office/dev-program)，免费订阅 Microsoft 365, 然后开始开发! 


## <a name="see-also"></a>另请参阅
- 定期查看 [Microsoft Graph 开发人员博客](https://developer.microsoft.com/graph/blogs/), 了解发布公告和有帮助的资源。 
- 浏览 Microsoft Graph API 新增功能的详细信息, 以及[changelog](https://developer.microsoft.com/graph/changelog/)中的 API 行为更新。
- 查找[早期版本的重点内容](whats-new-earlier.md)。
- 了解有关 [Microsoft Graph 的版本控制、支持和中断性变更策略](versioning-and-support.md)。
