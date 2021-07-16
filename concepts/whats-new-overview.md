---
title: Microsoft Graph 新增功能
description: Microsoft Graph 新增功能
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 873e6fa03fd02470eb520657573556266de6f2a7
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53443205"
---
# <a name="whats-new-in-microsoft-graph"></a>Microsoft Graph 新增功能

查看 Microsoft Graph 中的最近两个月新增功能要点、[以前增加的内容](whats-new-earlier.md)以及如何[分享你的想法](#want-to-stay-in-the-loop)。 有关 API 级更新的详细列表，请参见 [API更改日志](https://developer.microsoft.com/graph/changelog/)。 

> [!IMPORTANT]
> 处于 _预览_ 状态的功能（包括 API 和工具）可能会发生更改，恕不另行通知，有些功能可能永远不会提升为正式发布 (GA) 状态。不要在生产应用中使用预览功能。

## <a name="july-2021-new-and-generally-available"></a>2021 年 7 月: 新版本和正式版

### <a name="cloud-communications--calls"></a>云通信 | 呼叫
在采用 [基于 Teams 策略录制](/microsoftteams/teams-recording-policy) 的组织中，支持对应用程序在 [接听](/graph/api/call-answer) [通话](/graph/api/resources/call) 时可以处理的参与者数量容量限制。

### <a name="users"></a>用户
让用户 [更改自己的密码](/graph/api/user-changepassword) 而无需管理员角色。


## <a name="july-2021-new-in-preview-only"></a>2021 年 7 月: 预览版新增功能

### <a name="devices-and-apps--cloud-pc"></a>设备和应用 | 云电脑
本地连接 [运行状况检查](/graph/api/cloudpconpremisesconnection-runhealthcheck?view=graph-rest-beta&preserve-view=true) 可以识别更多可能的运行状况检查错误类型:
- 在组织单位 (`adJoinCheckComputerObjectAlreadyExists`) 中未找到云 PC 计算机帐户。
- 在 Azure AD (`azureAdDeviceSyncCheckDeviceNotFound`) 中未找到云 PC 对象。
- 检查云 PC 对象是否已同步到 Azure AD (`azureAdDeviceSyncCheckLongSyncCircle`) 时超时。 

详情和建议的补救措施见[参考文献](/graph/api/resources/cloudpconpremisesconnectionhealthcheck?view=graph-rest-beta&preserve-view=true#cloudpconpremisesconnectionhealthcheckerrortype-values)。

### <a name="devices-and-apps--multi-tenant-management"></a>设备和应用|多租户管理
[Microsoft 365 Lighthouse API](managedtenants-concept-overview.md) 的首次亮相，使管理服务提供商 (MSP) 能够大规模地远程管理多个客户租户的合规性和威胁检测，并帮助使租户设备处于健康和安全状态。

### <a name="search"></a>搜索
使用 [Microsoft 搜索 API 检索与用户最相关人员](search-concept-person.md) 的信息。相关性由用户的通信和协作模式以及业务关系决定。 

### <a name="teamwork"></a>团队合作
- [订阅聊天资源](teams-changenotifications-chat.md) 的更改通知。
- [订阅聊天中](teams-changenotifications-chatmembership.md)、[频道](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true) 中或 [团队](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true) 中用户的更改通知 (即，[conversationMember](/graph/api/resources/conversationmember?view=graph-rest-beta&preserve-view=true) 资源)。

## <a name="june-2021-new-and-generally-available"></a>2021 年 6 月：新版本和正式发布版本

### <a name="applications"></a>应用程序
获取或设置 [应用程序](/graph/api/resources/application)或 [servicePrincipal](/graph/api/resources/serviceprincipal) 的状态，以确定 Microsoft 是否已通过 **disabledByMicrosoftStatus** 属性禁用应用程序。 禁用原因包括可疑、滥用或恶意活动，或违反 Microsoft 服务协议。

### <a name="change-notifications"></a>更改通知
在以下资源过期之前，已延长订阅的最大长度：
- OneDrive [driveItem](/graph/api/resources/driveitem) 和 SharePoint [列表](/graph/api/resources/list)从 3 天延长至 30 天。
- [组](/graph/api/resources/group)、[用户](/graph/api/resources/user)或其他目录资源，从 3 天延长至 29 天。

### <a name="change-tracking"></a>更改跟踪
移除了 Microsoft OneDrive for Business 和 SharePoint 中，非根文件夹中的更改跟踪限制。

### <a name="education"></a>教育版
教育版[分配服务](/graph/api/resources/educationassignment)的 API 现已正式发布。 

### <a name="identity-and-access--governance"></a>身份和访问 | 治理
[访问评审](/graph/api/resources/accessreviewsv2-root) API 的 GA。 查看[概述](accessreviews-overview.md)和教程，以[评审对安全组的访问权限](tutorial-accessreviews-securitygroup.md)，以及[对 Microsoft 365 组的访问权限](tutorial-accessreviews-m365group.md)。 请注意，[旧访问评审 API](/graph/api/resources/accessreviews-root?view=graph-rest-beta&preserve-view=true) 已被弃用，并将在 2023 年 5 月停止返回数据。


## <a name="june-2021-new-in-preview-only"></a>2021 年 6 月：预览版新增功能

### <a name="cloud-communications--online-meetings"></a>云通信 | 联机会议
分别通过 **allowAttendeeToEnableCamera** 和 **allowAttendeeToEnableMic** 启用和禁用与会者打开摄像头和麦克风，在 [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true) 中自定义音频和视频控件。

### <a name="devices-and-apps--cloud-pc"></a>设备和应用 | 云电脑
- [分配](/graph/api/cloudpcusersetting-assign?view=graph-rest-beta&preserve-view=true)和管理 [cloudPcUserSetting](/graph/api/resources/cloudpcusersetting?view=graph-rest-beta&preserve-view=true)，为云电脑上的用户启用本地管理员或自助服务选项。 当前可在组级别（属于 Microsoft 365 组或安全组的用户）进行分配。
- [获取](/graph/api/cloudpc-get?view=graph-rest-beta&preserve-view=true) [cloudPC](/graph/api/resources/cloudpc?view=graph-rest-beta&preserve-view=true) 的几个新属性：预配策略的名称和预配期间使用的本地连接的名称，以及执行重新预配或取消预配的宽限期的结束日期/时间。
- 对[本地连接](/graph/api/cloudpconpremisesconnection-runhealthcheck?view=graph-rest-beta&preserve-view=true)进行[运行状况检查](/graph/api/resources/cloudpconpremisesconnection?view=graph-rest-beta&preserve-view=true)时，支持更多状态和错误类型。

### <a name="education"></a>教育
- 现在，教师可以在发布作业时选择日历的默认行为。 教师可以通过使用 [educationAssignment](/graph/api/resources/educationAssignment?view=graph-rest-beta&preserve-view=true) 资源的 **addToCalendarAction** 属性来控制作业的日历行为。
- 现在，教师还可以在发布作业时设置日历的默认行为。 教师可以通过使用 [educationAssignmentDefaults](/graph/api/resources/educationAssignmentDefaults?view=graph-rest-beta&preserve-view=true) 资源的 **addToCalendarAction** 属性来控制作业默认的日历行为。

### <a name="groups"></a>组
允许通过设置 **isAssignableToRole** 属性在创建时向 [组](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) 分配 Azure AD 角色。如果设置此属性，则可以方便地管理个人的角色 - 合格人员可以加入组，而不必为每个人分配角色，默认情况下，为组分配角色将为加入组的每个新成员分配角色。 

### <a name="identity-and-access--governance"></a>身份和访问 | 治理
通过使用 [ 计划定义](/graph/api/resources/accessreviewscheduledefinition?view=graph-rest-beta&preserve-view=true) 的 **additionalNotificationRecipients** 属性，将用户或组成员设置为接收 [访问评审](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true) 进度的通知。

### <a name="identity-and-access--identity-and-sign-in"></a>身份和访问 | 身份和登录
使用 [conditionalAccessDevices](/graph/api/resources/conditionalAccessDevices?view=graph-rest-beta&preserve-view=true) 的 **deviceFilter** 属性定义筛选器，动态包含或排除设备。

### <a name="sites-and-lists"></a>网站和列表
通过调用 [createLink](/graph/api/listitem-createlink?view=graph-rest-beta&preserve-view=true)，为 [listItem](/graph/api/resources/listitem?view=graph-rest-beta&preserve-view=true) 创建或获取现有的 [sharingLink](/graph/api/resources/sharinglink?view=graph-rest-beta&preserve-view=true)。

### <a name="teamwork"></a>团队合作
- 通过 webUrl 属性 [获取](/graph/api/chat-get?view=graph-rest-beta&preserve-view=true)[聊天](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true)的 **非跳转 URL**。
- [订阅[频道](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true)、[conversationMember](/graph/api/resources/conversationmember?view=graph-rest-beta&preserve-view=true) 或[团队](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true)资源的更改通知。](/graph/webhooks?view=graph-rest-beta&preserve-view=true)
- 将带有 API 的[特定于资源的同意](/microsoftteams/platform/graph-api/rsc/resource-specific-consent)权限，用于[频道](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true)、[聊天](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true)、[chatMessage](/graph/api/resources/chatMessage?view=graph-rest-beta&preserve-view=true)、[chatMessageHostedContent](/graph/api/resources/chatMessageHostedContent?view=graph-rest-beta&preserve-view=true) 或[团队](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true)。
- 获取[团队](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true)的[特定于资源的权限授予](/graph/api/resources/resourcespecificpermissiongrant?view=graph-rest-beta&preserve-view=true)列表，该列表指定团队的应用，以及相应的已获得授权的特定于资源的权限。
- [获取](/graph/api/teamsasyncoperation-get?view=graph-rest-beta&preserve-view=true)具体的[异步操作](/graph/api/resources/teamsasyncoperation?view=graph-rest-beta&preserve-view=true)，或[列出](/graph/api/chat-list-operations?view=graph-rest-beta&preserve-view=true)在[聊天](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true)上运行的所有异步操作。
- 可在[创建聊天](/graph/api/chat-post?view=graph-rest-beta&preserve-view=true)时指定[Teams 应用](/graph/api/resources/teamsapp?view=graph-rest-beta&preserve-view=true)。
- 使用一个操作 [provisionEmail](/graph/api/channel-provisionemail?view=graph-rest-beta&preserve-view=true) 获取 [频道的电子邮件地址](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true) (如果存在)，或者另创建一个。使用 [removeEmail](/graph/api/channel-removeemail?view=graph-rest-beta&preserve-view=true) 操作删除电子邮件地址。

### <a name="teamwork--shifts"></a>团队合作 | 倒班
- 支持 [offerShiftRequest](/graph/api/resources/offershiftrequest?view=graph-rest-beta&preserve-view=true)、[timeOff](/graph/api/resources/timeoff?view=graph-rest-beta&preserve-view=true)、[timeOffReason](/graph/api/resources/timeoffreason?view=graph-rest-beta&preserve-view=true) 和 [timeOffRequest](/graph/api/resources/timeoffrequest?view=graph-rest-beta&preserve-view=true) 实体发送同步更改通知。
- 支持管理[工时记录卡](/graph/api/resources/timecard?view=graph-rest-beta&preserve-view=true)资源和常见功能，例如，[上班打卡](/graph/api/timecard-clockin?view=graph-rest-beta&preserve-view=true)、[下班打卡](/graph/api/timecard-clockout?view=graph-rest-beta&preserve-view=true)、[开始休息](/graph/api/timecard-startbreak?view=graph-rest-beta&preserve-view=true)、[结束休息](/graph/api/timecard-endbreak?view=graph-rest-beta&preserve-view=true)、[确认](/graph/api/timecard-confirm?view=graph-rest-beta&preserve-view=true)和[替班](/graph/api/timecard-replace?view=graph-rest-beta&preserve-view=true)。


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
