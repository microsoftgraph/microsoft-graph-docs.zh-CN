---
title: Microsoft Graph 新增功能
description: Microsoft Graph 新增功能
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: b2e5cbb811e7e606fd57a9c967c40bc3956a2c58
ms.sourcegitcommit: 0adbbcbc65b6acab80e9195f13321055994f56be
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2021
ms.locfileid: "53236211"
---
# <a name="whats-new-in-microsoft-graph"></a>Microsoft Graph 新增功能

查看 Microsoft Graph 中的最近两个月新增功能要点、[以前增加的内容](whats-new-earlier.md)以及如何[分享你的想法](#want-to-stay-in-the-loop)。 有关 API 级更新的详细列表，请参见 [API更改日志](https://developer.microsoft.com/graph/changelog/)。 

> [!IMPORTANT]
> 处于 _预览_ 状态的功能（包括 API 和工具）可能会发生更改，恕不另行通知，有些功能可能永远不会提升为正式发布 (GA) 状态。不要在生产应用中使用预览功能。

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
- 使用单个操作 [provisionEmail](/graph/api/channel-provisionemail?view=graph-rest-beta&preserve-view=true) 获取[频道](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true)的电子邮件地址（如果存在）。如不存在，请创建一个。 使用 [removeEmail](/graph/api/channel-removeemail?view=graph-rest-beta&preserve-view=true) 操作删除电子邮件地址。

### <a name="teamwork--shifts"></a>团队合作 | 倒班
- 支持 [offerShiftRequest](/graph/api/resources/offershiftrequest?view=graph-rest-beta&preserve-view=true)、[timeOff](/graph/api/resources/timeoff?view=graph-rest-beta&preserve-view=true)、[timeOffReason](/graph/api/resources/timeoffreason?view=graph-rest-beta&preserve-view=true) 和 [timeOffRequest](/graph/api/resources/timeoffrequest?view=graph-rest-beta&preserve-view=true) 实体发送同步更改通知。
- 支持管理[工时记录卡](/graph/api/resources/timecard?view=graph-rest-beta&preserve-view=true)资源和常见功能，例如，[上班打卡](/graph/api/timecard-clockin?view=graph-rest-beta&preserve-view=true)、[下班打卡](/graph/api/timecard-clockout?view=graph-rest-beta&preserve-view=true)、[开始休息](/graph/api/timecard-startbreak?view=graph-rest-beta&preserve-view=true)、[结束休息](/graph/api/timecard-endbreak?view=graph-rest-beta&preserve-view=true)、[确认](/graph/api/timecard-confirm?view=graph-rest-beta&preserve-view=true)和[替班](/graph/api/timecard-replace?view=graph-rest-beta&preserve-view=true)。

## <a name="may-2021-new-and-generally-available"></a>2021 年 5 月：新版本和正式发布版本

### <a name="devices-and-apps--cloud-printing"></a>设备和应用 | 云打印
使用 [打印机](/graph/api/resources/printer)的 **lastSeenDateTime** 属性，查找打印机上次与“通用打印”交互的时间。

### <a name="identity-and-access--identity-and-sign-in"></a>身份和访问 | 身份和登录
使用 [authorizationPolicy](/graph/api/resources/authorizationpolicy) 的 **guestUserRoleId** 属性，获取或更新来宾用户的角色。

### <a name="mail"></a>邮件
- [创建草稿并以 MIME 格式发送 Outlook 邮件](outlook-send-mime-message.md)，附加 S/MIME 数字签名，并用 S/MIME 加密邮件内容。
- 通过[设置 isHidden 属性](/graph/api/user-post-mailfolders#example)，将 [mailFolder](/graph/api/resources/mailfolder) 创建为[隐藏文件夹](/graph/api/resources/mailfolder#hidden-mail-folders)。

### <a name="microsoft-graph-toolkit"></a>Microsoft Graph 工具包
请尝试 Microsoft Graph 工具包 2.2 中的以下新功能：
- [文件](/graph/toolkit/components/file)和[文件列表](/graph/toolkit/components/file-list)组件
- [MSAL 2.0 身份验证提供程序](/graph/toolkit/providers/msal2)
- [SharePoint 框架库](/graph/toolkit/get-started/mgt-spfx)

### <a name="reports--azure-ad-activity-reports"></a>报告 | Azure AD 活动报告
Azure AD 预配服务和其相关属性执行的向[列表](/graph/api/provisioningobjectsummary-list)报告 API 操作的正式发布。 将 API 之前的 Beta 版本与 v1.0 版本对齐。 

## <a name="may-2021-new-in-preview-only"></a>2021 年 5 月：仅限预览版新增功能

### <a name="connecting-external-content"></a>连接外部内容
- 设计连接器时，请注意[实施和运行限制](connecting-external-content-api-limits.md)。
- 尝试[将 Postman 和连接器 API 一起使用](connecting-external-content-connectors-api-postman.md)。

### <a name="devices-and-apps--cloud-pc"></a>设备和应用 | 云电脑
请求最小特权应用程序权限`CloudPC.Read.All`或`CloudPC.ReadWrite.All`以下资源的访问方法：
  - 读写操作和 [cloudPC](/graph/api/resources/cloudpc?view=graph-rest-beta&preserve-view=true) 的 [reprovision](/graph/api/cloudpc-reprovision?view=graph-rest-beta&preserve-view=true) 方法。
  - 读写操作和 [cloudPcDeviceImage](/graph/api/resources/cloudpcdeviceimage?view=graph-rest-beta&preserve-view=true) 的 [getSourceImages](/graph/api/cloudpcdeviceimage-getsourceimages?view=graph-rest-beta&preserve-view=true) 方法。
  - 读写操作和 [cloudPcOnPremisesConnection](/graph/api/resources/cloudpconpremisesconnection?view=graph-rest-beta&preserve-view=true) 的 [updateAdDomainPassword](/graph/api/cloudpconpremisesconnection-updateaddomainpassword?view=graph-rest-beta&preserve-view=true) 方法。
  - 读写操作和 [cloudPcProvisioningPolicy](/graph/api/resources/cloudpcprovisioningpolicy?view=graph-rest-beta&preserve-view=true) 的[分配](/graph/api/cloudpcprovisioningpolicy-assign?view=graph-rest-beta&preserve-view=true)方法。

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理
Beta 版本的 Intune 月度更新。将 **日期** 筛选器设置为 2021 年 6 月，并查找具有此相同标题的部分。

### <a name="education"></a>教育版
- [设置 SharePoint 资源文件夹](/graph/api/educationAssignment-setupresourcesfolder?view=graph-rest-beta&preserve-view=true)，以在同一位置上​​传和存储所有基于文件的资源，从而进行 [educationAssignment](/graph/api/resources/educationAssignment?view=graph-rest-beta&preserve-view=true)。
- [设置 SharePoint 资源文件夹](/graph/api/educationsubmission-setupresourcesfolder?view=graph-rest-beta&preserve-view=true)，以在同一位置上传和存储所有基于文件的资源（例如 Word 或 Excel 文件），从而进行 [educationSubmission](/graph/api/resources/educationsubmission?view=graph-rest-beta&preserve-view=true)。

### <a name="identity-and-access--governance"></a>身份和访问 | 治理
- 通过[筛选已登录用户](/graph/api/accesspackageassignment-filterbycurrentuser?view=graph-rest-beta&preserve-view=true)获取一批 [accessPackageAssignment](/graph/api/resources/accessPackageAssignment?view=graph-rest-beta&preserve-view=true) 资源。
- 通过[筛选已登录用户](/graph/api/accesspackageassignmentrequest-filterbycurrentuser?view=graph-rest-beta&preserve-view=true)获取一批 [accessPackageAssignmentRequest](/graph/api/resources/accessPackageAssignmentRequest?view=graph-rest-beta&preserve-view=true) 资源。

### <a name="use-sdks"></a>使用 SDK
试用 [Microsoft Graph .NET SDK v4](https://www.nuget.org/packages/Microsoft.Graph/4.0.0-preview.4) 预览版，并利用以下改进功能：
- 使用单个 API 对 Microsoft Graph 和 Azure .NET 客户端进行身份验证。
- 针对 JSON 序列化和反序列化的新支持。
- 轻松访问响应信息。
- 升级依赖项的更好体验。


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
