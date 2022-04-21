---
title: Microsoft Graph 新增功能
description: Microsoft Graph 新增功能
author: angelgolfer-ms
ms.localizationpriority: high
ms.openlocfilehash: 30119dbd92c3a1b8552f19857225d868d50dd03b
ms.sourcegitcommit: 0ae140eafaca2dddc4584930cc0ac27fb1731c61
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2022
ms.locfileid: "65017111"
---
# <a name="whats-new-in-microsoft-graph"></a>Microsoft Graph 新增功能

查看 Microsoft Graph 中的最近两个月新增功能要点、[以前增加的内容](whats-new-earlier.md)以及如何[分享你的想法](#want-to-stay-in-the-loop)。 有关 API 级更新的详细列表，请参见 [API更改日志](https://developer.microsoft.com/graph/changelog/)。 

> [!IMPORTANT]
> 处于 _预览_ 状态的功能（包括 API 和工具）可能会发生更改，恕不另行通知，有些功能可能永远不会提升为正式发布 (GA) 状态。不要在生产应用中使用预览功能。


## <a name="march-2022-new-and-generally-available"></a>2022 年 3 月：新增和正式发布

### <a name="files"></a>文件
使用 [捆绑包](/graph/api/resources/bundle) 资源一次共享多个文件，就像其他 [driveItem](/graph/api/resources/driveitem) 资源一样。 可以对捆绑包应用 CRUD 操作， [将](/graph/api/bundle-additem) 项添加到或 [从捆绑包中删除](/graph/api/bundle-removeitem) 项。

### <a name="identity-and-access--directory-management"></a>身份和访问 | 目录管理
使用 [特定于资源的权限](/graph/api/resources/resourcespecificpermission) 授权 Teams 应用直接访问聊天或团队的特定实例的数据。 例如，特定于资源的权限 ChannelMessage.Read.Group 允许 Teams 应用读取单个团队的频道消息。

### <a name="identity-and-access--governance"></a>身份和访问 | 治理
[获取](/graph/api/approval-get)与[访问包分配](/graph/api/resources/accesspackageassignmentrequest)的请求关联的[审批](/graph/api/resources/approval)决策。

### <a name="identity-and-access--identity-and-sign-in"></a>身份和访问 | 身份和登录
指定客户端应用程序[包含或排除](/graph/api/resources/conditionalaccessclientapplications)为应用[条件访问策略](/graph/api/resources/conditionalaccesspolicy)的一组[条件](/graph/api/resources/conditionalAccessConditionSet)。


## <a name="march-2022-new-in-preview-only"></a>2022 年 3 月：仅预览版中的新增功能

### <a name="cloud-communications--online-meeting"></a>云通信 | 联机会议
指定一个或多个 [会议参与者](/graph/api/resources/meetingParticipants?view=graph-rest-beta&preserve-view=true) 为共同组织者。

### <a name="device-and-app-management--cloud-pc"></a>设备和应用管理|云电脑
- 对[unifiedRoleDefinition](/graph/api/resources/unifiedroledefinition?view=graph-rest-beta&preserve-view=true)资源的读取操作使用`RoleManagement.Read.CloudPC`的委派权限或应用程序权限资源。
- 对[unifiedRoleDefinition](/graph/api/resources/unifiedroledefinition?view=graph-rest-beta&preserve-view=true)资源的读取和写入操作使用`RoleManagement.ReadWrite.CloudPC`的委派权限或应用程序权限资源。
- 指定 Azure 订阅的 ID 和显示名称，作为设备的[源映像信息](/graph/api/resources/cloudPcSourceDeviceImage?view=graph-rest-beta&preserve-view=true)的一部分。
- 指定 [Windows 设置](/graph/api/resources/cloudpcwindowssettings?view=graph-rest-beta&preserve-view=true) 在为 [预配策略创建云电脑时](/graph/api/resources/cloudPcProvisioningPolicy?view=graph-rest-beta&preserve-view=true)进行配置。

### <a name="device-and-app-management--corporate-management"></a>设备和应用管理|公司管理
- Intune 3 beta 版更新。

### <a name="device-and-app-management--multi-tenant-management"></a>设备和应用管理|多租户管理
[列出](/graph/api/managedtenants-managedtenant-list-auditevents?view=graph-rest-beta&preserve-view=true) 和 [获取 Microsoft 365 Lighthouse 中托管租户的](/graph/api/managedtenants-auditevent-get?view=graph-rest-beta&preserve-view=true) 审核事件。

### <a name="identity-and-access--directory-management"></a>身份和访问 | 目录管理
[列表](/graph/api/organizationsettings-list-microsoftapplicationdataaccess?view=graph-rest-beta&preserve-view=true)或[更新](/graph/api/microsoftapplicationdataaccesssettings-update?view=graph-rest-beta&preserve-view=true)[设置](/graph/api/resources/microsoftapplicationdataaccesssettings?view=graph-rest-beta&preserve-view=true)，这些设置指定从 Microsoft 应用程序访问Microsoft 365属于组织中用户的数据。 例如，如果授权正确，是否只有Microsoft 365应用（如 Word 和 Excel）才能访问用户的Microsoft 365数据，或者其他 Microsoft 应用（如 Windows）是否也可以访问数据。 默认情况下，组织中的所有用户都可以在 Microsoft 应用中访问用户有权访问的任何Microsoft 365数据。 

### <a name="security--attack-simulation-and-training"></a>安全 | 攻击模拟和训练
- [列出租户的模拟自动化](/graph/api/attacksimulationroot-list-simulationautomations?view=graph-rest-beta&preserve-view=true)。
- [列表为租户运行模拟自动化](/graph/api/resources/simulationautomationrun?view=graph-rest-beta&preserve-view=true)。

### <a name="search"></a>搜索
- 在 [搜索请求中指定](/graph/api/resources/searchrequest?view=graph-rest-beta&preserve-view=true) 是否从搜索结果中剪裁重复的 SharePoint 文件。 默认值为 false。
- 使用支持 KQL 和查询变量的模板限定 [搜索查询](/graph/api/resources/searchquery?view=graph-rest-beta&preserve-view=true) 字符串。

### <a name="sites-and-lists"></a>网站和列表
对于包含分类数据的 [列](/graph/api/resources/columnDefinition?view=graph-rest-beta&preserve-view=true) ，请指定父 [术语](/graph/api/resources/termstore-term?view=graph-rest-beta&preserve-view=true) 和 [术语集](/graph/api/resources/termstore-set?view=graph-rest-beta&preserve-view=true) ，子术语可选为列值。

### <a name="tasks-and-plans"></a>任务和计划
通过检查相应 [plannerPlan](/graph/api/resources/plannerPlan?view=graph-rest-beta&preserve-view=true)资源关系的 **详细信息** 关系，确定用于 Planner 外部体验的 Planner 计划（如 Microsoft Teams）能否跟踪该上下文中的工作。

### <a name="teamwork"></a>Teamwork
- 获取或设置有关[团队](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true)的[摘要信息](/graph/api/resources/teamSummary?view=graph-rest-beta&preserve-view=true)，包括所有者、成员和来宾的计数。
- 在聊天中[列出消息](/graph/api/chat-list-messages?view=graph-rest-beta&preserve-view=true)时，按降序对邮件进行排序。


## <a name="february-2022-new-and-generally-available"></a>2022 年 2 月：新版本和正式版

### <a name="teamwork"></a>Teamwork
通过 **onlineMeetingInfo** 属性获取与 [聊天](/graph/api/resources/chat)关联的 [联机会议的详细信息](/graph/api/resources/teamworkOnlineMeetingInfo)。

## <a name="february-2022-new-in-preview-only"></a>2022 年 2 月：仅限预览版中的新增功能

### <a name="applications"></a>应用程序
- 使用新策略选项 [应用程序身份验证方法](/graph/api/resources/applicationauthenticationmethodpolicy?view=graph-rest-beta&preserve-view=true) 限制应用程序或服务主体上的自定义密码机密。
- 为运行 Windows 并在 Microsoft Store 或 Xbox 游戏商店中发布的应用指定 [设置](/graph/api/resources/windowsApplication?view=graph-rest-beta&preserve-view=true)。

### <a name="change-notifications"></a>更改通知
订阅 Outlook 联系人、事件或消息的更改，以接收有效负载中包含资源数据的通知。 有关详细信息，请参阅 [Microsoft Graph 中 Outlook 资源的更改通知](outlook-change-notifications-overview.md)。

### <a name="device-and-app-management--cloud-pc"></a>设备和应用管理|云电脑 
- 定义 [还原点设置](/graph/api/resources/cloudpcrestorepointsetting?view=graph-rest-beta&preserve-view=true)，其中包括创建还原点的频率，以及用户是否可以基于还原点备份还原自己的云电脑。
- [根据以前的快照](/graph/api/manageddevice-restorecloudpc?view=graph-rest-beta&preserve-view=true) 云电脑还原。
- [通过指定其托管设备 ID 和还原点的日期/时间范围（例如之前、之后）在单个请求中还原多个云电脑](/graph/api/manageddevice-bulkrestorecloudpc?view=graph-rest-beta&preserve-view=true)。

### <a name="identity-and-access--directory-management"></a>身份和访问 | 目录管理
使用应用程序权限 `CustomSecAttributeAssignment.Read.All` 为没有登录用户的组织读取[自定义安全属性定义](/graph/api/resources/customsecurityattributedefinition?view=graph-rest-beta&preserve-view=true)。

### <a name="identity-and-access--governance"></a>标识和访问权限 | 治理
- 在多阶段访问评审中为每个[阶段](/graph/api/resources/accessreviewstage?view=graph-rest-beta&preserve-view=true)配置[设置](/graph/api/resources/accessreviewstagesettings?view=graph-rest-beta&preserve-view=true)。 除了[获取](/graph/api/accessreviewstage-get?view=graph-rest-beta&preserve-view=true)或[更新](/graph/api/accessreviewstage-update?view=graph-rest-beta&preserve-view=true)访问评审阶段外，还可以执行以下操作： 
  - [阻止](/graph/api/accessreviewstage-stop?view=graph-rest-beta&preserve-view=true)审阅者向阶段提供更多输入，并继续进行下一个阶段（如果适用）。 
  - [筛选](/graph/api/accessreviewstage-filterbycurrentuser?view=graph-rest-beta&preserve-view=true)并获取[访问评审实例](/graph/api/resources/accessreviewinstance?view=graph-rest-beta&preserve-view=true)的所有阶段，其中调用用户是其审阅者
  - [列出](/graph/api/accessreviewstage-list-decisions?view=graph-rest-beta&preserve-view=true)多阶段访问评审中的决策。
- 应用可以使用应用程序权限 `EntitlementManagement.ReadWrite.All` 来[创建访问包资源请求](/graph/api/entitlementmanagement-post-accesspackageresourcerequests?view=graph-rest-beta&preserve-view=true)，以向[访问包目录](/graph/api/resources/accesspackagecatalog?view=graph-rest-beta&preserve-view=true)添加或删除资源。

### <a name="identity-and-access--identity-and-sign-in"></a>标识和访问权限 | 标识和登录
- 使用许多新属性来配置 [组织的品牌](/graph/api/resources/organizationalbrandingproperties?view=graph-rest-beta&preserve-view=true)。例如，登录页面的公司徽标的横幅版本、包含基于 CDN 的 URL 的自定义 favicon，以及用户管理帐户的一些其他自定义属性。
- 在[条件访问策略](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta&preserve-view=true)中包括或排除 Linux 作为[平台](/graph/api/resources/conditionalaccessplatforms?view=graph-rest-beta&preserve-view=true)条件之一。
- 使用 Azure AD 确定组织中的[风险服务主体](/graph/api/resources/riskyserviceprincipal?view=graph-rest-beta&preserve-view=true)，它会持续根据各种信号和机器学习[检测和评估](/graph/api/resources/serviceprincipalriskdetection?view=graph-rest-beta&preserve-view=true)风险。 可以[确认](/graph/api/riskyserviceprincipal-confirmcompromised?view=graph-rest-beta&preserve-view=true)风险服务主体是否确实遭到入侵，Microsoft 将据此对其禁用该服务主体对象。 可以[消除](/graph/api/riskyserviceprincipal-dismiss?view=graph-rest-beta&preserve-view=true)风险服务主体的风险。 此外，还可以列出服务主体的[风险历史记录](/graph/api/riskyserviceprincipal-list-history?view=graph-rest-beta&preserve-view=true)。
- 使用[跨租户访问设置](/graph/api/resources/crosstenantaccesspolicy-overview?view=graph-rest-beta&preserve-view=true)来控制和管理组织中用户与其他组织之间的协作。 它们非常细化，可让你确定组织和外部组织中可以参与 Azure AD B2B 协作和 Azure AD B2B 直接连接的用户、组和应用程序。 
- 启用或禁用组织中的用户和组以使用 [Azure AD 本机基于证书的身份验证 (CBA)](/graph/api/resources/x509CertificateAuthenticationMethodConfiguration?view=graph-rest-beta&preserve-view=true)。

### <a name="search"></a>搜索
为组织中的用户设置 [首字母缩写词](/graph/api/resources/search-acronym?view=graph-rest-beta&preserve-view=true)、 [书签](/graph/api/resources/search-bookmark?view=graph-rest-beta&preserve-view=true)和 [QnA](/graph/api/resources/search-qna?view=graph-rest-beta&preserve-view=true) 资源，作为组织中用户的 [管理搜索答案](search-concept-answers.md)。


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
