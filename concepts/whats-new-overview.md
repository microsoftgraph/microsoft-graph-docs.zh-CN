---
title: Microsoft Graph 新增功能
description: Microsoft Graph 新增功能
author: angelgolfer-ms
ms.localizationpriority: high
ms.openlocfilehash: c3c777812ca45cc1ad8d28bdbb266b63b0df3880
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59764512"
---
# <a name="whats-new-in-microsoft-graph"></a>Microsoft Graph 新增功能

查看 Microsoft Graph 中的最近两个月新增功能要点、[以前增加的内容](whats-new-earlier.md)以及如何[分享你的想法](#want-to-stay-in-the-loop)。 有关 API 级更新的详细列表，请参见 [API更改日志](https://developer.microsoft.com/graph/changelog/)。 

> [!IMPORTANT]
> 处于 _预览_ 状态的功能（包括 API 和工具）可能会发生更改，恕不另行通知，有些功能可能永远不会提升为正式发布 (GA) 状态。不要在生产应用中使用预览功能。

## <a name="september-2021-new-and-generally-available"></a>2021 年 9 月: 新增功能和正式发布

### <a name="cloud-communications--online-meetings"></a>云通信 | 联机会议
将 `OnlineMeetingArtifact.Read.All` 用为委派权限或应用程序权限，以读取联机会议的项目。 有关详细信息，请参阅 [联机会议权限](permissions-reference.md#online-meetings-permissions)。

### <a name="files"></a>文件
- 通过 **恶意软件** 属性获取 [driveItem](/graph/api/resources/driveItem) 中检测到的病毒的详细信息。
- 使用 [delta](/graph/api/driveitem-delta) 函数不仅可以跟踪根文件夹的更改，还可以跟踪驱动器中其他文件夹的更改。

### <a name="identity-and-access--directory-management"></a>标识和访问权限 | 目录管理
- 基于角色的访问控制 (RBAC) 提供商可以在 Azure Active Director 中[管理角色](/graph/api/resources/rolemanagement)，方法是[定义可以在特定资源上执行的角色操作](/graph/api/resources/unifiedroledefinition)，基于这些角色定义为用户[分配角色](/graph/api/resources/unifiedroleassignment)，为他们授权相应的资源访问权限。

### <a name="search--query"></a>搜索 | 查询
- 聚合数值或字符串类型搜索结果，这些结果由 [Microsoft Graph 连接器](/microsoftsearch/connectors-overview) 导入，并在 [架构](/graph/api/resources/schema) 中设置为可精简。请参阅有关 [使用聚合优化搜索结果](search-concept-aggregation.md) 的详细信息。
- 对任何可排序属性上的 OneDrive 和 SharePoint 搜索结果进行 [排序](/graph/api/resources/search-api-overview#sort-search-results)。 有关详细信息，请参阅 [使用 Microsoft 搜索 API 对搜索结果进行排序](search-concept-sort.md)。

### <a name="teamwork"></a>团队合作
- 使用一个操作 [provisionEmail](/graph/api/channel-provisionemail) 获取 [频道的电子邮件地址](/graph/api/resources/channel) (如果存在)，或者另创建一个。使用 [removeEmail](/graph/api/channel-removeemail) 操作删除电子邮件地址。

### <a name="workbooks-and-charts"></a>工作簿和图表
异步创建表行。 为了提高性能，创建多个表行的好做法是在 [create tableRow](/graph/api/table-post-rows) 操作中对其进行批处理并异步执行该操作。 遵循 [GET workbookOperation](/graph/api/workbookoperation-get) 操作和 [tableRowOperationResult](/graph/api/workbook-tableRowOperationResult) 函数，以获取新的 [workbookTableRow](/graph/api/resources/workbooktablerow) 资源。


## <a name="september-2021-new-in-preview-only"></a>2021 年 9 月: 仅预览版新增功能

### <a name="cloud-communications--online-meetings"></a>云通信 | 联机会议
获取 [联机会议](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true) 的 [会议出席报告](/graph/api/resources/meetingattendancereport?view=graph-rest-beta&preserve-view=true) 中的参与者总数。

### <a name="compliance--ediscovery"></a>合规性 | 电子数据展示
[创建用例](/graph/api/ediscovery-case-post?view=graph-rest-beta&preserve-view=true) 操作始终以大格式创建用例。 这扩大了用例大小限制，以容纳更高的数据总量和项目总数。 有关详细信息，请参阅 [大用例优势](/microsoft-365/compliance/advanced-ediscovery-large-cases?view=o365-worldwide&preserve-view=true#benefits-of-large-cases)。

### <a name="devices-and-apps--cloud-pc"></a>设备和应用 | 云电脑
- [将云电脑重新设置](/graph/api/manageddevice-reprovisioncloudpc?view=graph-rest-beta&preserve-view=true) 为已注册到 Intune 的云托管虚拟桌面。
- 使用新的虚拟 CPU (vCPU)和存储大小将云电脑升级或降级到其他配置，从而 [调整云电脑大小](/graph/api/manageddevice-resizecloudpc?view=graph-rest-beta&preserve-view=true)。

### <a name="education"></a>教育版
如果将 `Prefer: include-unknown-enum-members` 请求头应用于对 [educationAssignment](/graph/api/resources/educationassignment?view=graph-rest-beta&preserve-view=true) 或 [educationAssignmentDefaults](/graph/api/resources/educationassignmentdefaults?view=graph-rest-beta&preserve-view=true) 资源执行操作，则支持仅向学生日历添加作业。

### <a name="identity-and-access--governance"></a>标识和访问权限 | 治理
[删除](/graph/api/accesspackageassignmentrequest-delete?view=graph-rest-beta&preserve-view=true)[accessPackageAssignmentRequest](/graph/api/resources/accesspackageassignmentrequest?view=graph-rest-beta&preserve-view=true) 以删除已拒绝或已完成的请求。

### <a name="identity-and-access--identity-and-sign-in"></a>标识和访问权限 | 标识和登录
允许用户使用 [软件 OATH 令牌](/graph/api/resources/softwareOathAuthenticationMethod?view=graph-rest-beta&preserve-view=true) 执行多重身份验证。 软件 OATH 令牌为基于软件的数字生成器，其使用 OATH 基于时间的一次性密码(TOTP)标准。


## <a name="august-2021-new-and-generally-available"></a>2021 年 8 月: 新增功能和正式发布

### <a name="cloud-communications--calls"></a>云通信 | 呼叫
[参与者](/graph/api/resources/participant) 可以将元数据作为数据的 blob 包含在 [呼叫](/graph/api/resources/call) 名单中。

### <a name="cloud-communications--online-meetings"></a>云通信 | 联机会议
- 将 [联机会议](/graph/api/resources/onlinemeeting) 创建为实时事件，并使用制作者角色配置 [广播设置](/graph/api/resources/broadcastMeetingSettings) 和 [会议参与者信息](/graph/api/resources/meetingparticipantinfo)。 请参阅 [示例](/graph/api/application-post-onlinemeetings#example-2-create-a-live-event-with-user-token)。
- 使用 "allowMeetingChat **属性为联机会议启用、禁用** 或限制聊天持续时间。
- 通过使用 **allowTeamworkReactions** 属性来启用或禁用联机会议的响应。
- 允许与会者分别使用 **allowAttendeeToEnableCamera** 或 **allowAttendeeToEnableMic** 属性启用相机或麦克风。

### <a name="cloud-communications--presence"></a>云通信 | 在线
- [设置用户的在线状态](/graph/api/presence-setpresence)，这是每个 Teams 客户端(桌面、移动或 Web)上的聚合状态。
- 为用户 [清除在线会话](/graph/api/presence-clearpresence)。


### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 企业管理
v1.0 版本的 Intune 月度更新。设置 2021 年 8 月的 **日期** 筛选器，并查找具有此相同标题的节。

### <a name="devices-and-apps--service-health-and-communications"></a>设备和应用|服务运行状况和通信
使用 Microsoft Graph 中的[服务通信 API](service-communications-concept-overview.md) 访问有关 Microsoft 云服务的运行状况和消息中心帖子。

### <a name="identity-and-access--governance"></a>身份和访问 | 治理
获取访问评审范围的集合，这些范围用于定义[访问评审实例](/graph/api/resources/accessReviewInstance)的审阅者和回退审阅者。

### <a name="sites-and-lists--taxonomy"></a>站点和列表 | 分类
访问 SharePoint [术语库](/graph/api/resources/termstore-store) 分类，以及由 [组](/graph/api/resources/termstore-group)、[设置](/graph/api/resources/termstore-set)、[术语](/graph/api/resources/termstore-term) 资源以及术语之间的 [关系](/graph/api/resources/termstore-relation) 资源组成的层次结构。

### <a name="teamwork"></a>团队合作
在委派上下文中 [列出聊天](/graph/api/chat-list) (用户所属)。

## <a name="august-2021-new-in-preview-only"></a>2021 年 8 月: 仅预览版新增功能

### <a name="cloud-communications--calls"></a>云通信 | 呼叫
- 使用 [startHoldMusic](/graph/api/participant-startHoldMusic?view=graph-rest-beta&preserve-view=true) 操作让 [参与者](/graph/api/resources/participant?view=graph-rest-beta&preserve-view=true) 保持呼叫并在后台播放音乐。
- 使用 [stopHoldMusic](/graph/api/participant-stopHoldMusic?view=graph-rest-beta&preserve-view=true) 操作重新合并之前呼叫保持的参与者。

### <a name="cloud-communications--online-meetings"></a>云通信 | 联机会议
将 [联机会议](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true) 设置为自动录制。

### <a name="devices-and-apps--cloud-pc"></a>设备和应用 | 云电脑
为云电脑 [结束宽限期](/graph/api/cloudPC-endGracePeriod?view=graph-rest-beta&preserve-view=true)。 宽限期允许用户最多可在取消设置前的 7 天内访问云电脑。 结束宽限期会立即取消设置云电脑，无需等待七天。

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 企业管理
beta 版本的 Intune 月度更新。将 **日期** 筛选器设置为 2021 年 6 月，并查找具有此相同标题的节。

### <a name="identity-and-access--governance"></a>身份和访问 | 治理
- [重新处理](/graph/api/accesspackageassignmentrequest-reprocess?view=graph-rest-beta&preserve-view=true)[访问包分配请求](/graph/api/resources/accesspackageassignmentrequest?view=graph-rest-beta&preserve-view=true)以自动重试用户对包的访问请求。
- [重新处理](/graph/api/accesspackageassignment-reprocess?view=graph-rest-beta&preserve-view=true)[访问包分配](/graph/api/resources/accesspackageassignment?view=graph-rest-beta&preserve-view=true)以自动重新评估和强制执行用户分配。
- [获取一组策略要求](/graph/api/accesspackage-getapplicablepolicyrequirements?view=graph-rest-beta&preserve-view=true)以便[为访问包创建分配请求](/graph/api/resources/accesspackageassignmentrequestrequirements?view=graph-rest-beta&preserve-view=true)。
- 获取[访问评审审阅者](/graph/api/resources/accessreviewreviewer?view=graph-rest-beta&preserve-view=true)资源的集合，这些资源用于定义与[访问审阅实例](/graph/api/resources/accessReviewInstance?view=graph-rest-beta&preserve-view=true)联系的审阅者。
- 使用 **recommendationLookBackDuration** 属性，获取或设置在 [访问评审的计划设置中](/graph/api/resources/accessReviewScheduleSettings?view=graph-rest-beta&preserve-view=true)配置建议的非活动持续时间。

### <a name="identity-and-access--identity-and-sign-in"></a>身份和访问 | 身份和登录
- 组织可以使用[策略来强制应用使用应用程序身份验证方法的最佳做法](/graph/api/resources/applicationauthmethodpolicy?view=graph-rest-beta&preserve-view=true)。 此类策略可以应用于[特定应用程序和服务主体](/graph/api/resources/appmanagementpolicy?view=graph-rest-beta&preserve-view=true)，或[租户中的所有应用程序和服务主体](/resources/tenantappmanagementpolicy?view=graph-rest-beta&preserve-view=true)。
- 支持在 [用户](/api/user-list-approleassignments?view=graph-rest-beta&preserve-view=true)、[组](/api/group-list-approleassignments?view=graph-rest-beta&preserve-view=true) 和 [服务主体](/api/serviceprincipal-list-approleassignments?view=graph-rest-beta&preserve-view=true) 的 **appRoleAssignments** 导航属性上进行分页。
- 允许 Azure Active Directory (Azure AD)租户设置 [与另一个标识提供程序(IdP)支持 SAML 或 WS-Fed 协议的组织联盟](/graph/api/resources/samlOrWsFedExternalDomainFederation?view=graph-rest-beta&preserve-view=true)。 这使得 Azure AD 租户能够允许来宾用户访问其资源。

### <a name="teamwork"></a>团队合作
- 获取与 [聊天](/api/resources/chat?view=graph-rest-beta&preserve-view=true) 关联的 [联机会议的信息](/graph/api/resources/teamworkOnlineMeetingInfo?view=graph-rest-beta&preserve-view=true)。
- 获取在其中创建 **聊天** 的租户的标识符。

### <a name="users"></a>用户
使用用户 [signInActivity](/graph/api/resources/signInActivity?view=graph-rest-beta&preserve-view=true) 的最后一个交互式和非交互式登录日期/时间值来 [管理非活动帐户](/azure/active-directory/reports-monitoring/howto-manage-inactive-user-accounts)。

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
