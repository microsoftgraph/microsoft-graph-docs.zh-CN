---
title: Microsoft Graph 新增功能
description: 查看过去两个月 Microsoft Graph 中的新增功能、早期版本中添加的内容以及如何分享你的想法的亮点。
author: angelgolfer-ms
ms.localizationpriority: high
ms.openlocfilehash: 9faaf3d0db85a040bbb65b21896819dfb59e1ee4
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66444227"
---
# <a name="whats-new-in-microsoft-graph"></a>Microsoft Graph 新增功能

查看 Microsoft Graph 中的最近两个月新增功能要点、[以前增加的内容](whats-new-earlier.md)以及如何[分享你的想法](#want-to-stay-in-the-loop)。 有关 API 级更新的详细列表，请参见 [API更改日志](https://developer.microsoft.com/graph/changelog/)。 

> [!IMPORTANT]
> 处于 _预览_ 状态的功能（包括 API 和工具）可能会发生更改，恕不另行通知，有些功能可能永远不会提升为正式发布 (GA) 状态。不要在生产应用中使用预览功能。

## <a name="june-2022-new-and-generally-available"></a>2022 年 6 月：新版本和正式发布版本

### <a name="cloud-communications--call-records"></a>云通信 | 通话记录
在 [获取呼叫记录](/graph/api/callrecords-callrecord-get) 并展开 [会话](/graph/api/resources/callrecords-session) 的每个 [区段](/graph/api/resources/callrecords-segment) 时，获取有关 [媒体流](/graph/api/resources/callrecords-mediastream) 的音频编解码器、视频编解码器、网络传输协议和跟踪路由跃点的信息。

### <a name="identity-and-access--directory-management"></a>身份和访问 | 目录管理
- [列出管理单元](/graph/api/device-list-memberOf)（[设备](/graph/api/resources/device)所属）。
- 将设备作为 [管理单元](/graph/api/resources/administrativeunit) 中的成员进行管理：[列出成员](/graph/api/administrativeunit-list-members)（包括设备），并 [获取](/graph/api/administrativeunit-get-members)、[添加](/graph/api/administrativeunit-post-members) 和 [删除](/graph/api/administrativeunit-delete-members) 作为成员的设备。 

### <a name="identity-and-access--identity-and-sign-in"></a>身份和访问 | 身份和登录
 配置和管理租户中 [临时访问通行证身份验证方法策略的设置](/graph/api/resources/temporaryAccessPassAuthenticationMethodConfiguration)。

### <a name="reports--microsoft-365-usage-reports"></a>报告 | Microsoft 365 使用情况报告
- 在由以下方法生成的 Teams 报表中查找新列：
  - [getTeamsUserActivityCounts](/graph/api/reportroot-getteamsuseractivitycounts)
  - [getTeamsUserActivityUserDetail](/graph/api/reportroot-getTeamsUserActivityUserDetail)
  - [getTeamsDeviceUsageUserDetail](/graph/api/reportroot-getTeamsDeviceUsageUserDetail)
  - [getTeamsDeviceUsageUserCounts](/graph/api/reportroot-getteamsdeviceusageusercounts)
  - [getTeamsDeviceUsageDistributionUserCounts](/graph/api/reportroot-getTeamsDeviceUsageDistributionUserCounts)
- 已弃用以下方法生成的 Teams 报表中的 Windows Phone 列：
  - [getTeamsDeviceUsageUserCounts](/graph/api/reportroot-getteamsdeviceusageusercounts)
  - [getTeamsDeviceUsageDistributionUserCounts](/graph/api/reportroot-getTeamsDeviceUsageDistributionUserCounts)


### <a name="teamwork"></a>Teamwork
在 Teams 中订阅以下内容的更改通知：
- [团队和频道](teams-changenotifications-team-and-channel.md)
- [团队和频道成员身份](teams-changenotifications-teammembership.md)
- [聊天](teams-changenotifications-chat.md)
- [聊天成员身份](teams-changenotifications-chatmembership.md)

## <a name="june-2022-new-in-preview-only"></a>2022 年 6 月：新增功能（仅限预览版）

### <a name="compliance--ediscovery"></a>合规性 | 电子数据展示
从 [安全](/graph/api/resources/security-api-overview?view=graph-rest-beta&preserve-view=true) 命名空间（而不是符合性命名空间）访问 [电子数据展示 API](/graph/api/resources/security-ediscoverycase?view=graph-rest-beta&preserve-view=true)。

### <a name="education"></a>教育
- 为 [分配](/graph/api/resources/educationassignment?view=graph-rest-beta&preserve-view=true) [创建](/graph/api/educationassignment-setupfeedbackresourcesfolder?view=graph-rest-beta&preserve-view=true) SharePoint 文件夹，以上传反馈文档。
- 在与分配关联的反馈文件夹中 [创建](/graph/api/educationfeedbackresourceoutcome-post-outcomes?view=graph-rest-beta&preserve-view=true) [提交](/graph/api/resources/educationsubmission?view=graph-rest-beta&preserve-view=true) 的 [反馈文档](/graph/api/resources/educationFeedbackResourceOutcome?view=graph-rest-beta&preserve-view=true)。

### <a name="identity-and-access--directory-management"></a>身份和访问 | 目录管理
将已验证的子域 [升级](/graph/api/domain-promote?view=graph-rest-beta&preserve-view=true) 为根域。

### <a name="identity-and-access--identity-and-sign-in"></a>身份和访问 | 身份和登录
隐藏租户登录页的 [登录页文本可见性设置](/graph/api/resources/loginpagetextvisibilitysettings?view=graph-rest-beta&preserve-view=true) 中的自助式密码重置 (SSPR) 链接。


## <a name="may-2022-new-and-generally-available"></a>2022 年 5 月：新版本和正式版

### <a name="education"></a>教育
- [跟踪分配资源的更改](/graph/api/educationassignment-delta)。
- [跟踪分配类别资源的更改](/graph/api/educationcategory-delta)。

### <a name="identity-and-access--directory-management"></a>身份和访问 | 目录管理
在 Azure Active Directory (Azure AD) 中注册的[应用程序](/graph/api/resources/application)可以指定服务或资产管理数据库中的应用程序或服务联系人信息。

### <a name="identity-and-access--identity-and-sign-in"></a>身份和访问 | 身份和登录
允许 Azure Active Directory (Azure AD)租户设置 [与另一个标识提供程序(IdP)支持 SAML 或 WS-Fed 协议的组织联盟](/graph/api/resources/samlOrWsFedExternalDomainFederation)。 这使得 Azure AD 租户能够允许来宾用户访问其资源。

### <a name="search"></a>搜索
对于 [搜索请求](/graph/api/resources/searchrequest)，每页最多可指定 1000 个搜索结果。

### <a name="sites-and-lists"></a>网站和列表
- 通过使用 [getCompatibleHubContentTypes](/graph/api/contenttype-getcompatiblehubcontenttypes)操作，从内容类型中心获取兼容的 [内容类型](/graph/api/resources/contentType) 资源集合。 
- 使用 [addCopyFromContentTypeHub](/graph/api/contenttype-addcopyfromcontenttypehub) 操作，将内容类型从内容类型中心添加或同步到 [网站](/graph/api/resources/site) 或 [列表](/graph/api/resources/list)。 这使得内容类型或其更新可用于需要它的特定站点或列表。 这是对传统同步基础结构的一项改进，后者将内容类型推送到整个组织中的所有站点，从而减少了发布传播的等待时间。 
- 获取一个或多个在站点或列表上发生的[丰富的长时间运行的操作](/graph/api/resources/richlongrunningoperation)，在同步添加内容类型时可能会发生这种情况。

### <a name="tasks-and-plans"></a>任务和计划
- [获取](/graph/api/plannerplandetails-get)或[更新](/graph/api/plannerplandetails-update)作为[计划](/graph/api/resources/plannerplan)[详细信息](/graph/api/resources/plannerplandetails)的一部分的类别描述。
- 使用 [计划容器](/graph/api/resources/plannerplancontainer)的 **类型** 属性来指定授权规则和 **计划** 的生存期，而不是 **计划** 的 **所有者** 属性。
- 获取[任务](/graph/api/resources/plannerTask)的优先级。

### <a name="teamwork"></a>Teamwork
[获取频道上的消息](/graph/api/channel-list-messages)，并包含对消息 [的任何答复](/graph/api/channel-list-messages#example-3-request-with-top-and-expand-query-options-on-replies)。

### <a name="to-do-tasks"></a>待办任务
- 将复杂的 [待办事项任务](/graph/api/resources/todotask) 分解为更具可操作性的小型任务，每个任务都是一个 [清单项](/graph/api/resources/checklistitem)。
- 使用用户定义的 [类别](/graph/api/resources/outlookcategory) 标记待办事项任务，以便对 Outlook 联系人、事件、消息、组帖子、待办事项任务进行分组。


## <a name="may-2022-new-in-preview-only"></a>2022 年 5 月：仅限预览版中的新增功能

### <a name="application"></a>应用程序
为本地应用程序配置 Azure AD 应用程序代理以实现安全的远程访问时，请使用 [onPremisesPublishing](/graph/api/resources/onPremisesPublishing?view=graph-rest-beta&preserve-view=true) 资源中的 **isStateSessionEnabled** 属性，指定如果应用程序使用 OAuth 2.0 授权代码授予流，是否验证状态参数。设置此属性有助于管理员保护应用，以避免出现跨网站请求伪造 (CSRF)。

### <a name="compliance--subject-rights-requests"></a>合规性 | 主体权限请求
- 指定或获取应在[使用者权限请求](/graph/api/resources/subjectRightsRequest?view=graph-rest-beta&preserve-view=true)中搜索的位置，例如[邮箱](/graph/api/resources/subjectRightsRequestAllMailboxLocation?view=graph-rest-beta&preserve-view=true)、[SharePoint、OneDrive 或 Teams 频道](/graph/api/resources/subjectRightsRequestAllSiteLocation?view=graph-rest-beta&preserve-view=true)。
- 指定或获取应用于在使用者权限请求中搜索的基于 KQL 的内容查询。

### <a name="device-and-app-management--cloud-pc"></a>设备和应用管理|云电脑
- [批量重新设置云电脑设备](/graph/api/manageddevice-bulkReprovisionCloudPc?view=graph-rest-beta&preserve-view=true)时获取明确定义的[结果](/graph/api/resources/cloudpcbulkremoteactionresult?view=graph-rest-beta&preserve-view=true)。
- [获取](/graph/api/manageddevice-getcloudpcreviewstatus?view=graph-rest-beta&preserve-view=true)或[设置](/graph/api/manageddevice-setcloudpcreviewstatus?view=graph-rest-beta&preserve-view=true)[云电脑审查状态](/graph/api/resources/cloudpcreviewstatus?view=graph-rest-beta&preserve-view=true)，或为多个设备[批量设置云电脑审查状态](/graph/api/manageddevice-bulksetcloudpcreviewstatus?view=graph-rest-beta&preserve-view=true)。

### <a name="device-and-app-management--multi-tenant-management"></a>设备和应用管理|多租户管理
[获取](/graph/api/managedtenants-managedtenant-list-tenantusage?view=graph-rest-beta&preserve-view=true)托管租户中每个服务的每月活跃用户数。

### <a name="education"></a>教育
使用与已安装的 Microsoft Teams 应用相对应的 [Teams 应用资源](/graph/api/resources/educationteamsappresource?view=graph-rest-beta&preserve-view=true)，使教育服务用户能够使用嵌入式 Teams 应用程序（如 YouTube 或 FlipGrid）创建和共享作业。

### <a name="identity-and-access--directory-management"></a>身份和访问 | 目录管理
[为组织](/graph/api/organization-activateService?view=graph-rest-beta&preserve-view=true) 和 [为用户](/graph/api/user-activateServicePlan?view=graph-rest-beta&preserve-view=true) 激活服务已弃用，并将在 2022 年 6 月 30 日停止返回数据。

### <a name="identity-and-access--identity-and-sign-in"></a>身份和访问 | 身份和登录
[授权策略](/graph/api/resources/authorizationPolicy?view=graph-rest-beta&preserve-view=true)的[默认用户角色](/graph/api/resources/defaultuserrolepermissions?view=graph-rest-beta&preserve-view=true)可以指定设备的注册所有者是否可以读取自己的 BitLocker 恢复密钥。

### <a name="reports--identity-and-access-reports"></a>报告 | 身份和访问报告
获取 [用户的注册身份验证方法使用报告](/graph/api/resources/userregistrationdetails?view=graph-rest-beta&preserve-view=true)，其中包括适用于多重身份验证的默认方法。

### <a name="search--index"></a>搜索 | 索引
[获取](/graph/api/externalconnectors-connectionquota-get?view=graph-rest-beta&preserve-view=true)[连接](/graph/api/resources/externalconnectors-externalconnection?view=graph-rest-beta&preserve-view=true)的[配额信息](/graph/api/resources/externalconnectors-connectionQuota?view=graph-rest-beta&preserve-view=true)。此信息包括可以引入到连接中的项数，并包括连接中剩余的项目，及其所有连接的租户级剩余配额。

### <a name="sites-and-lists"></a>网站和列表
[跟踪 SharePoint 列表项资源的更改](/graph/api/listitem-delta?view=graph-rest-beta&preserve-view=true)。

### <a name="teamwork"></a>团队合作
- 使用应用程序权限[获取指定用户参与的所有聊天](/graph/api/chat-list?view=graph-rest-beta&preserve-view=true)，而无需该用户在场。
- [向多个用户批量发送活动源通知](/graph/api/teamwork-sendActivityNotificationToRecipients?view=graph-rest-beta&preserve-view=true)，一次最多 100 个用户。

### <a name="to-do-tasks"></a>待办任务
从 2022 年 5 月 31 日开始，[基于 baseTask 构建的待办事项 API 集](/graph/api/resources/tasks-overview?view=graph-rest-beta&preserve-view=true) 已弃用。 该 API 集将于 2022 年 8 月 31 日停止返回数据。 请改用 [在 todoTask 上构建的待办事项 API 集](/graph/api/resources/todo-overview?view=graph-rest-beta&preserve-view=true)。


## <a name="want-to-stay-in-the-loop"></a>保持循环

我们可以通过以下方式进行参与：

- 是否有希望 Microsoft Graph 支持的方案？ 在 [Microsoft 技术社区](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph)中建议新功能并进行投票。
    某些新功能来源于开发人员社区的热门请求。 Microsoft Graph 团队会定期评估客户需求，并按以下顺序发布新功能：

    1. 处于 **_预览_** 状态的 Debut。 任何相关的 REST API 更新都在 beta 终结点 (`https://graph.microsoft.com/beta`) 中。  

    2. 如果有足够的反馈表明具有可行性，则提升为 **_正式发布_ (GA)** 状态。 任何相关的 REST API 更新都添加到 v1.0 终结点 (`https://graph.microsoft.com/v1.0`)。 
- 成为 Microsoft Graph 社区中的活跃成员! [加入](https://aka.ms/m365-dev-call) 每周Microsoft 365平台社区通话。
- 注册 [Microsoft 365 开发人员计划](https://developer.microsoft.com/office/dev-program)，免费订阅 Microsoft 365, 然后开始开发! 


## <a name="see-also"></a>另请参阅
- 定期查看 [Microsoft Graph 开发人员博客](https://developer.microsoft.com/graph/blogs/), 了解发布公告和有帮助的资源。 
- 浏览 Microsoft Graph API 新增功能的详细信息, 以及[changelog](https://developer.microsoft.com/graph/changelog/)中的 API 行为更新。
- 查找[早期版本的重点内容](whats-new-earlier.md)。
- 了解有关 [Microsoft Graph 的版本控制、支持和中断性变更策略](versioning-and-support.md)。
