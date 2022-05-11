---
title: Microsoft Graph 新增功能
description: Microsoft Graph 新增功能
author: angelgolfer-ms
ms.localizationpriority: high
ms.openlocfilehash: 75b01f4903153249131cc69e336bb2d12e26095d
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65316159"
---
# <a name="whats-new-in-microsoft-graph"></a>Microsoft Graph 新增功能

查看 Microsoft Graph 中的最近两个月新增功能要点、[以前增加的内容](whats-new-earlier.md)以及如何[分享你的想法](#want-to-stay-in-the-loop)。 有关 API 级更新的详细列表，请参见 [API更改日志](https://developer.microsoft.com/graph/changelog/)。 

> [!IMPORTANT]
> 处于 _预览_ 状态的功能（包括 API 和工具）可能会发生更改，恕不另行通知，有些功能可能永远不会提升为正式发布 (GA) 状态。不要在生产应用中使用预览功能。


## <a name="april-2022-new-in-preview-only"></a>2022 年 4 月：仅限预览版中的新增功能

### <a name="customer-bookings"></a>客户预订
- [获取[企业](/graph/api/resources/bookingbusiness?view=graph-rest-beta&preserve-view=true)中[员工成员](/graph/api/resources/bookingstaffmember?view=graph-rest-beta&preserve-view=true)资源的可用信息](/graph/api/bookingbusiness-getstaffavailability?view=graph-rest-beta&preserve-view=true)。
- 使用面向`Bookings.Read.All`[企业](/graph/api/resources/bookingbusiness?view=graph-rest-beta&preserve-view=true)、[员工成员](/graph/api/resources/bookingstaffmember?view=graph-rest-beta&preserve-view=true)、[服务](/graph/api/resources/bookingservice?view=graph-rest-beta&preserve-view=true)、[客户](/graph/api/resources/bookingcustomer?view=graph-rest-beta&preserve-view=true)和[预约](/graph/api/resources/bookingappointment?view=graph-rest-beta&preserve-view=true)资源的读取操作中的应用程序权限。
- 对客户和预约资源使用读/写操作的应用程序权限 `BookingsAppointment.ReadWrite.All`。

### <a name="device-and-app-management--cloud-pc"></a>设备和应用管理|云电脑
将 [Windows 设置](/graph/api/resources/cloudpcwindowssettings?view=graph-rest-beta&preserve-view=true)指定为租户的[云电脑组织设置](/graph/api/resources/cloudPcOrganizationSettings?view=graph-rest-beta&preserve-view=true)的一部分。

### <a name="identity-and-access--directory-management"></a>身份和访问 | 目录管理
配置[联合身份验证设置](/graph/api/resources/internalDomainFederation?view=graph-rest-beta&preserve-view=true)，将域与 Azure Active Directory 联合。

### <a name="reports--identity-and-access-reports"></a>报告 | 身份和访问报告
通过在相应的 Azure Active Directory 登录日志中标记事件，确认事件存在[高风险且已泄露](/graph/api/signin-confirmCompromised?view=graph-rest-beta&preserve-view=true)或[安全](/graph/api/signin-confirmSafe?view=graph-rest-beta&preserve-view=true)。

### <a name="reports--microsoft-365-usage-reports"></a>报告 | Microsoft 365 使用情况报告
- 获取指定时间段内特定 Teams 活动的计数的[总分布报告](/graph/api/reportroot-getTeamsUserActivityTotalDistributionCounts?view=graph-rest-beta&preserve-view=true)。 Teams 活动的计数包括团队聊天消息、通话、会议、音频持续时间、发布消息等。
- 在报告中获取其获取用户详细信息，包括[获取用户详细信息](/graph/api/reportroot-getTeamsUserActivityUserDetail?view=graph-rest-beta&preserve-view=true)、[获取活动计数](/graph/api/reportroot-getteamsuseractivitycounts?view=graph-rest-beta&preserve-view=true)，以及[获取活动总计数](/graph/api/reportroot-getteamsuseractivitytotalcounts?view=graph-rest-beta&preserve-view=true)。

### <a name="teamwork"></a>Teamwork
与一个或多个团队共享频道：
- [仅列出与团队共享的频道](/graph/api/team-list-incomingchannels?view=graph-rest-beta&preserve-view=true)。
- [列出团队中的所有频道](/graph/api/team-list-allchannels?view=graph-rest-beta&preserve-view=true)，包括在团队中托管或与团队共享的频道。
- [列出可以访问指定共享通道的团队成员](/graph/api/sharedwithchannelteaminfo-list-allowedmembers?view=graph-rest-beta&preserve-view=true)。
- [删除与团队共享的频道](/graph/api/team-delete-incomingchannel?view=graph-rest-beta&preserve-view=true)。
- [列出已共享指定频道的团队](/graph/api/sharedwithchannelteaminfo-list?view=graph-rest-beta&preserve-view=true)。
- [取消与团队共享频道](/graph/api/sharedwithchannelteaminfo-delete?view=graph-rest-beta&preserve-view=true)。


## <a name="march-2022-new-and-generally-available"></a>2022 年 3 月：新增和正式发布

### <a name="files"></a>文件
使用 [捆绑包](/graph/api/resources/bundle) 资源一次共享多个文件，就像其他 [driveItem](/graph/api/resources/driveitem) 资源一样。 可以对捆绑包应用 CRUD 操作， [将](/graph/api/bundle-additem) 项添加到或 [从捆绑包中删除](/graph/api/bundle-removeitem) 项。

### <a name="identity-and-access--directory-management"></a>身份和访问 | 目录管理
使用 [特定于资源的权限](/graph/api/resources/resourcespecificpermission) 授权 Teams 应用直接访问聊天或团队的特定实例的数据。 例如，特定于资源的权限 ChannelMessage.Read.Group 允许 Teams 应用读取单个团队的频道消息。

### <a name="identity-and-access--governance"></a>身份和访问 | 治理
- [获取](/graph/api/approval-get)与[访问包分配](/graph/api/resources/accesspackageassignmentrequest)的请求关联的[审批](/graph/api/resources/approval)决策。
- 作为 [Azure Active Directory (Azure AD) 权利管理](/graph/api/resources/entitlementmanagement-overview)的一部分，使用[访问包评估策略](/graph/api/resources/accesspackageassignmentpolicy)来管理[对访问包](/graph/api/resources/accesspackage)的请求、审批、分配或定期审查。 可以控制内部和外部用户对组织组、应用程序和联机网站 SharePoint 的访问权限。

### <a name="identity-and-access--identity-and-sign-in"></a>身份和访问 | 身份和登录
指定客户端应用程序[包含或排除](/graph/api/resources/conditionalaccessclientapplications)为应用[条件访问策略](/graph/api/resources/conditionalaccesspolicy)的一组[条件](/graph/api/resources/conditionalAccessConditionSet)。

### <a name="use-the-toolkit"></a>使用工具包
通过社区贡献来庆祝真正的团队合作，并试用 [Microsoft Graph 工具包 v2.4.0](https://github.com/microsoftgraph/microsoft-graph-toolkit/releases/tag/v2.4.0) 中的新功能：
- 通过使用 `disable-image-fetch` 属性控制不必要的提取，优化[人员](/graph/toolkit/components/person)组件中人员图像的刷新。
- 通过使用 `disable-images` 属性，避免在[人员选取器](/graph/toolkit/components/people-picker)组件中不必要地加载人员图像。 
- 使用 `user-filters`、`group-filters` 和 `people-filters` 属性筛选[人员选取器](/graph/toolkit/components/people-picker)组件中的可用用户、组和人员列表。


## <a name="march-2022-new-in-preview-only"></a>2022 年 3 月：仅预览版中的新增功能

### <a name="cloud-communications--online-meeting"></a>云通信 | 联机会议
指定一个或多个 [会议参与者](/graph/api/resources/meetingParticipants?view=graph-rest-beta&preserve-view=true) 为共同组织者。

### <a name="compliance--ediscovery"></a>合规性 | 电子数据展示
[清除数据](/graph/api/ediscovery-sourcecollection-purgeData?view=graph-rest-beta&preserve-view=true)并永久删除电子数据展示[源集合](/graph/api/resources/ediscovery-sourcecollection?view=graph-rest-beta&preserve-view=true)中的 Microsoft Teams 消息。

### <a name="device-and-app-management--cloud-pc"></a>设备和应用管理|云电脑
- 对[unifiedRoleDefinition](/graph/api/resources/unifiedroledefinition?view=graph-rest-beta&preserve-view=true)资源的读取操作使用`RoleManagement.Read.CloudPC`的委派权限或应用程序权限资源。
- 对[unifiedRoleDefinition](/graph/api/resources/unifiedroledefinition?view=graph-rest-beta&preserve-view=true)资源的读取和写入操作使用`RoleManagement.ReadWrite.CloudPC`的委派权限或应用程序权限资源。
- 指定 Azure 订阅的 ID 和显示名称，作为设备的[源映像信息](/graph/api/resources/cloudPcSourceDeviceImage?view=graph-rest-beta&preserve-view=true)的一部分。
- 指定 [Windows 设置](/graph/api/resources/cloudpcwindowssettings?view=graph-rest-beta&preserve-view=true)在为[预配策略创建云电脑时](/graph/api/resources/cloudPcProvisioningPolicy?view=graph-rest-beta&preserve-view=true)进行配置。

### <a name="device-and-app-management--corporate-management"></a>设备和应用管理|公司管理
- Intune 3 beta 版更新。

### <a name="device-and-app-management--multi-tenant-management"></a>设备和应用管理|多租户管理
[列出](/graph/api/managedtenants-managedtenant-list-auditevents?view=graph-rest-beta&preserve-view=true) 和 [获取 Microsoft 365 Lighthouse 中托管租户的](/graph/api/managedtenants-auditevent-get?view=graph-rest-beta&preserve-view=true) 审核事件。

### <a name="identity-and-access--directory-management"></a>身份和访问 | 目录管理
- [列表](/graph/api/organizationsettings-list-microsoftapplicationdataaccess?view=graph-rest-beta&preserve-view=true)或[更新](/graph/api/microsoftapplicationdataaccesssettings-update?view=graph-rest-beta&preserve-view=true)[设置](/graph/api/resources/microsoftapplicationdataaccesssettings?view=graph-rest-beta&preserve-view=true)，这些设置指定从 Microsoft 应用程序访问Microsoft 365属于组织中用户的数据。 例如，如果授权正确，是否只有Microsoft 365应用（如 Word 和 Excel）才能访问用户的Microsoft 365数据，或者其他 Microsoft 应用（如 Windows）是否也可以访问数据。 默认情况下，组织中的所有用户都可以在 Microsoft 应用中访问用户有权访问的任何Microsoft 365数据。 
- 在采用零信任网络案例模式后，Microsoft 合作伙伴可以使用[粒度委派管理员权限 (GDAP) ](/graph/api/resources/delegatedadminrelationships-api-overview?view=graph-rest-beta&preserve-view=true)以对其客户租户最低权限访问执行管理任务，避免潜在的安全风险。 合作伙伴无需像过去那样请求全局管理员角色，而是在一定的时间内请求客户租户管理的特定角色，并且其客户必须明确授予对他们的最低特权访问。

### <a name="security--attack-simulation-and-training"></a>安全 | 攻击模拟和训练
- [列出租户的模拟自动化](/graph/api/attacksimulationroot-list-simulationautomations?view=graph-rest-beta&preserve-view=true)。
- [列表为租户运行模拟自动化](/graph/api/resources/simulationautomationrun?view=graph-rest-beta&preserve-view=true)。

### <a name="search"></a>搜索
- 在 [搜索请求中指定](/graph/api/resources/searchrequest?view=graph-rest-beta&preserve-view=true) 是否从搜索结果中剪裁重复的 SharePoint 文件。默认为 false。
- 使用支持 KQL 和查询变量的模板限定 [搜索查询](/graph/api/resources/searchquery?view=graph-rest-beta&preserve-view=true) 字符串。

### <a name="sites-and-lists"></a>网站和列表
- 对于包含分类数据的 [列](/graph/api/resources/columnDefinition?view=graph-rest-beta&preserve-view=true) ，请指定父 [术语](/graph/api/resources/termstore-term?view=graph-rest-beta&preserve-view=true) 和 [术语集](/graph/api/resources/termstore-set?view=graph-rest-beta&preserve-view=true) ，子术语可选为列值。
- 获取[网站](/graph/api/resources/site?view=graph-rest-beta&preserve-view=true)的设置，包括语言和时区。

### <a name="tasks-and-plans"></a>任务和计划
通过检查相应 [plannerPlan](/graph/api/resources/plannerPlan?view=graph-rest-beta&preserve-view=true)资源关系的 **详细信息** 关系，确定用于 Planner 外部体验的 Planner 计划（如 Microsoft Teams）能否跟踪该上下文中的工作。

### <a name="teamwork"></a>Teamwork
- 获取或设置有关[团队](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true)的[摘要信息](/graph/api/resources/teamSummary?view=graph-rest-beta&preserve-view=true)，包括所有者、成员和来宾的计数。
- 在聊天中[列出消息](/graph/api/chat-list-messages?view=graph-rest-beta&preserve-view=true)时，按降序对邮件进行排序。


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
