---
title: Microsoft Graph 新增功能
description: Microsoft Graph 新增功能
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 5926d13f8971d891d48eb09205162f502999faed
ms.sourcegitcommit: 22bd45d272681658d46a8b99af3c3eabc7b05cb1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/18/2021
ms.locfileid: "58384469"
---
# <a name="whats-new-in-microsoft-graph"></a>Microsoft Graph 新增功能

查看 Microsoft Graph 中的最近两个月新增功能要点、[以前增加的内容](whats-new-earlier.md)以及如何[分享你的想法](#want-to-stay-in-the-loop)。 有关 API 级更新的详细列表，请参见 [API更改日志](https://developer.microsoft.com/graph/changelog/)。 

> [!IMPORTANT]
> 处于 _预览_ 状态的功能（包括 API 和工具）可能会发生更改，恕不另行通知，有些功能可能永远不会提升为正式发布 (GA) 状态。不要在生产应用中使用预览功能。

## <a name="august-2021-new-and-generally-available"></a>2021 年 8 月：新版本和正式版

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理
Intune v 1.0 版的每月更新。 设置 2021 年 8 月的 **日期** 筛选器，并查找具有相同标题的部分。

### <a name="devices-and-apps--service-health-and-communications"></a>设备和应用|服务运行状况和通信
使用 Microsoft Graph 中的[服务通信 API](service-communications-concept-overview.md) 访问有关 Microsoft 云服务的运行状况和消息中心帖子。

### <a name="identity-and-access--governance"></a>身份和访问 | 治理
获取访问评审范围的集合，这些范围用于定义[访问评审实例](/graph/api/resources/accessReviewInstance)的审阅者和回退审阅者。

## <a name="august-2021-new-in-preview-only"></a>2021 年 8 月：仅限预览版新增功能

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理
Intune beta 版每月更新。 设置 2021 年 8 月的 **日期** 筛选器，并查找具有相同标题的部分。

### <a name="identity-and-access--governance"></a>身份和访问 | 治理
- [重新处理](/graph/api/accesspackageassignmentrequest-reprocess?view=graph-rest-beta&preserve-view=true)[访问包分配请求](/graph/api/resources/accesspackageassignmentrequest?view=graph-rest-beta&preserve-view=true)以自动重试用户对包的访问请求。
- [重新处理](/graph/api/accesspackageassignment-reprocess?view=graph-rest-beta&preserve-view=true)[访问包分配](/graph/api/resources/accesspackageassignment?view=graph-rest-beta&preserve-view=true)以自动重新评估和强制执行用户分配。
- [获取一组策略要求](/graph/api/accesspackage-getapplicablepolicyrequirements?view=graph-rest-beta&preserve-view=true)以便[为访问包创建分配请求](/graph/api/resources/accesspackageassignmentrequestrequirements?view=graph-rest-beta&preserve-view=true)。
- 获取[访问评审审阅者](/graph/api/resources/accessreviewreviewer?view=graph-rest-beta&preserve-view=true)资源的集合，这些资源用于定义与[访问审阅实例](/graph/api/resources/accessReviewInstance?view=graph-rest-beta&preserve-view=true)联系的审阅者。
- 使用 **recommendationLookBackDuration** 属性，获取或设置在[访问评审的计划设置中](/graph/api/resources/accessReviewScheduleSettings?view=graph-rest-beta&preserve-view=true)配置建议的非活动持续时间。

### <a name="identity-and-access--identity-and-sign-in"></a>身份和访问 | 身份和登录
组织可以使用[策略来强制应用使用应用程序身份验证方法的最佳做法](/graph/api/resources/applicationauthmethodpolicy?view=graph-rest-beta&preserve-view=true)。 此类策略可以应用于[特定应用程序和服务主体](/graph/api/resources/appmanagementpolicy?view=graph-rest-beta&preserve-view=true)，或[租户中的所有应用程序和服务主体](/resources/tenantappmanagementpolicy?view=graph-rest-beta&preserve-view=true)。

## <a name="july-2021-new-and-generally-available"></a>2021 年 7 月: 新版本和正式版

### <a name="cloud-communications--calls"></a>云通信 | 呼叫
在采用 [基于 Teams 策略录制](/microsoftteams/teams-recording-policy) 的组织中，支持对应用程序在 [接听](/graph/api/call-answer) [通话](/graph/api/resources/call) 时可以处理的参与者数量容量限制。

### <a name="identity-and-access--identity-and-sign-in"></a>身份和访问 | 身份和登录
- 共享通用基类型 [identityProviderBase](/graph/api/resources/identityproviderbase) 的标识提供程序的正式版：
  - Azure AD 租户中 Azure AD B2B 方案的内置标识提供程序。 这些提供程序可以支持 Azure AD、Microsoft 帐户 (MSA) 或电子邮件一次性密码。
  - Azure AD B2C 租户中的社交标识提供程序允许用户使用社交媒体帐户（如 Microsoft、Google、Facebook、Amazon、LinkedIn 或 Twitter）注册和登录服务。
- 弃用早期[标识提供程序](/graph/api/resources/identityprovider) API。

### <a name="users"></a>用户
让用户 [更改自己的密码](/graph/api/user-changepassword) 而无需管理员角色。


## <a name="july-2021-new-in-preview-only"></a>2021 年 7 月: 预览版新增功能

### <a name="devices-and-apps--cloud-pc"></a>设备和应用 | 云电脑
本地连接 [运行状况检查](/graph/api/cloudpconpremisesconnection-runhealthcheck?view=graph-rest-beta&preserve-view=true) 可以识别更多可能的运行状况检查错误类型:
- 在组织单位 (`adJoinCheckComputerObjectAlreadyExists`) 中未找到云 PC 计算机帐户。
- 在 Azure AD (`azureAdDeviceSyncCheckDeviceNotFound`) 中未找到云 PC 对象。
- 检查云 PC 对象是否已同步到 Azure AD (`azureAdDeviceSyncCheckLongSyncCircle`) 时超时。 

详情和建议的补救措施见[参考文献](/graph/api/resources/cloudpconpremisesconnectionhealthcheck?view=graph-rest-beta&preserve-view=true#cloudpconpremisesconnectionhealthcheckerrortype-values)。

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理
Intune beta 版每月更新。 设置 2021 年 7 月的 **日期** 筛选器，并查找具有相同标题的部分。

### <a name="devices-and-apps--multi-tenant-management"></a>设备和应用|多租户管理
[Microsoft 365 Lighthouse API](managedtenants-concept-overview.md) 的首次亮相，使管理服务提供商 (MSP) 能够大规模地远程管理多个客户租户的合规性和威胁检测，并帮助使租户设备处于健康和安全状态。

### <a name="education"></a>教育
- 获取作为[学校数据同步状态](/graph/api/resources/educationsynchronizationprofilestatus?view=graph-rest-beta&preserve-view=true)一部分的错误计数和状态消息。
- 获取作为此类同步可能状态的 `extracting` 或 `validating`。

### <a name="identity-and-access--governance"></a>身份和访问 | 治理
获取[访问评审实例](/graph/api/resources/accessreviewinstance?view=graph-rest-beta&preserve-view=true)的生命周期中的错误集合。

### <a name="search"></a>搜索
- 使用 [Microsoft 搜索 API 检索与用户最相关人员](search-concept-person.md) 的信息。相关性由用户的通信和协作模式以及业务关系决定。 
- 访问 microsoft.graph.externalConnectors 子命名空间中的[连接器索引 API](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true)。

### <a name="teamwork"></a>团队合作
- [订阅聊天资源](teams-changenotifications-chat.md) 的更改通知。
- [订阅聊天中](teams-changenotifications-chatmembership.md)、[频道](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true) 中或 [团队](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true) 中用户的更改通知 (即，[conversationMember](/graph/api/resources/conversationmember?view=graph-rest-beta&preserve-view=true) 资源)。
- 通过从 [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta&preserve-view=true) 或[聊天](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true)访问 [eventMessageDetail](/graph/api/resources/EventMessageDetail?view=graph-rest-beta&preserve-view=true)，获取聊天、频道或团队中发生事件的详细信息。 例如，添加到频道或聊天的成员以及更新的团队说明。


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
