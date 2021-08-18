---
title: Microsoft Graph 早期版本的亮点
description: Microsoft Graph 早期版本中的新增功能
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 4240678b35a4a309c5d3d53bed7b2955c16cb84e
ms.sourcegitcommit: b7e01a1331abe5f5c9aa2828d93dad08229573f1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58336861"
---
# <a name="highlights-of-earlier-releases"></a>早期版本的亮点

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

## <a name="april-2021-new-and-generally-available"></a>2021 年 4 月：新增功能，正式可用

### <a name="identity-and-access--identity-and-sign-in"></a>身份和访问 | 身份和登录
- 在租户级别[管理身份验证策略](/graph/api/resources/authenticationflowspolicy)，以启用或禁用外部用户的[自服务注册](/graph/api/resources/selfservicesignupauthenticationflowconfiguration)。
- 管理员可以将用户流与与外部用户共享的应用程序相关联，并在这些应用程序上启用[自助注册](/azure/active-directory/external-identities/self-service-sign-up-overview)。 他们可以定制义自助注册用户流，并创建个性化的注册体验。 应用程序与用户流相关联后，进入该应用程序的用户将能够启动一个提供来宾帐户的注册流。
- 在 Azure AD 租户中配置[用户流属性](/graph/api/resources/identityuserflowattribute)可让你在注册期间收集用户相关信息。 您可以收集一组内置属性，或配置自定义用户流属性来收集来自未内置于目录的用户的信息。 
- 在 [Azure Active Directory 用户](/graph/api/resources/b2xidentityuserflow)中，可管理语言默认值， [自定义在用户流中显示给用户的语言和字符串](/graph/api/resources/userflowlanguageconfiguration)。
- 在用于 Azure AD 自助服务注册和 Azure AD B2C 注册的用户流中使用 [API 连接器](/graph/api/resources/identityapiconnector)，以在特定步骤调用 API 以影响用户流的执行。

### <a name="teamwork"></a>团队合作
- 如果 [chatMessage](/graph/api/resources/chatmessage) 在 [频道](/graph/api/resources/channel)内，则通过 **channelIdentity** 属性标识频道。
- 如果 **[chatMessage](/graph/api/resources/chatmessage)** 在 [聊天](/graph/api/resources/chat)中，则通过 **chatId** 属性识别聊天。
- 使用 **关系** ，通过聊天或 [获取](/graph/api/resources/chatmessage) 聊天中的 [邮件](/graph/api/resources/chat)。
- 使用应用程序权限来[获取](/graph/api/chat-get)指定[聊天](/graph/api/resources/chat)的属性。
- 使用应用程序权限来[获取指定的聊天成员](/graph/api/chat-get-members)或[获取聊天中包括的所有聊天成员](/graph/api/chat-list-members)。 由于作为聊天成员的用户的数据是敏感数据，除获取应用程序权限外，请[请求对这些操作的其他访问权限](teams-protected-apis.md)。 

### <a name="use-the-toolkit"></a>使用工具包
第一次使用 [Microsoft Graph 工具包](/graph/toolkit/overview)？请尝试使用新的[工具包学习路径](/learn/paths/m365-msgraph-toolkit/?WT.mc_id=m365-19989-cxa)，使用工具包的 Web 组件和身份验证提供程序集将 Web 应用连接到 Microsoft Graph，并加载来自 Microsoft 365 的数据。

## <a name="april-2021-new-in-preview-only"></a>2021 年 4 月：仅预览版新增功能

### <a name="cloud-communications--online-meetings"></a>云通信 | 联机会议
- 通过onlineMeeting的 **meetingAttendanceReport** 属性获取预定的在线会议中 [每个与会者的出席情况](/graph/api/resources/attendancerecord?view=graph-rest-beta&preserve-view=true)的 [报告](/graph/api/resources/meetingattendancereport?view=graph-rest-beta&preserve-view=true)。
- 使用 "allowMeetingChat **属性为联机会议启用、禁用** 或限制聊天持续时间。
- 通过使用 **allowTeamworkReactions** 属性来启用或禁用联机会议的响应。

### <a name="compliance"></a>合规性
[将](/graph/api/ediscovery-settings-get?view=graph-rest-beta&preserve-view=true)、 [更新](/graph/api/ediscovery-settings-update?view=graph-rest-beta&preserve-view=true)或 [重置为默认](/graph/api/ediscovery-settings-resettodefault?view=graph-rest-beta&preserve-view=true) 以下 [设置](/graph/api/resources/ediscovery-settings?view=graph-rest-beta&preserve-view=true) 用于电子数据 [大小写](/graph/api/resources/ediscovery-case?view=graph-rest-beta&preserve-view=true)：
- 通过 **redundancyDetection** 属性 [检测重复项，近重复项](/microsoft-365/compliance/near-duplicate-detection-in-advanced-ediscovery?view=o365-worldwide&preserve-view=true)和 [电子邮件线程](/microsoft-365/compliance/email-threading-in-advanced-ediscovery?view=o365-worldwide&preserve-view=true)。
- [通过主题](/microsoft-365/compliance/themes-in-advanced-ediscovery?view=o365-worldwide&preserve-view=true) 属性，识别审阅集文档中一 **理念** 主题。
- 通过 **ocr** 属性，[通过光学字符识别（OCR）从图像文件中提取文本](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery?view=o365-worldwide&preserve-view=true#optical-character-recognition-ocr)。

这些设置提供了分析功能，可以在 [Advanced eDiscovery](/microsoft-365/compliance/overview-ediscovery-20?view=o365-worldwide&preserve-view=true)的端到端工作流程中[智能地挑选数据](/microsoft-365/compliance/overview-ediscovery-20?view=o365-worldwide&preserve-view=true#cull-data-intelligently)。

### <a name="devices-and-apps--device-updates"></a>设备和应用|设备更新
Windows Update for Business 部署服务的 API 的系列。 该服务支持在设备上部署 Windows 10 功能更新和重要 Windows 10 安全更新。 若要了解更多信息，请首先查看 [Windows 更新 API 概述](windowsupdates-concept-overview.md)。

### <a name="education"></a>教育版
- 将文件夹与 [educationAssignment](/graph/api/resources/educationAssignment?view=graph-rest-beta&preserve-view=true) ，通过 **resourcesFolderUrl** 属性来存储所有相关文件资源。
- 通过 [webUrl](/graph/api/resources/educationAssignment?view=graph-rest-beta&preserve-view=true) 属性 **educationAssignment** 链接。

### <a name="identity-and-access--governance"></a>身份和访问 | 治理
管理员可以使用[accessReviewPolicy](/graph/api/resources/accessreviewpolicy?view=graph-rest-beta&preserve-view=true)资源在目录级别[获取](/graph/api/accessreviewpolicy-get?view=graph-rest-beta&preserve-view=true)或[更新](/graph/api/accessreviewpolicy-update?view=graph-rest-beta&preserve-view=true)策略以查看访问权限。 例如，管理员可使用访问审阅策略来启用或禁用查看自己拥有组的访问权限的组所有者。

### <a name="search"></a>搜索
为用户查询[启用拼写建议或更正](search-concept-speller.md)。 这适用于用户查询包含键入错误或错误呈现无搜索结果时。

### <a name="teamwork"></a>团队合作
- 使用 [资源特定的权限](/graph/api/resources/resourcespecificpermissiongrant?view=graph-rest-beta&preserve-view=true) ，列出有权访问指定的 [组或](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) 或 [权限的应用](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true)。
- [获取](/graph/api/teamsappicon-get?view=graph-rest-beta&preserve-view=true)与 Teams 应用关联的 [图标](/graph/api/resources/teamsAppIcon?view=graph-rest-beta&preserve-view=true)属性。 若要获取图标的实际图像，请使用 [获取托管内容](/graph/api/teamworkhostedcontent-get?view=graph-rest-beta&preserve-view=true)。

### <a name="use-sdks"></a>使用 SDK
- 试用 [Microsoft Graph JavaScript 客户端库版本 3.0.0 的预览版本](https://www.npmjs.com/package/@microsoft/microsoft-graph-client/v/3.0.0-Preview.1)。此版本可实现多个身份验证流、服务器端身份验证、Node.js Stream 大型文件上传和进度跟踪等。请参阅[升级指南](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/changelogs/v3-upgrade-guide.md)了解详细信息。
- 尝试新的学习路径， 以[探索用于 JavaScript 开发的 Microsoft Graph 方案](/learn/paths/m365-msgraph-scenarios/?WT.mc_id=m365-16105-cxa)。


## <a name="march-2021-new-and-generally-available"></a>2021 年 3 月: 新版本和正式版

### <a name="applications"></a>应用程序
- 支持在 Azure AD 应用程序库中 [列出](/graph/api/applicationtemplate-list) 应用程序，并将此类应用程序的实例 [添加](/graph/api/applicationtemplate-instantiate) 到目录中的 [applicationTemplate](/graph/api/resources/applicationtemplate) 资源的 GA。
- 添加此类实例 `Application.ReadWrite.OwnedBy` 时 [仅](/graph/api/applicationtemplate-instantiate) 权限。
- 使用 [servicePrincipal](/graph/api/resources/serviceprincipal) 的 **signInAudience** 属性获取当前应用程序支持的用户帐户。

### <a name="devices-and-apps--cloud-printing"></a>设备和应用 | 云打印
- 适用于通用打印的 [云打印](universal-print-concept-overview.md) GA! 查看 [公告](https://techcommunity.microsoft.com/t5/windows-it-pro-blog/universal-print-is-ready-for-business/ba-p/2176778)，并查看如何 [开始使用通用打印](/universal-print/fundamentals/universal-print-license)。
- 在 [打印任务定义](/graph/api/resources/printtaskdefinition)上[订阅更改通知](universal-print-webhook-notifications.md)或[打印机](/graph/api/resources/printer)资源。

### <a name="identity-and-access--governance"></a>身份和访问 | 治理
- 使用 Azure Active Directory （Azure AD） [许可请求](/graph/api/resources/consentrequests-root) 管理尝试访问需要管理员审批的应用的用户的请求工作流。API 使用以下资源：
  - [adminConsentRequestPolicy](/graph/api/resources/adminconsentrequestpolicy) 一个资源，用于创建和管理组织的应用访问请求。
  - [appConsentRequest](/graph/api/resources/appconsentrequest)一个资源，用于聚合和管理用户访问特定应用的请求。
  - [userConsentRequest](/graph/api/resources/userConsentRequest)一个资源，用于请求访问需要管理员授权的用户。 
  - [accessReviewReviewer用户](/graph/api/resources/accessReviewReviewerScope) 资源定义 **adminConsentRequestPolicy** 中指定的用户，用于查看 **appConsentRequest** 和 **userConsentRequest** 对象。
  - 审批 [资源](/graph/api/resources/approval) 表示对请求的批准决定。
- 支持租户在 Azure AD 中自定义 [使用条款](/graph/api/resources/agreement) API 的 GA。

### <a name="identity-and-access--identity-and-sign-in"></a>身份和访问 | 身份和登录
- [身份验证方法](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta&preserve-view=true)包括 [FIDO2 安全键](/graph/api/resources/fido2authenticationmethod)、[Microsoft Authenticator 应用](/graph/api/resources/microsoftauthenticatorauthenticationmethod)和 [Windows Hello for Business](/graph/api/resources/windowshelloforbusinessauthenticationmethod)。
- GA [身份验证方法策略](/graph/api/resources/authenticationmethodspolicies-overview) 定义身份验证方法，允许使用这些方法在 Azure AD 中登录并执行多重身份验证 （MFA） 的用户。 可在 Microsoft Graph 中管理的身份验证方法策略包括 [FIDO2 安全密钥](/graph/api/resources/fido2authenticationmethodconfiguration)、使用 [Microsoft Authentic](/graph/api/resources/microsoftauthenticatorauthenticationmethodconfiguration)ator 应用登录无密码电话登录以及租户的 [电子邮件 OTP 身份验证方法策略](/graph/api/resources/emailauthenticationmethodconfiguration)。
- GA [功能推出策略](/graph/api/resources/featureRolloutPolicy) ，帮助租户管理员在为整个组织启用这些功能之前对特定组进行功能试点。
- 组织品牌 [GA](/graph/api/resources/organizationalbrandingproperties) ，用于自定义 Azure Active Directory 登录屏幕的外观。 组织可根据工作地点自定义特定用户。

### <a name="tasks-and-plans"></a>任务和计划
- 使用权限的委派 `Tasks.Read` 读取所有 Planner 资源的操作。
- 使用权限的委派 `Tasks.ReadWrite` 读取和写入所有 Planner 资源的操作。

### <a name="teamwork"></a>团队合作
- [聊天](/graph/api/resources/chat) 操作、[对话邮件](/graph/api/resources/conversationmember)、聊天 [应用](/graph/api/resources/teamsappinstallation)、聊天 [选项卡](/graph/api/resources/teamstab)及其方法。
- 代表了 Microsoft Teams 应用目录中应用版本细节的[teamsAppDefinition](/graph/api/resources/teamsAppDefinition) GA 的一些更多属性，其中包括:
  - **createdBy**、**描述**、**shortDescription**、**lastModifiedDateTime**
  - **publishingState**，可以是`submitted`中之一和由管理员发布的正在审核、`published`、或`rejected` 中的状态
  - [teamworkBot](/graph/api/resources/teamworkbot) 类型的 **机器人** 关系，表示 Teams 应用清单中指定的机器人的详细信息。
- 使用活动源通知 API 在三个环境中更好地让用户参与：
  - [在聊天中向用户发送通知](/graph/api/chat-sendactivitynotification)
  - [向团队中的用户发送通知](/graph/api/team-sendactivitynotification)
  - [向用户发送通知](/graph/api/userteamwork-sendactivitynotification)
- 将用户的消息历史记录和数据从外部系统迁移到 Teams 频道，使用户能够顺畅地继续通信。使用以下支持迁移方案的方法：
  - [创建团队](/graph/api/team-post)
  - [创建频道](/graph/api/channel-post)
  - [在频道中创建 chatMessage](/graph/api/channel-post-messages)
  - [在渠道中回复消息](/graph/api/channel-post-messagereply)
  - [在团队中完成邮件迁移](/graph/api/team-completemigration)
  - [在频道中完成邮件迁移](/graph/api/channel-completemigration)
- [列表](/graph/api/chatmessage-list-chatmessagehostedcontents) 或 [获取](/graph/api/chatmessagehostedcontent-get) [chatMessage](/graph/api/resources/chatmessage) 中的丰富内容，如图片或代码片段。
- 订阅 chatMessage `ChannelMessage.Read.All` 资源 [更改通知的委派权限](/graph/api/resources/chatmessage) 支持。

## <a name="march-2021-new-in-preview-only"></a>2021 年 3 月：仅限预览版中的新增功能

### <a name="applications"></a>应用程序
[创建自签名证书证书](/graph/api/servicePrincipal-addTokenSigningCertificate?view=graph-rest-beta&preserve-view=true) 添加到 SAML 应用程序。借助此功能，允许 Azure AD 对 SAML 响应进行签名，帮助租户中启用 Azure AD 库应用单一登录。

### <a name="devices-and-apps--cloud-pc"></a>设备和应用 | 云电脑
添加到 [cloudPcDeviceImage](/graph/api/resources/cloudpcdeviceimage?view=graph-rest-beta&preserve-view=true) 资源之后，上传设备源映像失败再出现两个原因：操作系统不受支持 （`osVersionNotSupported`）， 或者预配 Windows 虚拟机 （`sourceImageInvalid`） 的源映像无效。

### <a name="devices-and-apps--cloud-printing"></a>设备和应用 | 云打印
当打印机与通用打印交互时，获取最近日期/时间 (**lastSeenDateTime** 属性)。

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理
Intune [3](https://developer.microsoft.com/graph/changelog/?from=2021-03-01&to=2021-03-31&filterBy=Corporate%20management) beta 版更新。

### <a name="identity-and-access--governance"></a>身份和访问 | 治理
将新模型 [访问权限审阅](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true) 组成员身份和所有其他支持的资源类型。弃用[旧访问审阅模式](/graph/api/resources/accessreviews-root?view=graph-rest-beta&preserve-view=true)。

### <a name="sites-and-lists"></a>网站和列表
- 通过 [contentType](/graph/api/resources/contentType?view=graph-rest-beta&preserve-view=true) 实体上的一组新属性和方法，支持特定站点集合中文档或文档集的特定内容类型或模板。方法包括下列几种：
  - [addCopy](/graph/api/contenttype-addcopy?view=graph-rest-beta&preserve-view=true)
  - [associateWithHubSites](/graph/api/contenttype-associatewithhubsites?view=graph-rest-beta&preserve-view=true)
  - [copyToDefaultContentLocation](/graph/api/contenttype-copytodefaultcontentlocation?view=graph-rest-beta&preserve-view=true)
  - [isPublished](/graph/api/contenttype-ispublished?view=graph-rest-beta&preserve-view=true)
  - [发布](/graph/api/contenttype-publish?view=graph-rest-beta&preserve-view=true)
  - [取消发布](/graph/api/contenttype-unpublish?view=graph-rest-beta&preserve-view=true)
- 按其列标签自定义内容类型。列由 [columnDefinition](/graph/api/resources/columndefinition?view=graph-rest-beta&preserve-view=true) 实体表示，并支持全套的 CRUD 操作。
- [获取可应用于列表上网站的内容类型](/graph/api/site-getApplicableContentTypesForList?view=graph-rest-beta&preserve-view=true)。
- 按 **columnDefinition** 实体中的下列属性来区分列类型: 布尔型、计算型、选择型、货币型、日期时间型、查找型、数字型、人或组型、文本型。这些属性是互斥的。

### <a name="sites-and-lists--taxonomy"></a>网站和列表 | 分类
- 使用术语库 [关系](/graph/api/resources/site?view=graph-rest-beta&preserve-view=true)[termStore](/graph/api/resources/termstore-store?view=graph-rest-beta&preserve-view=true)导航到 **术语** 存储。
- 反之，则使用 **parentSiteId** 属性获取术语库的父站点的ID。

### <a name="users"></a>用户
- [通过](/graph/api/regionalandlanguagesettings-get?view=graph-rest-beta&preserve-view=true) 或 [更新](/graph/api/regionalandlanguagesettings-update?view=graph-rest-beta&preserve-view=true) 用户 [对翻译语言的偏好](/graph/api/resources/translationpreferences?view=graph-rest-beta&preserve-view=true)。例如，是否翻译、自动翻译、或在翻译消息、聊天和网页中的特定语言之前提示，以及进行任何 [翻译覆盖](/graph/api/resources/translationlanguageoverride?view=graph-rest-beta&preserve-view=true)。
- [为用户激活](/graph/api/user-activateServicePlan?view=graph-rest-beta&preserve-view=true) 计划许可证。


## <a name="february-2021-new-and-generally-available"></a>2021 年 2 月：新版本和正式版

### <a name="cloud-communications--online-meeting"></a>云通信 | 联机会议
对[onlineMeeting](/graph/api/resources/onlinemeeting)资源的操作和方法使用基于策略的 `OnlineMeetings.Read.All` 或 `OnlineMeetings.ReadWrite.All` 应用程序权限。 这意味着管理员可以[配置应用访问策略](cloud-communication-online-meeting-application-access-policy.md)，允许应用代表用户访问在线会议。

### <a name="sites-and-lists"></a>网站和列表
使用 [权限](/graph/api/resources/permission) 资源及其 CRUD 操作来管理为 [driveItem](/graph/api/resources/driveitem) 授予的共享权限。 带链接面的权限代表共享项目上创建的链接。 带有邀请面的权限表示通过邀请特定用户或组访问文件而增加的权限。

## <a name="february-2021-new-in-preview-only"></a>2021 年 2 月：仅限预览版中的新增功能

### <a name="applications"></a>应用程序
对 [同步 API](/graph/api/resources/synchronization-overview?view=graph-rest-beta&preserve-view=true) 使用应用程序权限，这些 API 可在 Azure AD 中自动供应 (创建、维护) 和取消供应 (删除) 身份。

### <a name="cloud-communications--calls"></a>云通信 | 呼叫
支持[基于政策的通话录音](/microsoftteams/teams-recording-policy)，使用管理政策自动记录通话，以便根据相关企业或监管政策的要求进行后续处理和保留。 在基于策略的参与者加入呼叫之前，策略规定向与策略相关联的具有处理新参与者的可用能力的机器人发送一个 [participantJoiningNotification ](/graph/api/resources/participantJoiningNotification?view=graph-rest-beta&preserve-view=true)。 机器人在其响应有效载荷中会以 [acceptJoinResponse](/graph/api/resources/acceptjoinresponse?view=graph-rest-beta&preserve-view=true)、[rejectJoinResponse](/graph/api/resources/rejectjoinresponse?view=graph-rest-beta&preserve-view=true) 或 [inviteNewBotResponse](/graph/api/resources/invitenewbotresponse?view=graph-rest-beta&preserve-view=true) 中的一个来响应。

### <a name="compliance--ediscovery"></a>合规性 | 电子数据展示
- 为了诉讼、内部调查或其他法律操作的目的，使用 [legalHold](/graph/api/resources/ediscovery-legalhold?view=graph-rest-beta&preserve-view=true) 资源及其 API 来无限期地保护不删除其内容。
- 使用 [sourceCollection](/graph/api/resources/ediscovery-sourcecollection?view=graph-rest-beta&preserve-view=true) 资源及其 API 来搜索和识别 Microsoft 365 中保管和非保管位置的相关文档。
- 在审查过程中使用 [标记](/graph/api/resources/ediscovery-tag?view=graph-rest-beta&preserve-view=true) 资源和 API 来标记文档，以分离响应式和非响应式内容。
- 从[审阅集](/graph/api/resources/ediscovery-reviewset?view=graph-rest-beta&preserve-view=true)中[导出](/graph/api/ediscovery-reviewset-export?view=graph-rest-beta&preserve-view=true)文档。
- 使用 [AddToReviewSet](/graph/api/ediscovery-reviewset-addtoreviewset?view=graph-rest-beta&preserve-view=true) 操作将 **sourceCollection** 中的文档添加到 **reviewSet** 中。
- 根据[审阅集查询](/graph/api/resources/ediscovery-reviewsetquery?view=graph-rest-beta&preserve-view=true)将[标签应用](/graph/api/ediscovery-reviewsetquery-applytags?view=graph-rest-beta&preserve-view=true)到文档中。
- 在 `microsoft.graph.ediscovery` 命名空间中定义了所有 eDiscovery API。
- 将委托权限模式由 `User.Read` 改为 `eDiscovery.Read.All` 和 `eDiscovery.ReadWrite.All`。

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理
- Intune [2月](https://developer.microsoft.com/graph/changelog/?from=2021-02-01&to=2021-02-28&filterBy=Corporate%20management) 更新的测试版。
- Intune 在 [设备](/graph/api/resources/device?view=graph-rest-beta&preserve-view=true) 资源上设置的新属性: **deviceCategory**、**deviceOwnership**、**domainName**、**enrollmentProfileName**、**enrollmentType**、**isRooted**、**managementType** 和 **registrationDateTime**。

### <a name="education"></a>教育版
使用 [educationAssignmentDefaults](/graph/api/resources/educationAssignmentDefaults?view=graph-rest-beta&preserve-view=true) 来指定课堂作业的默认操作，例如，作业到期时间、作业通知的频道 URL。仍然可以在创建任务时自定义值。

### <a name="identity-and-access--identity-and-sign-in"></a>身份和访问 | 身份和登录
- 使用 [smsAuthenticationMethodConfiguration](/graph/api/resources/smsAuthenticationMethodConfiguration?view=graph-rest-beta&preserve-view=true) 资源以 [获取](/graph/api/smsauthenticationmethodconfiguration-get?view=graph-rest-beta&preserve-view=true)、[更新](/graph/api/smsauthenticationmethodconfiguration-update?view=graph-rest-beta&preserve-view=true) 或 [删除](/graph/api/smsauthenticationmethodconfiguration-delete?view=graph-rest-beta&preserve-view=true) 组织中短信身份验证策略的配置设置。
- 使用 [temporaryAccessPassAuthenticationMethodConfiguration](/graph/api/resources/temporaryaccesspassauthenticationmethodconfiguration?view=graph-rest-beta&preserve-view=true) 资源以 [获取](/graph/api/temporaryaccesspassauthenticationmethodconfiguration-get?view=graph-rest-beta&preserve-view=true)、[更新](/graph/api/temporaryaccesspassauthenticationmethodconfiguration-update?view=graph-rest-beta&preserve-view=true) 和 [删除](/graph/api/temporaryaccesspassauthenticationmethodconfiguration-delete?view=graph-rest-beta&preserve-view=true) 组织中临时访问传递身份验证策略的配置设置。

### <a name="identity-and-access--governance"></a>身份和访问 | 治理
- 在 [[访问包分配请求](/graph/api/resources/accesspackage?view=graph-rest-beta&preserve-view=true)，将地理位置信息分配给](/graph/api/resources/accesspackageassignmentrequest?view=graph-rest-beta&preserve-view=true)。
- 获取所有表示 SharePoint Online 资源存储地理位置的[访问包资源环境](/graph/api/resources/accesspackageresourceenvironment?view=graph-rest-beta&preserve-view=true)的列表。
- 对下列资源的操作使用应用权限 (`EntitlementManagement.Read.All` 或 `EntitlementManagement.ReadWrite.All`):
  - [accessPackage](/graph/api/resources/accesspackage?view=graph-rest-beta&preserve-view=true)
  - [accessPackageAssignment](/graph/api/resources/accesspackageassignment?view=graph-rest-beta&preserve-view=true)
  - [accessPackageAssignmentPolicy](/graph/api/resources/accesspackageassignmentpolicy?view=graph-rest-beta&preserve-view=true)
  - [accessPackageAssignmentRequest](/graph/api/resources/accesspackageassignmentrequest?view=graph-rest-beta&preserve-view=true)
  - [accessPackageAssignmentResourceRole](/graph/api/resources/accesspackageassignmentresourcerole?view=graph-rest-beta&preserve-view=true)
  - [accessPackageCatalog](/graph/api/resources/accesspackagecatalog?view=graph-rest-beta&preserve-view=true)
  - [accessPackageResourceRequest](/graph/api/resources/accesspackageresourcerequest?view=graph-rest-beta&preserve-view=true)
  - [connectedOrganization](/graph/api/resources/connectedorganization?view=graph-rest-beta&preserve-view=true)
  - [entitlementManagementSettings](/graph/api/resources/entitlementmanagementsettings?view=graph-rest-beta&preserve-view=true)

### <a name="reports--microsoft-365-usage-reports"></a>报告 | Microsoft 365 使用情况报告
在[SharePoint站点使用情况的详细报告](/graph/api/reportroot-getsharepointsiteusagedetail?view=graph-rest-beta&preserve-view=true)中获取更多属性：anonymousLinkCount、companyLinkCount、externalSharing、地理位置、secureLinkForGuestCount、secureLinkForMemberCount、siteSensitivityLabelId 和 unmanagedDevicePolicy。

### <a name="tasks-and-plans"></a>任务和计划
- 在计划的 [计划详细信息](/graph/api/resources/plannerplandetails?view=graph-rest-beta&preserve-view=true) 对象中最多定义 25 个类别。 对于每个类别指定一个描述性标签，并将计划中的任务与一个或多个类别联系起来。 
- 使用 [名单](/graph/api/resources/plannerRoster?view=graph-rest-beta&preserve-view=true) 来表示在 [计划](/graph/api/resources/plannerplan?view=graph-rest-beta&preserve-view=true) 上协作的用户集合。 使用 **rosterPlans** 关系以获取该用户的 [成员](/graph/api/resources/plannerrostermember?view=graph-rest-beta&preserve-view=true) 名单。 
- 对于在 Planner 之外的体验中显现的计划 (如 Microsoft Teams)，在 [计划上下文中详细](/graph/api/resources/plannerplancontextdetails?view=graph-rest-beta&preserve-view=true) 中指定如何显示到 [计划上下文](/graph/api/resources/plannerPlanContext?view=graph-rest-beta&preserve-view=true) 的链接。 

### <a name="use-sdks"></a>使用 SDK
请试用[Microsoft Graph Java SDK v3](https://github.com/microsoftgraph/msgraph-sdk-java/tree/feature/v3)预览版！ 更多信息，请看相关[博客文章](https://developer.microsoft.com/graph/blogs/announcing-the-public-preview-of-microsoft-graph-java-sdk-v3/)。

## <a name="january-2021-new-in-preview-only"></a>2021 年 1 月：仅限预览版新增功能

### <a name="cloud-communications"></a>云通信
- 以 [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true) 的形式组织实时事件 - 参见[示例](/graph/api/application-post-onlinemeetings?view=graph-rest-beta&preserve-view=true#example-3-create-a-live-event-with-a-user-token)。 
- 获取[与会者报告](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true#example-4-retrieve-the-attendee-report-of-a-live-event)、[录制内容](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true#example-5-retrieve-the-recording-of-a-live-event)或实时事件的备选录制的内容流。
- 获取[外出](/graph/api/resources/outofofficesettings?view=graph-rest-beta&preserve-view=true)用户的[状态](/graph/api/resources/presence?view=graph-rest-beta&preserve-view=true)，以及为该状态设置的任何消息。

### <a name="devices-and-apps--cloud-pc"></a>设备和应用 | 云电脑
- 为成功的[本地网络连接](/graph/api/resources/cloudPcOnPremisesConnection?view=graph-rest-beta&preserve-view=true)[更新 Active Directory 域密码](/graph/api/cloudpconpremisesconnection-updateaddomainpassword?view=graph-rest-beta&preserve-view=true)。
- [在本地网络连接上运行运行状况检查](/graph/api/cloudpconpremisesconnection-runhealthcheck?view=graph-rest-beta&preserve-view=true)现在可以在[本地连接运行状态检查](/graph/api/resources/cloudpconpremisesconnectionhealthcheck?view=graph-rest-beta&preserve-view=true)资源中暴露 5 种其他错误类型。 有关错误类型的更多信息，请参阅 2021 年 1 月的[更改日志](https://developer.microsoft.com/graph/changelog)。

### <a name="devices-and-apps--cloud-printing"></a>设备和应用 | 云打印
- [ 订阅更改云打印的通知](universal-print-webhook-notifications.md) - 当打印作业启动时，以及当打印机准备下载打印作业时。
- 获取[打印机](/graph/api/resources/printer?view=graph-rest-beta&preserve-view=true)状态的全部[可能值](/graph/api/resources/printerstatus?view=graph-rest-beta&preserve-view=true#printerprocessingstatedetail-values)。
- 代表已登录用户在应用程序中使用委派权限：
  - `PrinterShare.ReadBasic.All` 读取打印机共享的基本信息，不包括访问控制信息。
  - `PrintConnector.Read.All` 读取打印连接器。
  - `PrintConnector.ReadWrite.All` 读取或写入打印连接器。
  - `PrintJob.Create` 创建打印作业并将内容上载到打印作业。
  - `PrintSettings.Read.All` 读取租户范围的打印设置。
  - `PrintSettings.ReadWrite.All` 读取或写入租户范围的打印设置。
  - `Reports.Read.All` 读取每个指定用户或每个打印机的打印使用情况摘要。

### <a name="education"></a>教育版
使用班级[作业设置](/graph/api/resources/educationAssignmentSettings?view=graph-rest-beta&preserve-view=true)来启用或禁用动画来以庆祝交作业。

### <a name="groups"></a>组
使用 **membershipRuleProcessingStatus** 属性获取基于规则的动态组的处理状态。当用户的属性发生更改时，此选项非常有用，用户在基于规则的 [Microsoft 365 组](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true)中的会员资格将根据为组织设置的组会员资格规则重新评估。 

### <a name="identity-and-access--directory-management"></a>身份和访问 | 目录管理
获取用户或设备对构建在PowerApps上的第三方软件的[使用权](/graph/api/resources/UsageRight?view=graph-rest-beta&preserve-view=true)，或者，设备对订阅的使用权。 使用权包括相应服务或产品的标识符，以及使用权的当前状态，如激活、未激活、警告或暂停。

### <a name="identity-and-access--identity-and-sign-in"></a>身份和访问 | 身份和登录
- 应用可以使用应用程序权限，让管理员管理用户的 [身份验证方法](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta&preserve-view=true)。
- 支持 [Microsoft Authenticator](/graph/api/resources/microsoftauthenticatorauthenticationmethod?view=graph-rest-beta&preserve-view=true) 作为用户登录或对 Azure AD 执行多因素身份验证的身份验证方法。
- 使用 [Microsoft Authenticator 策略](/graph/api/resources/microsoftauthenticatorauthenticationmethodconfiguration?view=graph-rest-beta&preserve-view=true)可以定义配置设置以及启用 Microsoft Authenticator 作为身份验证方法的用户或组。 使用 Microsoft Authenticator 策略代替已弃用的 [Microsoft Authenticator 无密码手机登录策略](/graph/api/resources/passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration?view=graph-rest-beta&preserve-view=true)。 
- 支持 [Windows Hello 企业版](/graph/api/resources/windowshelloforbusinessauthenticationmethod?view=graph-rest-beta&preserve-view=true)作为用户在不使用密码的情况下登录 Windows 设备的身份验证方法。

### <a name="reports--identity-and-access-reports"></a>报告 | 身份和访问报告
- [获取注册用户数的报告，或能够使用各种注册功能的用户数](/graph/api/authenticationmethodsroot-usersregisteredbyfeature?view=graph-rest-beta&preserve-view=true)，包括多因素认证、自助密码重置或无密码认证。
- [获取每种认证方式的注册用户数报告](/graph/api/authenticationmethodsroot-usersregisteredbymethod?view=graph-rest-beta&preserve-view=true)，包括密码、Windows Hello 企业版或无密码电话登录。

## <a name="december-2020-new-and-generally-available"></a>2020 年 12 月：新版本和正式版

### <a name="calendar"></a>日历
- 会议组织者可以使用 [事件](/graph/api/resources/event)的 **hideAttendees** 属性来控制与会者是否可以在会议“**跟踪**”列表中看到彼此。
- 组织者可用的 **isDraft** 属性和 [cancel](/graph/api/event-cancel) 方法的 GA，以及组织者和与会者可用的 [forward](/graph/api/event-forward) 方法的 GA，以更好地管理日历中的 [事件](/graph/api/resources/event)资源。
- [日历](/graph/api/resources/calendar) 的 **hexColor** 和 **isDefault** 属性的 GA 可以更好地管理日历。

### <a name="cloud-communications"></a>云通信
[状态](/graph/api/resources/presence)资源的 GA，允许获取一个或多个用户的状态信息，例如他们的可用性和用户活动。

### <a name="identity-and-access--identity-and-sign-in"></a>身份和访问 | 身份和登录
尝试新[教程](tutorial-riskdetection-api.md)，学习如何使用[身份保护 API ](/graph/api/resources/identityprotectionroot)来识别风险，并配置工作流以确认泄露或启用修复。

### <a name="teamwork"></a>团队合作
- [API 管理 Teams 应用安装](/graph/api/resources/teamsappinstallation) 的 GA，包括获取团队或用户个人范围内的 应用，或者添加、删除或更新该应用。
- [获取用户和 Teams 应用间的聊天](/graph/api/userscopeteamsappinstallation-get-chat)。

### <a name="use-the-toolkit"></a>使用工具包
Microsoft Graph 工具包 2.0 的 GA 版本 - 此版本包含新 [Microsoft Graph 待办任务组件](./toolkit/components/todo.md)（与 [Planner 任务组件](./toolkit/components/tasks.md)不同），以及增强的[个人卡片组件](./toolkit/components/person-card.md)。有关更多信息，请参见[相关博客文章](https://developer.microsoft.com/graph/blogs/announcing-the-general-availability-of-microsoft-graph-toolkit-2-0/)。


## <a name="december-2020-new-in-preview-only"></a>2020 年 12 月：仅限预览版的新增功能

### <a name="compliance--ediscovery"></a>合规性 | 电子数据展示
继续实现 [Microsoft 365 合规 API](/graph/api/resources/ediscoveryapioverview?view=graph-rest-beta&preserve-view=true) 的管道是[保管人](/graph/api/resources/custodian?view=graph-rest-beta&preserve-view=true)资源及其相关操作和方法，以[释放](/graph/api/custodian-release?view=graph-rest-beta&preserve-view=true)或[激活](/graph/api/custodian-activate?view=graph-rest-beta&preserve-view=true)保管人。 使用 **保管人** 资源可以访问 Exchange Online 邮箱、OneDrive for Business、SharePoint 网站 ([siteSource](/graph/api/resources/siteSource?view=graph-rest-beta&preserve-view=true)) 和 Microsoft 365 组([unifiedGroupSource](/graph/api/resources/unifiedGroupSource?view=graph-rest-beta&preserve-view=true)) 中保管人的数据 ([userSource](/graph/api/resources/userSource?view=graph-rest-beta&preserve-view=true))。

### <a name="devices-and-apps--cloud-pc"></a>设备和应用 | 云电脑
在 [cloudPC](/graph/api/resources/cloudpc?view=graph-rest-beta&preserve-view=true) 资源的 **status** 属性中，将云管理虚拟机的故障状态统称为 `failed`。

### <a name="devices-and-apps--cloud-printing"></a>设备和应用 | 云打印
- [更新](/graph/api/printjob-update-configuration?view=graph-rest-beta&preserve-view=true)[打印作业](/graph/api/resources/printjob?view=graph-rest-beta&preserve-view=true)的[配置](/graph/api/resources/printjobconfiguration?view=graph-rest-beta&preserve-view=true)。
- 有关重命名一些属性和重新键入关系的详细信息，请参阅 API 更改日志的 [2020 年 12 月](https://developer.microsoft.com/graph/changelog/)部分。

### <a name="education"></a>教育版
- 如果作业发布后添加了学生，教师可以通过使用 [educationAssignment](/graph/api/resources/educationAssignment?view=graph-rest-beta&preserve-view=true) 资源的 **addedStudentAction** 属性来控制作业行为。
- 教师可以通过 **educationAssignment** 资源的 **notificationChannelUrl** 属性发布作业发布通知。

### <a name="identity-and-access"></a>身份和访问
获取或设置 Azure AD [使用条款](/graph/api/resources/agreement?view=graph-rest-beta&preserve-view=true)[协议](/graph/api/resources/agreement?view=graph-rest-beta&preserve-view=true)、[协议文件](/graph/api/resources/agreementfile?view=graph-rest-beta&preserve-view=true)和 [agreementfilelocalization](/graph/api/resources/agreementfilelocalization?view=graph-rest-beta&preserve-view=true) 的版本和创建元数据。

### <a name="identity-and-access--governance"></a>身份和访问 | 治理
作为 Azure Active Directory [权利管理](/graph/api/resources/entitlementmanagement-root?view=graph-rest-beta&preserve-view=true)的一部分，当希望访问组、应用程序或 SharePoint Online 网站的用户请求分配[访问包](/graph/api/resources/accesspackage?view=graph-rest-beta&preserve-view=true)时，他们现在可以响应[访问包分配请求](/graph/api/resources/accesspackageassignmentrequest?view=graph-rest-beta&preserve-view=true)中[本地化内容](/graph/api/resources/accesspackagelocalizedcontent?view=graph-rest-beta&preserve-view=true)中表示的[问题](/graph/api/resources/accesspackagequestion?view=graph-rest-beta&preserve-view=true)。

### <a name="identity-and-access--identity-and-sign-in"></a>身份和访问 | 身份和登录
- 管理员可以将用户流与与外部用户共享的应用程序相关联，并在这些应用程序上启用[自助注册](/azure/active-directory/external-identities/self-service-sign-up-overview)。 他们可以定制义自助注册用户流，并创建个性化的注册体验。 具体地说，它们建立[用于调用自定义用户流的注册启动事件的侦听器](/graph/api/resources/invokeuserflowlistener?view=graph-rest-beta&preserve-view=true)。 应用程序与用户流相关联后，进入该应用程序的用户将能够启动一个提供来宾帐户的注册流。
- 在 [Azure Active Directory 用户流](/graph/api/resources/b2xidentityuserflow?view=graph-rest-beta&preserve-view=true)或 [Azure Active Directory B2C 租户用户流](/graph/api/resources/b2cidentityuserflow?view=graph-rest-beta&preserve-view=true)中，可以管理语言默认值并[自定义在用户流中显示给用户的语言和字符串](/graph/api/resources/userflowlanguageconfiguration?view=graph-rest-beta&preserve-view=true)。
- 在用于 Azure AD 自助服务注册和 Azure AD B2C 注册的用户流中使用 [API 连接器](/graph/api/resources/identityapiconnector?view=graph-rest-beta&preserve-view=true)，以在特定步骤调用 API 以影响用户流的执行。
- 为租户定义[电子邮件 OTP 身份验证方法策略](/graph/api/resources/emailauthenticationmethodconfiguration?view=graph-rest-beta&preserve-view=true)。

### <a name="teamwork"></a>团队合作
- 对于[团队](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true)、[频道](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true)或[聊天](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true)环境中的[成员](/graph/api/resources/conversationmember?view=graph-rest-beta&preserve-view=true)资源，你现在可以：
  - 区分是 [Azure AD 用户](/graph/api/resources/aaduserconversationmember?view=graph-rest-beta&preserve-view=true)的成员，注意用户 ID、电子邮件地址和 Azure AD 租户 ID。 
  - [添加多个用户作为团队成员](/graph/api/conversationmembers-add?view=graph-rest-beta&preserve-view=true)。
- 对于[聊天](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true)资源：
  - [获取指定用户参与的聊天中的所有消息](/graph/api/chats-getallmessages?view=graph-rest-beta&preserve-view=true)，包括一对一聊天、群聊和会议聊天。
  - 使用所有功能来列出、获取、添加、删除和更新聊天中的[应用程序](/graph/api/resources/teamsappinstallation?view=graph-rest-beta&preserve-view=true)或[选项卡](/graph/api/resources/teamstab?view=graph-rest-beta&preserve-view=true)。
  - 使用 **chatType** 属性可将一对一聊天与群聊或与联机会议关联的聊天区分开来。
  - [创建](/graph/api/chat-post?view=graph-rest-beta&preserve-view=true)或[更新](/graph/api/chat-patch?view=graph-rest-beta&preserve-view=true)聊天。
  - 对于聊天上下文中的成员，请使用 **visibleHistoryStartDateTime** 属性设置或获取表示与该成员共享会话历史时间段的时间戳。
  - 在指定的聊天室中[创建](/graph/api/chat-post-members?view=graph-rest-beta&preserve-view=true)或[删除](/graph/api/chat-delete-members?view=graph-rest-beta&preserve-view=true)成员。 
- 对于[频道](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true)资源：
  - [通过团队中的所有频道获取所有消息](/graph/api/channels-getallmessages?view=graph-rest-beta&preserve-view=true)。
  - 团队所有者可以启用 [频道审核](/graph/api/resources/channelmoderationsettings?view=graph-rest-beta&preserve-view=true)，通过使用该频道的“**审核设置**”属性。以控制谁可以在该频道中发起新帖子或回复帖子。
- 作为 [Teams 应用程序定义](/graph/api/resources/teamsappdefinition?view=graph-rest-beta&preserve-view=true)的一部分，使用 **机器人** 关系连接到 [团队机器人](/graph/api/resources/teamworkbot?view=graph-rest-beta&preserve-view=true)。

### <a name="to-do-tasks"></a>待办任务
订阅[待办任务](/graph/api/resources/todoTask?view=graph-rest-beta&preserve-view=true)的[更改通知](webhooks.md)。


## <a name="november-2020-new-and-generally-available"></a>2020年 11 月：新版本和正式版

### <a name="cloud-communications"></a>云通信
- [meetingParticipantInfo](/graph/api/resources/meetingParticipantInfo) 类型的 **role** 属性 GA，将 [在线会议](/graph/api/resources/onlinemeeting) 中的参会者角色区分为与会者或报告者。
- **lobbyBypassSettings** 属性 GA 以及其 [值](/graph/api/resources/lobbybypasssettings#lobbybypassscope-values) 许可用户加入在线会议。
- **isEntryExitAnnounced** 属性 GA 自定义设置宣布召集者加入或离开在线会议。
- **allowedPresenters** 属性 GA 允许会议中特定报告者。

### <a name="search"></a>搜索
- Microsoft 搜索 [查询 API](/graph/api/resources/search-api-overview)的 GA，支持以下类型数据的范围搜索：
  - [Outlook 邮件](./search-concept-messages.md)
  - [Outlook 日历事件](./search-concept-events.md)
  - [OneDrive 和 SharePoint 资源](./search-concept-files.md)。

### <a name="teamwork"></a>团队合作

- 资源特定许可 (RSC) 权限的正式发布。RSC 权限允许团队所有者向生产应用授予具体同意，以便访问和/或修改团队的特定数据，例如读取团队的设置，或者修改频道的名称、说明及其他设置。
- 适用于 [频道](/graph/api/resources/channel) 或频道内的邮件 Api 的 GA。API 包括：
  - [创建](/graph/api/conversationmember-add) 或 从频道中[删除](/graph/api/conversationmember-delete) 对话成员。
  - [更新频道中成员](/graph/api/conversationmember-update) 的角色。
  - 获取频道中的特定邮件或所有邮件。
  - 获取频道中的特定回复或所有回复。
  - [在频道中跟踪新增的或者已更新的邮件](/graph/api/chatmessage-delta)。


## <a name="november-2020-new-in-preview-only"></a>2020 年 11 月：仅限预览版的新增功能

### <a name="devices-and-apps--cloud-pc"></a>设备和应用 | 云电脑
[云电脑 API](/graph/api/resources/virtualendpoint?view=graph-rest-beta&preserve-view=true) 首次上线，使组织可以预配和管理员工的虚拟桌面。 与 Intune API 配合使用来管理物理和虚拟终结点。

### <a name="devices-and-apps--cloud-printing"></a>设备和应用 | 云打印
在 [打印任务定义](/graph/api/resources/printtaskdefinition?view=graph-rest-beta&preserve-view=true)上[订阅更改通知](webhooks.md)。

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理
Intune beta 版[11 月](changelog.md#november-2020)更新。

### <a name="identity-and-access"></a>身份和访问
- 在 [应用](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true) 的 **spa** 属性中指定发送登录用户令牌的 URL，以及授权代码和访问令牌的URI。
- 通过 [组织品牌属性](/graph/api/resources/organizationalbrandingproperties?view=graph-rest-beta&preserve-view=true) 自定义 Azure Active Directory 登录屏幕的界面外观。 组织可根据工作地点自定义特定用户。

### <a name="identity-and-access--governance"></a>身份和访问 | 治理
[组成员资格访问审查 API](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true) 首次上线，可以定期审查用户访问，确保只有适当人员用户持续访问权，并有效管理组成员资格。

### <a name="search"></a>搜索
可以聚合数值或字符串类型的搜索结果，[Microsoft Graph 连接器](/microsoftsearch/connectors-overview)导入这些结果，并将其在[架构](/graph/api/resources/schema?view=graph-rest-beta&preserve-view=true)中设置为可精简。查看有关[使用聚合优化搜索结果](search-concept-aggregation.md)的更多信息。

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
获取适用于公司员工的[用户](/graph/api/resources/user)新属性：聘用日期、组织协会（如分部和成本中心）和员工类型（如顾问、合同工或供应商）。这些属性要求在GET操作中指定`$select` OData 查询参数。

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
- 管理[身份验证方法](/graph/api/resources/authenticationmethodspolicies-overview?view=graph-rest-beta&preserve-view=true)策略，以识别可以使用特定多重身份验证方法登录 Azure Active Directory 的用户。配置策略以定义以下内容：
  - 可以在 Azure AD 租户中使用的 FIDO2 安全密钥类型。
  - 允许使用 FIDO2 安全密钥或无密码电话登录来登录 Azure AD 的用户或用户组。
- 为用户配置[电子邮件身份验证方法](/graph/api/resources/emailauthenticationmethod?view=graph-rest-beta&preserve-view=true)，以自助重置密码。
- 使用 [Azure AD B2C](/azure/active-directory-b2c/overview) 并[选择一种机制来配置并允许最终用户通过本地帐户进行身份验证](/graph/api/resources/b2cauthenticationmethodspolicy?view=graph-rest-beta&preserve-view=true)。
- 使用 `Policy.ReadWrite.AuthenticationMethod` 来读取或写入组织的身份验证方法策略，作为代表已登录用户的委托权限或不存在已登录用户的情况下的应用程序权限。
- 在[授权策略](/graph/api/resources/authorizationpolicy?view=graph-rest-beta&preserve-view=true)中指定是否以及谁可以邀请外部用户加入组织。

### <a name="people-and-workplace-intelligence--insights"></a>人脉和工作场所智能 | 见解 
管理员可以查看[使用 PowerShell cmdlet 的示例](insights-customize-item-insights-privacy.md#how-to-configure-item-insights-settings-via-powershell)，为组织自定义项目见解设置。

### <a name="teamwork"></a>团队合作
- 使用实例属性 **channelCreationMode** 表明正在创建 [通道](/graph/api/resources/channel?preserve-view=true&view=graph-rest-beta#instance-attributes)以服务数据迁移。 使用 [completeMigration](/graph/api/channel-completemigration?view=graph-rest-beta&preserve-view=true) 表明迁移已结束，以便成员可以发布和阅读邮件。
- 使用实例属性 **teamCreationMode** 表明正在创建 [团队](/graph/api/resources/team?preserve-view=true&view=graph-rest-beta#instance-attributes)以服务迁移。 使用 [completeMigration](/graph/api/team-completemigration?view=graph-rest-beta&preserve-view=true) 表明迁移已结束，以便成员可以操作和发布邮件。

## <a name="september-2020-new-and-generally-available"></a>2020 年 9 月：新版本和正式版

### <a name="calendar"></a>日历
[事件](/graph/api/resources/event)资源的 **transactionId** 属性 GA，可选择由客户端应用程序设置，以避免客户端重试创建相同事件时出现多余的 POST 操作。 当低网络连接性导致客户端在从服务器中收到客户端先前创建事件请求的响应之前超时时，此功能很有用。

### <a name="cloud-communications"></a>云通信
[从[通话](/graph/api/resources/call)中删除参与者](/graph/api/participant-delete)。即使在有必要删除活动通话的参与者的情况下，也可以使用此操作。

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
除通过“**邮件** 属性” 获取 [用户](/graph/api/resources/user) 的 SMTP 地址之外，你现在可以设置该属性并更新用户的电子邮件地址。 

## <a name="september-2020-new-in-preview-only"></a>2020 年 9 月：仅限预览版的新增功能

### <a name="application"></a>应用程序
创建、列出或删除[服务主体](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true)公开的[委派权限分类](/graph/api/resources/delegatedpermissionclassification?view=graph-rest-beta&preserve-view=true)。 将委派权限分类与[用户同意设置](/azure/active-directory/manage-apps/configure-user-consent)结合使用可以对允许最终用户向应用授予同意的条件进行限制。

### <a name="cloud-communications"></a>云通信
- 弃用了 [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true)的 **autoAdmittedUsers** 属性。 使用新的 **lobbyBypassSettings** 属性和 [值](/graph/api/resources/lobbybypasssettings?view=graph-rest-beta&preserve-view=true#lobbybypassscope-values)取而代之。
- 使用宣布呼叫者加入或离开联机会议的其他设置（**isEntryExitAnnounced** 属性），并允许在会议中使用特定演示者（**allowedPresenters** 属性）。

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

  - 获取来自 OneDrive 和 SharePoint 的 [附加类型](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true#scope-search-based-on-entity-types)内容： **驱动器**、 **列表**、 **listItem** 和 **网站**。 
  - 搜索结果中的范围属性设为[所选属性](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true#get-selected-properties)。 
  - 获取 [listItem](/graph/api/resources/listitem?view=graph-rest-beta&preserve-view=true) 资源的自定义属性。
  - 对任何可排序属性上的 OneDrive 和 SharePoint 搜索结果进行[排序](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true#sort-search-results)。
  - [使用针对 OneDrive 和 SharePoint 的聚合](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true#refine-results-using-aggregations)优化结果。
- 查询通过 Microsoft Graph 连接器跨越[多个连接](./search-concept-custom-types.md)摄取的外部数据。
- 充分利用 Microsoft Graph 连接器的增强内容，了解：
  - [管理连接](connecting-external-content-manage-connections.md)
  - [管理架构](connecting-external-content-manage-schema.md)
  - [管理项目](connecting-external-content-manage-items.md)
- 跟踪 Microsoft Graph [连接](/graph/api/resources/externalconnection?view=graph-rest-beta&preserve-view=true)的状态。
- 定义[外部组](/graph/api/resources/externalgroup?view=graph-rest-beta&preserve-view=true)以设置添加到 Microsoft Graph [连接](/graph/api/resources/externalconnection?view=graph-rest-beta&preserve-view=true)的[外部项目](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) 对象的权限。 外部组可以表示非 Azure Active Directory 组或类似组的构造（例如业务单元），它们确定对外部数据源中的内容的权限。

### <a name="teamwork"></a>团队合作
- 获取 Teams [频道](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true)或[团队](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true)的创建日期/时间。


## <a name="august-2020-new-and-generally-available"></a>2020 年 8 月：新版本和正式版

### <a name="change-notifications"></a>更改通知
在 Microsoft Graph for US Government 国家云中[跟踪受支持资源的更改](delta-query-overview.md)。

### <a name="cloud-communications"></a>云通信
- [取消](/graph/api/call-cancelmediaprocessing)流程或队列中的任何交互式语音响应 (VR) 操作，这些操作可以是[播放音频提示](/graph/api/call-playprompt)或[录制响应](/graph/api/call-record)。
- 通过“**听录**”属性 [调用听录信息](/graph/api/resources/calltranscriptioninfo)。

### <a name="teamwork"></a>团队合作
- 使用另一种方法，无需创建组即可直接[创建团队](/graph/api/team-post)。
- 使用 **members** 导航属性，以更可靠、低延迟的方式在团队中添加成员。
- 通过 [应用程序定义](/graph/api/resources/teamsappdefinition)的 **publishingState** 属性获取 Microsoft Teams [应用](/graph/api/resources/teamsapp)的发布状态。 可能的值为 `submitted`、`published` 和 `rejected`。 请参阅[示例](/graph/api/teamsapp-list?view=graph-rest-beta&preserve-view=true#example-3-list-applications-with-a-given-id-and-return-the-submission-review-state)。
- 使用 `AppCatalog.Submit` 委派的权限，允许用户[提交应用](/graph/api/teamsapp-publish)并请求管理员审查。 对于用户[取消](/graph/api/teamsapp-delete)过去提交的尚未发布的应用使用相同的权限。 


## <a name="august-2020-new-in-preview-only"></a>2020 年 8 月：仅限预览版新增功能

### <a name="applications"></a>应用程序
在 [服务主体](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true)应用程序资源中支持基于密码的单点登录，并在 **passwordSingleSignOnSettings** 属性中指定此类 [设置](/graph/api/resources/passwordsinglesignonsettings?view=graph-rest-beta&preserve-view=true)。 有关 Azure AD 中基于密码的单一登录的信息，请参阅[配置基于密码的单一登录](/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications)。

### <a name="calendar"></a>日历
增强对涉及定期[事件](/graph/api/resources/event?view=graph-rest-beta&preserve-view=true)的方案的编程支持：
- 通过使用 **occurrenceId** 属性，可以可靠地标识定期数据系列中的任何事件，包括已修改或已取消的事件。
- 通过使用 **exceptionOccurrences** 属性获取定期数据系列中的任何例外事件。
- 通过使用 **cancelledOccurrences** 属性获取数据系列中的任何取消事件。

### <a name="change-notifications"></a>更改通知
- 使用 [订阅](/graph/api/resources/subscription?view=graph-rest-beta&preserve-view=true)的 **includeResourceData** 属性，以 [设置包含资源数据的更改通知](webhooks-with-resource-data.md)。请勿使用 **includeProperties** 属性。
- 获取[通过事件中心发送的更改通知](change-notifications-delivery.md)。

### <a name="devices-and-apps--cloud-printing"></a>设备和应用 | 云打印
- 通过使用 **allowAllUser** 属性向所有用户和组授予对 [打印机共享](/graph/api/resources/printershare?view=graph-rest-beta&preserve-view=true)的访问权限。
- 使用新的委派和应用程序权限来访问或管理[打印文档](/graph/api/resources/printDocument?view=graph-rest-beta&preserve-view=true)、[打印作业](/graph/api/resources/printjob?view=graph-rest-beta&preserve-view=true)、[打印机](/graph/api/resources/printer?view=graph-rest-beta&preserve-view=true)、[打印机共享](/graph/api/resources/printershare?view=graph-rest-beta&preserve-view=true)或[打印任务定义](/graph/api/resources/printtaskdefinition?view=graph-rest-beta&preserve-view=true)。有关详细信息，请参阅云打印[八月](changelog.md#august-2020)更新。

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理
beta 版本中的 Intune [8 月](changelog.md#august-2020)更新。

### <a name="identity-and-access--governance"></a>身份和访问 | 治理
- 自定义[使用条款协议](/graph/api/resources/agreement?view=graph-rest-beta&preserve-view=true)，以支持协议的到期日和频率，要求用户按设备接受协议，或者按设定的频率重新接受协议。 
- 使用 **file** 属性导航到某个 [自定义协议](/graph/api/resources/agreementfile?view=graph-rest-beta&preserve-view=true)以了解使用条款。请勿使用 **files** 属性。
- 添加、删除和列出内部或外部发起人，他们可以批准[互联组织](/graph/api/resources/connectedorganization?view=graph-rest-beta&preserve-view=true)关于访问组、应用程序或 SharePoint Online 网站的请求。有关更多信息，请参见[权利管理](/graph/api/resources/entitlementmanagement-root?view=graph-rest-beta&preserve-view=true)。

### <a name="identity-and-access--identity-and-sign-in"></a>身份和访问 | 身份和登录
- 为租户启用进一步自定义[授权策略](/graph/api/resources/authorizationpolicy?view=graph-rest-beta&preserve-view=true)，例如允许[默认的用户角色](/graph/api/resources/defaultuserrolepermissions?view=graph-rest-beta&preserve-view=true)创建应用程序或安全组或读取其他用户，允许用户注册电子邮件订阅或通过电子邮件验证加入租户，或允许用户自行重置密码。
- 在 Azure Active Directory B2C 租户中，以用户流的形式管理[预定义的可配置策略](/graph/api/resources/b2cuserflows?view=graph-rest-beta&preserve-view=true)。 查看更多有关 [B2C 用户流](/azure/active-directory-b2c/user-flow-overview)的详细信息。
- 在 Azure Active Directory 租户中，启用[自助注册体验作为 B2X 用户流](/graph/api/resources/b2xuserflows?view=graph-rest-beta&preserve-view=true)。查看有关[自助注册](/azure/active-directory/external-identities/self-service-sign-up-overview)的更多信息。

### <a name="people-and-workplace-intelligence--profile"></a>人员和工作场所智能 | 配置文件
在用户的[个人资料](/graph/api/resources/profile?view=graph-rest-beta&preserve-view=true)中添加和管理以下额外属性，这些属性可以在 Microsoft 365 和第三方应用程序的共享人员体验中体现：
- [地址](/graph/api/resources/itemAddress?view=graph-rest-beta&preserve-view=true)
- [纪念日](/graph/api/resources/personAnniversary?view=graph-rest-beta&preserve-view=true)
- [奖项](/graph/api/resources/personAward?view=graph-rest-beta&preserve-view=true)
- [证书](/graph/api/resources/personCertification?view=graph-rest-beta&preserve-view=true)
- [笔记](/graph/api/resources/personAnnotation?view=graph-rest-beta&preserve-view=true)：
- [专利](/graph/api/resources/itemPatent?view=graph-rest-beta&preserve-view=true)
- [出版物](/graph/api/resources/itemPublication?view=graph-rest-beta&preserve-view=true)


### <a name="reports--microsoft-365-usage-reports"></a>报告 | Microsoft 365 使用情况报告
获取[有关 Microsoft 365 应用使用情况的报告](/graph/api/resources/microsoft-365-apps-usage-report?view=graph-rest-beta&preserve-view=true)，特别是有关用户详细信息、用户数量和平台用户数量的报告。

### <a name="teamwork"></a>团队合作
获取[在聊天消息中托管的内容](/graph/api/resources/chatMessageHostedContent?view=graph-rest-beta&preserve-view=true)（如图像或代码段）。 请参阅[示例](/graph/api/chatmessagehostedcontent-get?view=graph-rest-beta&preserve-view=true&branch=master#example-2-get-hosted-content-bytes-for-an-image)，获取图像的内容字节。

### <a name="to-do-tasks"></a>待办任务
- 针对[微软待办](todo-concept-overview.md)推出了一组新 API，允许应用用户跨 Microsoft 365 客户端应用组织和跟踪个人任务。查看[使用微软待办 API](/graph/api/resources/todo-overview?view=graph-rest-beta&preserve-view=true) 了解详细信息。
- 弃用 [Outlook 任务 API](/graph/api/resources/outlooktask?view=graph-rest-beta&preserve-view=true)。


## <a name="july-2020-new-and-generally-available"></a>2020 年 7 月：新版本和正式版

### <a name="calendar"></a>日历
正式发布一项功能，它允许组织者接受备选会议时间提案，并允许受邀者在[暂时接受](/graph/api/event-tentativelyaccept?view=graph-rest-1.0&preserve-view=true&preserve-view=true)或[拒绝](/graph/api/event-decline?view=graph-rest-1.0&preserve-view=true&preserve-view=true)事件时[为会议建议新时间](outlook-calendar-meeting-proposals.md)。

### <a name="change-notifications"></a>更改通知
已删除从 [changeNotification](/graph/api/resources/changenotification) 类型中错误引入的 **sequenceNumber** 资源。

### <a name="groups"></a>组
[group](/graph/api/resources/group) 实体下列属性的通用版本：**assignedLabels**、**expirationDateTime**、**membershipRule**、**membershipRuleProcessingState**、**preferredLanguage** 和 **theme**。

### <a name="identity-and-access"></a>身份和访问
- 删除作为[设备](/graph/api/resources/device)的注册所有者或用户的用户。
- 跟踪对新创建、更新或删除的应用程序本地表示形式（由 [servicePrincipals](/graph/api/resources/serviceprincipal) 资源表示）和委派权限授予（由 [oAuth2PermissionGrant](/graph/api/resources/oauth2permissiongrant) 资源表示）的更改，而无需对整个资源集合执行完全读取操作。
- 正式发布[用于强制安全性默认设置的策略](/graph/api/resources/identitysecuritydefaultsenforcementpolicy)，可以保护组织免受常见攻击。

### <a name="identity-and-access--identity-and-sign-in"></a>身份和访问 | 身份和登录
- 正式发布[条件访问策略](/graph/api/resources/conditionalAccessPolicy)，它们是用于定义访问方案的自定义规则。
- 正式发布表示自定义规则的[命名位置](/graph/api/resources/namedLocation)，用于定义在条件访问策略中使用的网络位置。

### <a name="schema-extensions"></a>架构扩展
[架构扩展](/graph/api/resources/schemaextension)功能现在可在[Microsoft Cloud for US Government](./deployments.md)使用。

### <a name="teamwork"></a>团队合作
使用 `TeamsAppInstallation.ReadForTeam` 或 `TeamsAppInstallation.ReadWriteForTeam` 的委派权限，或者使用 `TeamsAppInstallation.ReadForTeam.All` 或 `TeamsAppInstallation.ReadWriteForTeam.All` 的应用程序权限来[列出已在团队中安装的应用](/graph/api/teamsappinstallation-list)。

## <a name="july-2020-new-in-preview-only"></a>2020 年 7 月：预览版新增功能

### <a name="cloud-communications"></a>云通信
- 使用 [更新](/graph/api/onlinemeeting-update?view=graph-rest-beta&preserve-view=true&preserve-view=true)操作来更新 [联机会议](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true&preserve-view=true)的 **startDateTime**、**endDateTime**、**participants** 或 **subject** 属性。
- 订阅有关 Microsoft Teams 上用户可用性更改的通知，如[状态](/graph/api/resources/presence?view=graph-rest-beta&preserve-view=true)资源所示。

### <a name="cloud-communications--call-records"></a>云通信 | 通话记录
- [获取](/graph/api/callrecords-callrecord-getpstncalls?view=graph-rest-beta&preserve-view=true)公用电话交换网 (PSTN) 通话的记录。
- [获取](/graph/api/callrecords-callrecord-getdirectroutingcalls?view=graph-rest-beta&preserve-view=true)直接路由通话的记录。

### <a name="compliance--ediscovery"></a>合规性 | 电子数据展示
首次推出的[电子数据展示事例](/graph/api/resources/ediscoverycase?view=graph-rest-beta&preserve-view=true)包含可在法律案件中作为证据的保管人、保留、集合、管理审阅集和导出。
应用现在可以对收集用于诉讼、调查或法规请求的[审阅集数据](/graph/api/resources/reviewset?view=graph-rest-beta&preserve-view=true)进行[查询](/graph/api/resources/reviewsetquery?view=graph-rest-beta&preserve-view=true)和挑选。 这一首次推出的内容是 Microsoft 365 [高级电子数据展示](/microsoft-365/compliance/overview-ediscovery-20?view=o365-worldwide&preserve-view=true)的一部分。

### <a name="devices-and-apps--cloud-printing"></a>设备和应用 | 云打印
- 使用应用程序权限 `Printer.ReadWrite.All` 和 [Internet 打印协议（IPP）编码](https://tools.ietf.org/html/rfc8010)至[更新打印机](/graph/api/printer-update?view=graph-rest-beta&preserve-view=true)。
- 使用以下应用权限之一、`PrintJob.ReadBasic.All`、`PrintJob.Read.All`、`PrintJob.ReadWriteBasic.All` 或 `PrintJob.ReadWrite.All`，来[获取打印作业](/graph/api/printjob-get?view=graph-rest-beta&preserve-view=true)或[列出打印机打印作业](/graph/api/printer-list-jobs?view=graph-rest-beta&preserve-view=true)。
- [获取打印作业](/graph/api/printjob-get?view=graph-rest-beta&preserve-view=true)时，请使用 `$expand` 获取对作业正在执行或已执行的[打印作业](/graph/api/resources/printtask?view=graph-rest-beta&preserve-view=true)。 [截取打印](universal-print-concept-overview.md#extending-universal-print-to-support-pull-printing)中使用打印任务、[任务定义](/graph/api/resources/printtaskdefinition?view=graph-rest-beta&preserve-view=true)、和[任务触发器](/graph/api/resources/printtasktrigger?view=graph-rest-beta&preserve-view=true)。
- [重定向打印作业](/graph/api/printjob-redirect?view=graph-rest-beta&preserve-view=true)至其他打印机，作为截取打印的组成部分。

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理
Intune [7 月](changelog.md#july-2020)试用版更新。

### <a name="groups"></a>组
使用 Microsoft 365 [组](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true)的 **isAssignableToRole** 属性，并在创建组的过程中对其进行设置，以指示该组是否可以分配给 Azure AD 角色。 这 [有助于在 Azure AD 中管理角色分配](/azure/active-directory/users-groups-roles/roles-groups-concept)，例如特权角色管理员或全局管理员可以创建 Microsoft 365 组并向该组分配 Azure AD 角色，而不是向单个用户分配这一角色，这样一来，用户加入该 _组_ 后，他们会被间接分配既定角色。

### <a name="identity-and-access"></a>身份和访问
- [获取访问令牌](/graph/api/synchronization-synchronization-acquireAccessToken?view=graph-rest-beta&preserve-view=true)，以授权 Azure AD 预配服务将用户预配到应用程序。
- [获取](/graph/api/entitlementmanagementsettings-get?view=graph-rest-beta&preserve-view=true)或[更新](/graph/api/entitlementmanagementsettings-update?view=graph-rest-beta&preserve-view=true)权限管理设置，这些设置控制对组织内部和外部用户的组、应用程序和 SharePoint Online 网站的访问权限。 

### <a name="identity-and-access--identity-and-sign-in"></a>身份和访问 | 身份和登录
- 将用户风险级别（`low`、`medium`、`high`、`none`）包含为应用 [条件访问策略](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta&preserve-view=true)的注意事项。
- [使用密码更改作为授予控制](/graph/api/resources/conditionalaccessgrantcontrols?view=graph-rest-beta&preserve-view=true#special-considerations-when-using-passwordchange-as-a-control)，以便传递条件访问策略。
- 在 Azure AD 租户和 Azure AD B2C 租户中，将 [OpenID Connect 提供程序](/graph/api/resources/openidconnectprovider?view=graph-rest-beta&preserve-view=true) (OIDC) 用作标识提供程序。 其 **claimsMapping** 属性允许 Azure AD 将 OIDC 提供程序的 [声明映射](/graph/api/resources/claimsmapping?view=graph-rest-beta&preserve-view=true)到 Azure AD 可识别和使用的声明。

### <a name="people-and-workplace-intelligence--insights"></a>人脉和工作场所智能|见解
在 Microsoft 365 中，对[项见解](/graph/api/resources/iteminsights?view=graph-rest-beta&preserve-view=true)的可用性和显示进行更[精细的隐私控制](insights-customize-item-insights-privacy.md)。 这些见解表示 OneDrive for Business 中的用户和文档之间的关系，并使用高级分析和机器学习技术进行计算。 

### <a name="people-and-workplace-intelligence--profile-card-customization"></a>人脉和工作区智能 | 个人资料卡片自定义
管理员可以使用[个人资料卡属性](/graph/api/resources/profilecardproperty?view=graph-rest-beta&preserve-view=true) API，[自定义显示在组织个人资料卡上的属性](add-properties-profilecard.md)。

### <a name="sites-and-lists"></a>网站和列表
访问 SharePoint [术语库](/graph/api/resources/termstore-store?view=graph-rest-beta&preserve-view=true)分类系统，该系统的层次结构包括 [group](/graph/api/resources/termstore-group?view=graph-rest-beta&preserve-view=true)、[set](/graph/api/resources/termstore-set?view=graph-rest-beta&preserve-view=true) 和 [term](/graph/api/resources/termstore-term?view=graph-rest-beta&preserve-view=true) 资源，以及术语之间的 [relation](/graph/api/resources/termstore-relation?view=graph-rest-beta&preserve-view=true) 资源。

### <a name="workbooks-and-charts"></a>工作簿和图表
[获取[工作簿](/graph/api/resources/workbook?view=graph-rest-beta&preserve-view=true)中长时间运行[操作](/graph/api/resources/workbookoperation?view=graph-rest-beta&preserve-view=true)的状态和任何结果](/graph/api/workbookoperation-get?view=graph-rest-beta&preserve-view=true)。



## <a name="june-2020-new-and-generally-available"></a>2020 年 6 月：新版本和正式版

### <a name="cloud-communications--online-meeting"></a>云通信 | 联机会议
- [创建联机会议](/graph/api/application-post-onlinemeetings?view=graph-rest-1.0&preserve-view=true&preserve-view=true) 以提供基于区域的加入信息时，请使用 `Accept-Language` HTTP 标头。
- 使用 [createOrGet](/graph/api/onlinemeeting-createorget?view=graph-rest-1.0&preserve-view=true&preserve-view=true) 返回具有指定 **externalId** 值的在线会议，或者创建一个外部值（如果不存在），以简化将结果会议嵌入到第三方日历中。

### <a name="files"></a>文件
- 增强的同步支持：
  - 使用 **pendingOperations** 属性标识可能会更新挂起的 [driveItem](/graph/api/resources/driveitem) 文件的二进制内容的任何 [操作](/graph/api/resources/pendingoperations)。
  - [还原](/graph/api/driveitem-restore) 已删除且位于 OneDrive 个人版回收站中的 **driveItem**。
- 获取或设置[照片](/graph/api/resources/photo)的方向。 OneDrive 个人版上支持设置。
- 使用安全哈希算法 (SHA-256) 增强[文件](/graph/api/resources/file)数据安全性和完整性。
- 在向 OneDrive for Business [上传一个大文件](/graph/api/driveitem-createuploadsession)时，使用 `deferCommit`这个参数来延迟最终的创建，直到应用程序请求完成上传。
- 使用 **fileSize** 属性作为 **项目** 参数的一部分提供估算，以便在在将文件 [上载](/graph/api/driveitem-createuploadsession)到 OneDrive 个人版中之前执行配额检查。
- 通过 [驱动器的 **quota** 属性找到 [storagePlanInformation](/graph/api/resources/storageplaninformation)](/graph/api/resources/drive) 资源，查看是否有更高的存储配额计划可用。

### <a name="groups"></a>组
使用应用程序权限`Group.Read.All`和`Group.ReadWrite.All`，以便获得[组对话](/graph/api/resources/conversation)和[对话线程](/graph/api/resources/conversationthread)的资源。

### <a name="identity-and-access"></a>身份和访问 
- GA 两组 API，用于 [标识保护](/graph/api/resources/identityprotectionroot)： [的风险检测](/graph/api/resources/riskdetection) 和 [有风险的用户](/graph/api/resources/riskyuser) API。

### <a name="security"></a>安全性
- 在 [警报](/graph/api/resources/alert?view=graph-rest-1.0&preserve-view=true&preserve-view=true)的属性中跟踪以下内容：
  - 与警报相关的事件的ID。
  - 将 [资源标识](/graph/api/resources/securityResource?view=graph-rest-1.0&preserve-view=true#securityresourcetype-values) 为受攻击或警报中的相关资源。
  - 指定与警报相关的 [网络连接](/graph/api/resources/networkconnection?view=graph-rest-1.0&preserve-view=true) 的源和目标位置。

### <a name="sites-and-lists"></a>网站和列表
指定 SharePoint [列表](/graph/api/resources/list) 资源的 [列定义](/graph/api/resources/columndefinition) 中的地理位置数据。

### <a name="teamwork"></a>团队合作
- 使用委派的权限[AppCatalog.Read.All](./permissions-reference.md#appcatalog-resource-permissions)列出来自 Microsoft Teams 应用程序目录的[应用](/graph/api/resources/teamsapp?view=graph-rest-1.0&preserve-view=true)。
- [获取有关映射到 Teams [频道](/graph/api/resources/channel)中的 **文件** 选项卡的文件夹](/graph/api/channel-get-filesfolder) 的信息。
- [获取 [团队](/graph/api/resources/team)的默认频道](/graph/api/team-get-primarychannel)，标记为 **常规**"。


## <a name="june-2020-new-in-preview-only"></a>2020 年 6 月：预览版新增功能

### <a name="calendar"></a>日历
除了跟踪 **calendarView** 中事件的增量更改（集合或由 start _和_ 结束日期分隔的事件），请对用户邮箱中的事件或特定用户日历中的事件使用 [delta](/graph/api/event-delta?view=graph-rest-beta&preserve-view=true)功能。

### <a name="cloud-communications--presence"></a>云通信 | 预览版
[获取组织中所有用户的状态](/graph/api/presence-get?view=graph-rest-beta&preserve-view=true) 或组织中特定用户的状态。

### <a name="devices-and-apps--cloud-printing"></a>设备和应用 | 云打印
- 在配置 [文档进行打印](/graph/api/resources/printdocument?view=graph-rest-beta&preserve-view=true)时指定[打印页边距](/graph/api/resources/printmargin?view=graph-rest-beta&preserve-view=true)。
- 支持以下 [打印机功能](/graph/api/resources/printercapabilities?view=graph-rest-beta&preserve-view=true)：
  - 源方向
  - 打印页面范围
  - 在DPI上的打印分辨率
  - 最大打印作业队列大小（以字节为单位）
  - 输入纸盒
  - 边距
  - collation
  - 文档缩放
- 支持打印分辨率（DPI）和文档缩放作为 [默认打印机设置](/graph/api/resources/printerdefaults?view=graph-rest-beta&preserve-view=true)中的一部分。
- 支持以下 [文档配置](/graph/api/resources/printerdocumentconfiguration?view=graph-rest-beta&preserve-view=true) 设置：
  - 输入纸盒
  - 输出纸盒
  - 媒体大小
  - 边距
  - 媒体类型
  - finishings （例如装订）
  - 每版打印页数
  - 多页版式指定每版打印页面的布局方向
  - collation
  - scaling
- 在[列出pring作业](/graph/api/printer-list-jobs?view=graph-rest-beta&preserve-view=true)时展开文档。
- [注册打印机]()并使用[printerCreateOperation](/graph/api/resources/printercreateoperation?view=graph-rest-beta&preserve-view=true)资源跟踪和验证打印机的注册。
- 在当前用户或应用程序的租户内[获取长期运行的打印机注册操作](/graph/api/printoperation-get?view=graph-rest-beta&preserve-view=true)。
- 一些属性和枚举类型的重命名 - 详见[六月](changelog.md#june-2020)更新的云打印更新。

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理
Intune[6月](changelog.md#june-2020)试用版中更新

### <a name="education"></a>教育
- 可以使用委托权限`EduRoster.ReadBasic`来 [获取](/graph/api/educationuser-get?view=graph-rest-beta&preserve-view=true)外部源程序中的 [教师](/graph/api/resources/educationteacher?view=graph-rest-beta&preserve-view=true)或 [学生](/graph/api/resources/educationstudent?view=graph-rest-beta&preserve-view=true)的ID，作为 **externalId** 属性。
- 如果从学习管理系统(LMS)创建了教育 [组织](/graph/api/resources/educationorganization?view=graph-rest-beta&preserve-view=true)或 [班别](/graph/api/resources/educationclass?view=graph-rest-beta&preserve-view=true)，那么使用 **externalSource** 属性来跟踪值`lms`。

### <a name="identity-and-access"></a>身份和访问
- IT专业人员可以使用作为轻量级代理的[连接器](/graph/api/resources/connector?view=graph-rest-beta&preserve-view=true)资源连接到[Azure AD 应用程序代理](/azure/active-directory/manage-apps/what-is-application-proxy)，并[在外部发布本地web应用程序应用程序](/graph/api/resources/onpremisespublishing?view=graph-rest-beta&preserve-view=true)，以便其组织的远程用户可以以安全的方式访问这些应用程序。
- 在租户级别[管理身份验证策略](/graph/api/resources/authenticationflowspolicy?view=graph-rest-beta&preserve-view=true)，以启用或禁用外部用户的[自服务注册](/graph/api/resources/selfservicesignupauthenticationflowconfiguration?view=graph-rest-beta&preserve-view=true)。
- [按需提供用户帐户](/graph/api/synchronization-synchronizationjob-provision-on-demand?view=graph-rest-beta&preserve-view=true)，并能够指定要提供的对象和要执行的同步规则。

### <a name="search"></a>搜索
- 利用 [模式](/graph/api/resources/schema?view=graph-rest-beta&preserve-view=true)中 [属性](/graph/api/resources/property?view=graph-rest-beta&preserve-view=true)上的增强功能：**isRefinable** 支持搜索结果的过滤和更精细的搜索体验控制，**别名** 和 **标签** 支持更好的相关性。
- 在 **架构** 中，最多可以指定 128 **属性** 资源。
- 使用 [get externalItem](/graph/api/externalitem-get?view=graph-rest-beta&preserve-view=true) 用于诊断目的。

### <a name="users"></a>用户
- 使用 [mailboxSettings](/graph/api/resources/mailboxsettings?view=graph-rest-beta&preserve-view=true) 的 **userPurpose** 属性，可在 Exchange Online 中识别共享邮箱和设备邮箱中的单个用户的邮箱并从中区分。 
- 使用 [用户设置](/graph/api/resources/usersettings?view=graph-rest-beta&preserve-view=true)去 [获取](/graph/api/regionalandlanguagesettings-get?view=graph-rest-beta&preserve-view=true)或[更新](/graph/api/regionalandlanguagesettings-update?view=graph-rest-beta&preserve-view=true)[首选语言和区域设置](/graph/api/resources/regionalandlanguagesettings?view=graph-rest-beta&preserve-view=true)。
- 用户设置是通过点击 Azure AD 用户配置文件以反映相同的用户首选项，可通过 [用户](/graph/api/resources/user?view=graph-rest-beta&preserve-view=true) 实现跨应用的一致用户体验的关系。请参阅[用户设置与邮箱设置的区别](/graph/api/resources/user?view=graph-rest-beta&preserve-view=true#user-preferences-for-languages-and-regional-formats)。


## <a name="may-2020-new-and-generally-available"></a>2020 年 5 月：新版本和正式版

### <a name="calendar--place"></a>日历 | 位置
v1.0 中的[位置 API](/graph/api/resources/place) 的正式版 - 在生产应用中使用此 API 可以获取、更新或删除租户中的[房间](/graph/api/resources/room)或[房间列表](/graph/api/resources/roomlist)。[进一步了解](outlook-calendar-concept-overview.md#build-apps-with-location-awareness-and-provide-intelligent-context)关于位置 API 的信息。

### <a name="change-notifications"></a>更改通知
- 订阅 Microsoft Cloud for US Government 中的更改通知。

### <a name="cloud-communications--call-records"></a>云通信 | 通话记录
- [通话记录 API](/graph/api/resources/callrecords-api-overview?view=graph-rest-1.0&preserve-view=true) 的正式版 - 使用 [callRecord ](/graph/api/resources/callrecord?view=graph-rest-1.0&preserve-view=true) 资源获取 Microsoft Teams 和 Skype 上的通话和在线会议的元数据。
- 订阅 [更改通知](./webhooks.md)，了解组织中所有 **callRecord** 资源的更改。
- 在 **callRecord** 中 [列出会话](/graph/api/callrecords-session-list?view=graph-rest-1.0&preserve-view=true)，并根据需要 [扩展每个会话以列出呼叫记录中的段](/graph/api/callrecords-session-list?view=graph-rest-1.0&preserve-view=true#example-2-get-session-list-with-segments)。
- 支持段中媒体端点的 60 GHz (`frequency60GHz`) 和 `unknownFutureValue`WiFi 波段值。
- 支持将语音邮件作为通信[段](/graph/api/resources/callrecords-segment)中服务端端点的一种可能类型。

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理
v1.0 中的 Intune [5 月](changelog.md#may-2020)更新。

### <a name="graph-explorer"></a>Graph 浏览器
[Graph 浏览器](https://developer.microsoft.com/en-us/graph/graph-explorer)中的许多新功能可用于增强沙箱中的学习和原型制作。例如：
- 在 C#、Java、JavaScript 和 Objective C 中查看与你输入的 REST API 查询相对应的代码段。
- 登录租户、查看访问令牌并将其复制到你喜欢的 REST 客户端应用程序。

有关详细信息，请参阅[新 Graph 浏览器现已上市](https://developer.microsoft.com/graph/blogs/new-graph-explorer-is-now-ga/)。

### <a name="groups"></a>组
- 通过 Azure AD Connect 将本地目录同步到 Azure Active Directory 时现在会返回 **onPremisesDomainName**、**onPremisesNetBiosName** 和 **onPremisesSamAccountName** 属性，作为 [组](/graph/api/resources/group?view=graph-rest-1.0&preserve-view=true)资源的一部分。
- 订阅由 21Vianet 运营的 Microsoft Cloud 中国的 [group](/graph/api/resources/group) 资源的更改通知。

### <a name="identity-and-access"></a>身份和访问
- v1.0 中的服务主体 API 的正式版 - 使用生产应用程序中的 [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-1.0&preserve-view=true) 资源，以编程方式管理应用程序实例并控制应用程序可以在租户中执行的操作。 你可以控制谁可以使用应用程序、应用程序可以访问哪些资源，例如添加密码凭据、滚动过期证书以及管理委派的权限授予和应用程序角色分配。
- [appRoleAssignment](/graph/api/resources/appRoleAssignment?view=graph-rest-1.0&preserve-view=true) API 的正式版，该 API 记录了 向[用户](/graph/api/resources/user?view=graph-rest-1.0&preserve-view=true)、[组](/graph/api/resources/group?view=graph-rest-1.0&preserve-view=true)或 [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-1.0&preserve-view=true)的 [appRole](/graph/api/resources/approle?view=graph-rest-1.0&preserve-view=true) 分配情况（代表 ID 令牌和访问令牌中的 `roles` 声明）。
- 在 Azure Active Directory 上使用 Facebook 作为标识提供程序。
- 使用 `AppRoleAssignment.ReadWrite.All` 的委派权限或应用程序权限以允许应用管理任何 API（包括 Microsoft Graph）的应用程序权限授予和任何应用（已登录或未登录用户）的应用程序分配。


### <a name="microsoft-graph-sdks"></a>Microsoft Graph SDK
有关如下内容，请参阅新的 SDK 指南：
- [分页](./sdks/paging.md)
- [批处理](./sdks/batch-requests.md)
- [将大文件上传到 OneDrive](./sdks/large-file-upload.md)
- [通过 HTTP 中间件组件自定义 SDK 服务客户端](./sdks/customize-client.md)。

### <a name="teamwork"></a>团队合作
- 如果你的方案涉及 Teams 在线会议，请参阅有关[如何在[日历 API ](outlook-calendar-online-meetings.md)和[云通信 API](cloud-communications-online-meetings.md)之间进行选择](choose-online-meeting-api.md)的新指南，以创建和加入在线会议。
- [在[频道](/graph/api/resources/channel?view=graph-rest-1.0&preserve-view=true)中发送](/graph/api/channel-post-messages?view=graph-rest-1.0&preserve-view=true)和[回复](/graph/api/channel-post-messagereply?view=graph-rest-1.0&preserve-view=true)邮件。
- 通过使用 **fileFolder** 导航属性，获取 [频道](/graph/api/resources/channel?view=graph-rest-1.0&preserve-view=true)文件的 OneDrive for Business 位置。

### <a name="teamwork--shifts"></a>团队合作 | Shifts
v1.0 中 [ shifts API](/graph/api/resources/shift?view=graph-rest-1.0&preserve-view=true) 的正式版 - 在生产应用程序中使用此 API 创建、更新和管理一线员工的日程安排，以使他们保持联系并有效进行协作。

### <a name="users"></a>用户
- 订阅由 21Vianet 运营的 Microsoft Cloud 中国的 [user](/graph/api/resources/user) 资源的更改通知。
- 通过使用 **user** 资源的 **externalUserState** 和 **externalUserStateChangeDateTime** 跟踪 [已受邀](/graph/api/invitation-post?view=graph-rest-1.0&preserve-view=true)加入组织的外部用户的最新状态更改的状态和日期/时间。

## <a name="may-2020-new-in-preview-only"></a>2020 年 5 月：仅限预览版新增功能

### <a name="change-notifications"></a>更改通知
- 使用正式架构化的类型 [changeNotification](/graph/api/resources/changenotification?view=graph-rest-beta&preserve-view=true) 和 [changeNotificationCollection](/graph/api/resources/changenotificationcollection?view=graph-rest-beta&preserve-view=true) 处理资源更改通知。 
- 通过使用 **changeNotification** 资源上的 **sequenceNumber** 属性跟踪通知是否按顺序或是否缺少通知。

### <a name="devices-and-apps--cloud-printing"></a>设备和应用 | 云打印
- [printer](/graph/api/resources/printer?view=graph-rest-beta&preserve-view=true) 和 [printerShare](/graph/api/resources/printershare?view=graph-rest-beta&preserve-view=true) 资源现在是奇偶校验的，并且彼此具有相同的属性。
- 围绕打印机共享的一些属性和类型名称清理：
  - 使用 [print](/graph/api/resources/print?view=graph-rest-beta&preserve-view=true) 的 **shared** 导航属性来获取在租户中注册的打印机共享列表。 
  - 有关详细信息，请参阅 [5 月](changelog.md#may-2020)更改日志。

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理
测试版中的 Intune [5 月](changelog.md#may-2020)更新。

### <a name="groups"></a>组
- 使用[组](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true)的现有规则或指定规则[评估](/graph/api/group-evaluatedynamicmembership?view=graph-rest-beta&preserve-view=true)用户或设备是否是动态组的成员。[基于规则的动态成员资格](/azure/active-directory/users-groups-roles/groups-dynamic-membership)减少了添加和删除成员的管理开销。
- 创建 Microsoft 365 [组](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true)时，通过在 **resourceBehaviorOptions** 属性中指定组的行为来仅限配置。 例如，允许成员发布、为新成员订阅对话、禁用欢迎电子邮件以及在 Outlook 体验中隐藏组。
- 在 **resourceProvisioningOptions** 属性中指定要提供的资源，这些资源通常不属于默认 [组](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true)创建的一部分。 当前支持使用 Microsoft Teams 功能将组作为[团队](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true)进行配置。

### <a name="identity-and-access"></a>身份和访问
- 获取从 [directoryObject](/graph/api/resources/directoryObject) 派生的实体集合时，请应用 OData 系统查询选项（`$count`、`$filter`、`$search`）。 你可以 [在这些实体的 **displayName** 和 **description** 属性中搜索特定标记](/graph/search-query-parameter#using-search-on-directory-object-collections)，并使用 OData 强制转换将 **directoryObject** 的结果修剪为特定的派生类型。 有关详细信息，请参阅[使用 $count、$filter、$search 和 $orderby 在 Microsoft Graph 中生成高级查询](https://developer.microsoft.com/en-us/graph/blogs/build-advanced-queries-with-count-filter-search-and-orderby/)。
- 作为 [身份保护 API](/graph/api/resources/identityprotection-root?view=graph-rest-beta&preserve-view=true) 的一部分，请使用 **riskEventType** 属性来 [获取检测到的风险类型](/graph/api/riskdetection-get?view=graph-rest-beta&preserve-view=true)或 [获取用户历史记录中的风险类型](/graph/api/riskyuser-list-history?view=graph-rest-beta&preserve-view=true)。不要使用 **riskType** 属性，因为它已被弃用。
- 在 [条件集](/graph/api/resources/conditionalaccessconditionset?view=graph-rest-beta&preserve-view=true)的 **clientAppTypes** 属性中为 [条件访问策略](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta&preserve-view=true)指定客户端应用程序类型。
- 使用 `EntitlementManagement.Read.All` 的委派权限允许应用代表已登录的用户请求读取访问包及相关权利管理资源。
- 使用 `Application.Read.All` 和 `Application.ReadWrite.All` 的委派或应用程序权限来[列出组织中的应用程序](/graph/api/application-list?view=graph-rest-beta&preserve-view=true)。
- 使用 [authorizationPolicy](/graph/api/resources/authorizationpolicy?view=graph-rest-beta&preserve-view=true) 资源类型控制 Azure AD 中的授权设置。

### <a name="teamwork"></a>团队合作
- [支持单点登录 (SSO)](/microsoftteams/platform/tabs/how-to/authentication/auth-aad-sso) 的 Teams 应用可以在 [teamsAppDefinition](/graph/api/resources/teamsappdefinition?view=graph-rest-beta&preserve-view=true) 的 **azureADAppId** 属性中从 Teams 应用清单中指定 `WebApplicationInfo.id`。
- 使用[细粒度权限](./permissions-reference.md#team-resource-specific-consent-permissions)访问[团队](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true)和[频道](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true)资源。


## <a name="april-2020-new-and-generally-available"></a>2020 年 4 月：新版本和正式版

### <a name="calendar"></a>日历
- 采用编程方式[共享或委派日历](outlook-share-or-delegate-calendar.md)，与 Outlook 用户体验的奇偶校验更加接近。 除了跟踪日历的当前用户权限和共享状态之外：
  - 对于每个[日历](/graph/api/resources/calendar?view=graph-rest-1.0&preserve-view=true)，你现在可以管理与之共享日历的每个用户的[权限](/graph/api/resources/calendarpermission?view=graph-rest-1.0&preserve-view=true)。 
  - 对于每个[邮箱](/graph/api/resources/mailboxsettings?view=graph-rest-1.0&preserve-view=true)，你现在可以指定代理人、邮箱所有者，还是两者同时接收会议邮件和会议响应。 
- [创建事件并作为联机会议更新](outlook-calendar-online-meetings.md)：
  - 对于每个 **日历**，指定允许的和默认的在线会议提供程序。
  - 创建或更新[事件](/graph/api/resources/event?view=graph-rest-1.0&preserve-view=true)以使其在线可用，并提供详细信息供与会者加入在线会议。 
  - 具体来说，使用 **事件** 的新 **onlineMeetingProvider** 和 **onlineMeeting** 属性来将 Microsoft Teams 设置或标识为在线会议提供程序，这是 **onlineMeetingUrl** 属性的 [已知问题](known-issues.md#onlinemeetingurl-property-support-for-microsoft-teams)的解决方法。
- 将[高达 150MB 的文件附件](outlook-large-attachments.md)添加到[event](/graph/api/resources/event?view=graph-rest-1.0&preserve-view=true)。

### <a name="files"></a>文件
- [签出](/graph/api/driveitem-checkout?view=graph-rest-1.0&preserve-view=true)或[签入](/graph/api/driveitem-checkin?view=graph-rest-1.0&preserve-view=true)文件到 OneDrive，以管理更新文件并在更新就绪后向其他人提供更新。
- 应用可选的密码和到期日/时间作为[邀请](/graph/api/driveitem-invite?view=graph-rest-1.0&preserve-view=true)和[创建共享链接](/graph/api/driveitem-createlink?view=graph-rest-1.0&preserve-view=true)操作的参数，以共享 [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0&preserve-view=true)。
- 获取或设置 [权限](/graph/api/resources/permission?view=graph-rest-1.0&preserve-view=true)的密码和到期日/时间，并跟踪被授予共享 **driveItem** 权限的用户的 [identitySet](/graph/api/resources/identityset?view=graph-rest-1.0&preserve-view=true)。
- 使用 **permission** 导航属性，获取 [共享驱动器项](/graph/api/resources/shareddriveitem?view=graph-rest-1.0&preserve-view=true)的 [权限](/graph/api/resources/permission?view=graph-rest-1.0&preserve-view=true)。
- 使用 [共享链接](/graph/api/resources/sharinglink?view=graph-rest-1.0&preserve-view=true)将用户限制为只能在 OneDrive for Business 或 SharePoint 上查看共享 **driveItem** 的内容并且不能下载。

### <a name="identity-and-access"></a>身份和访问
- 若要在基于角色的访问控制（RBAC）提供程序中管理角色并分配资源访问权限，请使用 [unifiedRoleAssignmentMultiple](/graph/api/resources/unifiedroleassignmentmultiple?view=graph-rest-1.0&preserve-view=true)。 **unifiedRoleAssignmentMultiple** 资源支持在一系列作用域中定义单个角色，并将该角色分配给多个主体（例如用户）。
- 使用 `/policies` URL 段并指定策略类型，访问[组织的特定类型的策略](/graph/api/resources/policy-overview?view=graph-rest-1.0&preserve-view=true)。 例如，组织可以强制实施 Web 会话在一段时间不活动后自动从该会话注销用户的策略；请参阅 [activityBasedTimeoutPolicy](/graph/api/resources/activitybasedtimeoutpolicy?view=graph-rest-1.0&preserve-view=true) 的实例的 CRUD 操作。 这是一项[重大更改](https://developer.microsoft.com/identity/blogs/breaking-changes-policy-api-microsoft-graph-1.0/)，可以通过对 `/policies` 段下所有类型的策略进行分组，以便更易于发现所有策略。 采用类似的方法访问其他类型的策略：[claimsMappingPolicy](/graph/api/resources/claimsmappingpolicy?view=graph-rest-1.0&preserve-view=true)、[homeRealmDiscoveryPolicy](/graph/api/resources/homerealmdiscoverypolicy?view=graph-rest-1.0&preserve-view=true)、[tokenLifetimePolicy](/graph/api/resources/tokenlifetimepolicy?view=graph-rest-1.0&preserve-view=true) 和 [tokenIssuancePolicy](/graph/api/resources/tokenissuancetimepolicy?view=graph-rest-1.0&preserve-view=true)。 

### <a name="mail"></a>邮件
向 [message](/graph/api/resources/message?view=graph-rest-1.0&preserve-view=true) 添加了[高达 150MB 的文件附件](outlook-large-attachments.md)。

### <a name="sites-and-lists"></a>站点和列表
- [列出站点](/graph/api/sites-list-followed?view=graph-rest-1.0&preserve-view=true)，这些站点时已登录用户关注的。
- 通过使用 **dataLocationCode** 属性来确定 [网站集](/graph/api/resources/sitecollection?view=graph-rest-1.0&preserve-view=true)的地理区域。
- 通过访问属于 [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0&preserve-view=true) 的 **sharepointIds** 的 **tenantId** 属性，在 SharePoint 上标识文件、文件夹或其他项目的租户。

## <a name="april-2020-new-in-preview-only"></a>2020 年 4 月：仅限预览版中的新增功能

### <a name="devices-and-apps--cloud-printing"></a>设备和应用 | 云打印

将允许的用户和组指定为在通用打印（Microsoft 365 基于云的打印基础结构）上使用特定的[打印机共享](/graph/api/resources/printershare?view=graph-rest-beta&preserve-view=true)。 若要体验可靠且集中的打印管理功能，并为打印用户提供简单而丰富安全的打印体验，请参阅[通用打印公告](https://techcommunity.microsoft.com/t5/windows-it-pro-blog/announcing-universal-print-a-cloud-based-print-solution/ba-p/1204775)并加入其预览计划。

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理
Intune [4 月](changelog.md#april-2020)更新。

### <a name="groups"></a>组
通过组的应用 ID 识别创建[组](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true)的应用。

### <a name="identity-and-access"></a>身份和访问
- [管理单元](/graph/api/resources/administrativeunit?view=graph-rest-beta&preserve-view=true)[跟踪更改](/graph/api/administrativeunit-delta?view=graph-rest-beta&preserve-view=true)。
- [oAuth2PermissionGrant](/graph/api/resources/oauth2permissiongrant?view=graph-rest-beta&preserve-view=true)[跟踪更改](/graph/api/oauth2permissiongrant-delta?view=graph-rest-beta&preserve-view=true)。
- [管理](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta&preserve-view=true)用户的[身份验证方法](/graph/api/resources/authenticationmethod?view=graph-rest-beta&preserve-view=true)，其中包括[密码](/graph/api/resources/passwordauthenticationmethod?view=graph-rest-beta&preserve-view=true)或[电话](/graph/api/resources/phoneauthenticationmethod?view=graph-rest-beta&preserve-view=true)。例如，[重置用户密码](/graph/api/passwordauthenticationmethod-resetpassword?view=graph-rest-beta&preserve-view=true)并[获取重置状态](/graph/api/authenticationoperation-get?view=graph-rest-beta&preserve-view=true)，或者为用户[添加电话号码](/graph/api/authentication-post-phonemethods?view=graph-rest-beta&preserve-view=true)以进行短信或语音通话身份验证（如果策略为用户启用）。

### <a name="reports--identity-and-access-reports"></a>报告 | 身份和访问报告
[列出](/graph/api/relyingpartydetailedsummary-list?view=graph-rest-beta&preserve-view=true) Active Directory 联合身份验证服务中配置的[依赖方](/windows-server/identity/ad-fs/technical-reference/understanding-key-ad-fs-concepts)。

### <a name="reports--microsoft-365-usage-reports"></a>报告 | Microsoft 365 使用情况报告
查看 CSV 报告中的 **会议创建** 和 **会议互动** 数据，以查看 [电子邮件活动计数](/graph/api/reportroot-getemailactivitycounts?view=graph-rest-beta&preserve-view=true)、[电子邮件活动用户计数](/graph/api/reportroot-getemailactivityusercounts?view=graph-rest-beta&preserve-view=true)和 [电子邮件活动用户详细信息](/graph/api/reportroot-getemailactivityuserdetail?view=graph-rest-beta&preserve-view=true)。


## <a name="march-2020-new-and-generally-available"></a>2020 年 3 月：新版本和正式版

### <a name="cloud-communications"></a>云通信
- 获取呼叫路由和[呼叫](/graph/api/resources/call?view=graph-rest-1.0&preserve-view=true)的传入上下文。
- 对呼叫进行[录制状态更新](/graph/api/call-updaterecordingstatus?view=graph-rest-1.0&preserve-view=true)。
- 可为[参与者](/graph/api/resources/participant?view=graph-rest-1.0&preserve-view=true)指定录制信息，包括录制的发起人和状态。
- 使用 **callChainId** 属性唯一标识会议或参与者到参与者 [呼叫](/graph/api/resources/call?view=graph-rest-1.0&preserve-view=true)中的参与者。
- 可将参与者的国家/地区代码和终结点类型（例如 Skype for Business 或 Skype for Business VOIP）标识为 [participantInfo](/graph/api/resources/participantinfo?view=graph-rest-1.0&preserve-view=true) 的组成部分。
- 第三方视频电话会议 (VTC) 设备合作伙伴可以通过云视频互操作 (CVI) 机器人和 [logTeleconferenceDeviceQuality](/graph/api/call-logteleconferencedevicequality?view=graph-rest-1.0&preserve-view=true) 函数，记录并提供视频电话会议设备的媒体质量数据。媒体质量数据包括，[音频](/graph/api/resources/teleconferencedeviceaudioquality?view=graph-rest-1.0&preserve-view=true)、[视频](/graph/api/resources/teleconferencedevicevideoquality?view=graph-rest-1.0&preserve-view=true)和[屏幕共享](/graph/api/resources/teleconferencedevicescreensharingquality?view=graph-rest-1.0&preserve-view=true)的开放类型数据。

### <a name="files"></a>文件
- 与用户共享、添加至用户 OneDrive、或作为搜索结果返回的[远程项](/graph/api/resources/remoteitem?view=graph-rest-1.0&preserve-view=true)，包含图像或视频的元数据。
- [关注](/graph/api/driveitem-follow?view=graph-rest-1.0&preserve-view=true) [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0&preserve-view=true)，以便能够便捷访问或方便执行移动、复制和另存为等操作。 使用[取消关注](/graph/api/driveitem-unfollow?view=graph-rest-1.0&preserve-view=true)可停止关注驱动器项。
- 向用户[授予](/graph/api/permission-grant?view=graph-rest-1.0&preserve-view=true)访问共享链接的权限，以便共享相应的驱动器项。

### <a name="identity-and-access"></a>身份和访问
- [组织联系人](/graph/api/resources/orgcontact?view=graph-rest-1.0&preserve-view=true)[跟踪更改](/graph/api/orgcontact-delta?view=graph-rest-1.0&preserve-view=true)。
- 使用 **riskEventTypes_v2** 属性可获取与 [登录](/graph/api/resources/signin?view=graph-rest-1.0&preserve-view=true)相关的风险事件类型。
- 使用 `User.ManageIdentities.All` 委托的权限，可允许应用读取、更新或删除与登录用户有权访问的用户帐户关联的标识。 在没有登录用户的情况下，在应用程序级别使用此权限。 这样，应用可以[管理](/graph/api/user-update?view=graph-rest-1.0&preserve-view=true)用户能够使用哪些标识来登录。

### <a name="reports"></a>报告
将 Teams 服务管理员和 Teams 通信管理员用作接受的用户角色，允许应用代表用户以[用户委派的授权的形式](reportroot-authorization.md)读取 Microsoft 365 服务使用情况报告。 

### <a name="sites"></a>网站
- 让用户[关注](/graph/api/site-follow?view=graph-rest-1.0&preserve-view=true)或[取消关注](/graph/api/site-unfollow?view=graph-rest-1.0&preserve-view=true) SharePoint 网站。
- 针对 SharePoint [列表](/graph/api/resources/list?view=graph-rest-1.0&preserve-view=true)[订阅更改通知](/graph/api/resources/subscription?view=graph-rest-1.0&preserve-view=true)。 

## <a name="march-2020-new-in-preview-only"></a>2020 年 3 月：仅限预览版中的新增功能

### <a name="calendar"></a>日历
- 使用 **calendarGroupId** 属性可获取创建 [日历](/graph/api/resources/calendar?view=graph-rest-beta&preserve-view=true)的 [日历组](/graph/api/resources/calendargroup?view=graph-rest-beta&preserve-view=true)。
- 使用 **isDraft** 属性可将 [事件](/graph/api/resources/event?view=graph-rest-beta&preserve-view=true)标识为用户已在 Outlook 中更新但尚未发送给更新与会者的会议。

### <a name="cloud-communications"></a>云通信
- 使用 [createOrGet](/graph/api/onlinemeeting-createorget?view=graph-rest-beta&preserve-view=true) 按自定义外部 ID 获取[联机会议](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true)实例，并在不存在此实例时创建一个实例。
- 可选择使用 **externalId** 属性来标识具有自定义外部 ID 的联机会议。
- 使用可选的 `Accept-Language`HTTP 请求标头 [创建](/graph/api/application-post-onlinemeetings?view=graph-rest-beta&preserve-view=true)或 [获取](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true)联机会议实例，以在成功操作时，采用指定语言和区域设置显示 **joinInformation** 属性的内容。

### <a name="devices-and-apps"></a>设备和应用
Intune [3 月](changelog.md#march-2020)更新。

### <a name="identity-and-access"></a>标识和访问
- 使用 `Auditlogs.Read.All` 权限可列出[用户](/graph/api/resources/user?view=graph-rest-beta&preserve-view=true)的[登录活动](/graph/api/resources/signinactivity?view=graph-rest-beta&preserve-view=true)。
- 使用 [Azure 资源的 Privileged Identity Management (PIM)](/graph/api/resources/privilegedidentitymanagement-resources?view=graph-rest-beta&preserve-view=true) 的 `PrivilegedAccess.Read.AzureResources` 应用程序级别权限为管理组、订阅、资源组和资源级别的 Azure 基础结构角色设置实时访问工作流。
- 使用 [identitySecurityDefaultsEnforcementPolicy](/graph/api/resources/identitysecuritydefaultsenforcementpolicy?view=graph-rest-beta&preserve-view=true) 实体可[获取](/graph/api/identitysecuritydefaultsenforcementpolicy-get?view=graph-rest-beta&preserve-view=true)或[更新](/graph/api/identitysecuritydefaultsenforcementpolicy-update?view=graph-rest-beta&preserve-view=true)预配置的默认安全设置，以保护组织免受常见攻击。
- 调用条件访问 API 时，请使用 `identity` 段。 例如，要[获取](/graph/api/conditionalaccesspolicy-get?view=graph-rest-beta&preserve-view=true)[条件性访问策略](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta&preserve-view=true)：`GET https://graph.microsoft.com/beta/identity/conditionalAccess/policies/{id}`。
- 使用 **authenticationRequirement** 属性可获取通过所有登录步骤所需的最高级别的身份验证，以便 [登录](/graph/api/resources/signin?view=graph-rest-beta&preserve-view=true)成功。
- 在[列出租户中发生的预配事件](/graph/api/provisioningobjectsummary-list?view=graph-rest-beta&preserve-view=true)时，请使用分页。

### <a name="search"></a>搜索
- 若要将文件中的数据添加到搜索结果中，只需将数据作为 [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) 编制索引即可。**externalFile** 类型已被弃用。
- [更新](/graph/api/externalitem-update?view=graph-rest-beta&preserve-view=true)[索引中的项](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true)，具体方法为专门更新纯文本表示的项（用 **content** 属性表示），或项的属性包（用 **properties** 属性表示）。 由于更新属性包中的任何属性都会覆盖整个属性包，因此请务必在更新中显式添加项的所有属性。
- 在调用 **externalItem** 的 [create](/graph/api/externalconnection-put-items?view=graph-rest-beta&preserve-view=true)、[update](/graph/api/externalitem-update?view=graph-rest-beta&preserve-view=true) 或 [delete](/graph/api/externalitem-delete?view=graph-rest-beta&preserve-view=true) 操作后，检查 `HTTP 429` 和 `Retry-After` 响应头。 使用 `Retry-After` 延迟来回退请求是从[限制](throttling.md#best-practices-to-handle-throttling)中恢复的最快方法。

### <a name="teamwork"></a>团队合作
使用 `ChannelMessage.Read.All` 应用程序级别权限，在没有登录用户的情况下读取频道中的 [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta&preserve-view=true) 实例。

### <a name="universal-print"></a>通用打印
调试允许用户在 web 上或从应用程序上打印的[通用打印 API](universal-print-concept-overview.md)。 借助 API，IT 管理员能够在 Microsoft 365 云远程打印机中管理用户和组对打印机的访问权限，以保持可用性、监视打印机状态，报告存档的打印作业和使用情况。 

注意：自 2020 年 3 月起，通用打印 _服务_ 仅在个人预览版中提供。 参见[宣布推出通用打印：基于云的打印解决方案](https://aka.ms/announcinguniversalprint)，了解有关参与的详细信息。


## <a name="february-2020-new-and-generally-available"></a>2020 年 2 月：新版本和正式版

### <a name="calendar"></a>日历
浏览“[在共享或委派日历中创建事件](outlook-create-event-in-shared-delegated-calendar.md)”示例，或浏览可用于此流程期间的代理人、受邀者和日历所有者的操作与属性。

### <a name="identity-and-access"></a>身份和访问
- 为了提升在订阅“[更改用户通知](webhooks.md)”的安全性，强制在通知流程中使用的客户端和网站服务器上[强制执行传输层安全性（TLS）1.2](/configmgr/core/plan-design/security/enable-tls-1-2)或更高。 新要求自 2020 年 2 月 15 日起分阶段推出。 到 2020 年 5 月 15 日，所有通知端点必须符合新的 TLS 要求。 [找出推出阶段](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/)，如有必要，请使用新的 **latestSupportedTlsVersion** 属性作为临时解决方法，以避免订阅失败，然后再完成 TLS 升级。
- 使用相应类型的[威胁评估请求](/graph/api/resources/threatAssessmentRequest?view=graph-rest-1.0&preserve-view=true)跟踪[邮件](/graph/api/resources/mailassessmentrequest?view=graph-rest-1.0&preserve-view=true)、[电子邮件文件](/graph/api/resources/emailfileassessmentrequest?view=graph-rest-1.0&preserve-view=true)（.EML 文件）、[电子邮件附件文件](/graph/api/resources/fileassessmentrequest?view=graph-rest-1.0&preserve-view=true)（文本、Word 或二进制文件）或 [URL](/graph/api/resources/urlassessmentrequest?view=graph-rest-1.0&preserve-view=true) 中的威胁。

### <a name="users"></a>用户
[重新处理](/graph/api/user-reprocesslicenseassignment?view=graph-rest-1.0&preserve-view=true)[用户](/graph/api/resources/user?view=graph-rest-1.0&preserve-view=true)的所有基于组的许可证分配。


## <a name="february-2020-new-in-preview-only"></a>2020 年 2 月：仅限预览版中的新增功能

### <a name="calendar"></a>日历
参看“[管理日历共享和委派的预览版 API 所支持的任务](outlook-share-or-delegate-calendar.md)”。

### <a name="cloud-communications"></a>云通信

- 使用新的[通话记录](/graph/api/resources/callrecord?view=graph-rest-beta&preserve-view=true)资源，在 Microsoft Teams 和 Skype for Business 上为组织获取通话和联机会议的元数据。
- 对于会议中的参与者，请使用 **initiator** 属性获取 [记录](/graph/api/resources/recordinginfo?view=graph-rest-beta&preserve-view=true)（如果有）的发起人的标识信息。

### <a name="devices-and-apps"></a>设备和应用
Intune [2 月](changelog.md#february-2020)更新。

### <a name="groups"></a>组
使用 [assignLicense](/graph/api/group-assignlicense?view=graph-rest-beta&preserve-view=true) 方法将产品（如 Microsoft 365 或企业移动性 + 安全性）的许可证分配给组。 由于 Azure AD 可确保将许可证分配给组的成员，因此加入或离开组的成员不再需要单独级别的许可证管理。

### <a name="identity-and-access"></a>身份和访问
- 创建[访问包分配策略](/graph/api/resources/accesspackageassignmentpolicy?view=graph-rest-beta&preserve-view=true)时设置请求程序、审批和审阅设置。
- 使用 `/policies` URL 段并指定策略类型，访问[组织的特定类型的策略](/graph/api/resources/policy-overview?view=graph-rest-beta&preserve-view=true)。 例如，组织可以强制实施 Web 会话在一段时间不活动后自动从该会话注销用户的策略；请参阅 [activityBasedTimeoutPolicy](/graph/api/resources/activitybasedtimeoutpolicy?view=graph-rest-beta&preserve-view=true) 的实例的 CRUD 操作。 这是一项[重大更改](https://developer.microsoft.com/identity/blogs/breaking-changes-policy-api-microsoft-graph-beta/)，可以通过对 `/policies` 段下所有类型的策略进行分组，以便更易于发现所有策略。 采用类似的方法访问其他类型的策略：[claimsMappingPolicy](/graph/api/resources/claimsmappingpolicy?view=graph-rest-beta&preserve-view=true)、[homeRealmDiscoveryPolicy](/graph/api/resources/homerealmdiscoverypolicy?view=graph-rest-beta&preserve-view=true)、[tokenLifetimePolicy](/graph/api/resources/tokenlifetimepolicy?view=graph-rest-beta&preserve-view=true) 和 [tokenIssuancePolicy](/graph/api/resources/tokenissuancetimepolicy?view=graph-rest-beta&preserve-view=true)。 
- 使用应用程序级和委派的 `Policy.ReadWrite.ApplicationConfiguration` 权限，以读取和写入有关前一项中所述的应用程序配置[策略](/graph/api/resources/policy-overview?view=graph-rest-beta&preserve-view=true)的操作。

### <a name="teamwork"></a>团队合作
- 在组织中的所有频道消息或所有聊天消息中使用[更改通知](/graph/api/resources/webhooks?view=graph-rest-beta&preserve-view=true)。
- [拒绝](/graph/api/swapshiftschangerequest-decline?view=graph-rest-beta&preserve-view=true)与[团队](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true)中的其他用户[换班的请求](/graph/api/resources/swapshiftschangerequest?view=graph-rest-beta&preserve-view=true)。

## <a name="january-2020-new-and-generally-available"></a>2020 年 1 月：新版本和正式版

### <a name="security"></a>安全性
作为客户警报管理的一部分，请使用 [update alert](/graph/api/alert-update?view=graph-rest-1.0&preserve-view=true) 方法并将“**注释**”字段更新为 `Closed in IPC` 或 `Closed in MCAS`。

### <a name="teamwork"></a>团队合作
使用“[团队](/graph/api/resources/team?view=graph-rest-1.0&preserve-view=true)”的 **primaryChannel** 导航属性来访问默认频道，“**常规**”。

### <a name="users"></a>用户
使用“**标识**”属性访问 [用户](/graph/api/resources/user?view=graph-rest-1.0&preserve-view=true)可用于登录至 Azure AD 用户账户的一个或多个标识。 这些标识可由 Microsoft，组织或 Facebook、Google 或 Microsoft 等社交标识提供商提供。 此属性允许用户使用任一这些身份登录至用户账户。

## <a name="january-2020-new-in-preview"></a>2020 年 1 月：预览版新增功能

### <a name="devices-and-apps"></a>设备和应用
Intune [1 月](changelog.md#january-2020)更新。


## <a name="december-2019-new-and-generally-available"></a>2019 年 12 月：新版本和正式版

### <a name="cloud-communications"></a>云通信
云通信 API 已正式发布，适用于[呼叫](/graph/api/resources/call?view=graph-rest-1.0&preserve-view=true)和[联机会议](/graph/api/resources/onlinemeeting?view=graph-rest-1.0&preserve-view=true)的 API [在 v1.0 中可用](/graph/api/resources/communications-api-overview?view=graph-rest-1.0&preserve-view=true)。

### <a name="education"></a>教育
使用 **classSettings** 属性管理课程专属设置，例如启用发送每周作业摘要的操作。 当团队表示[教育课程](/graph/api/resources/educationclass?view=graph-rest-1.0&preserve-view=true)时，此属性可在[团队](/graph/api/resources/team?view=graph-rest-1.0&preserve-view=true)资源中使用。

### <a name="identity-and-access"></a>标识和访问 
[尝试使用有限权限获取容器对象会返回部分数据](permissions-reference.md#limited-information-returned-for-inaccessible-member-objects)。 例如，与 [用户](/graph/api/resources/user?view=graph-rest-1.0&preserve-view=true)、另一个 **组** 和 [设备](/graph/api/resources/device?view=graph-rest-1.0&preserve-view=true)关联的 [组](/graph/api/resources/group?view=graph-rest-1.0&preserve-view=true)实例。 只有 User.Read.All 和 Group.Read.All 权限且正在尝试访问此 **组** 实例的应用将获取 **用户** 和 **组** 实例，但获得的 **设备** 对象数据有限（仅限数据类型和对象 ID，不包括属性值）。

### <a name="people-and-workplace-intelligence"></a>人员和工作场所智能
见解 API 已正式发布。在生产应用中使用此 API，以确定具有以下特征的最相关文档：

- 用户的[常用文档](/graph/api/insights-list-trending?view=graph-rest-1.0&preserve-view=true)
- 用户[使用的](/graph/api/insights-list-used?view=graph-rest-1.0&preserve-view=true)文档
- [与用户共享由用户共享的](/graph/api/insights-list-shared?view=graph-rest-1.0&preserve-view=true)文档

### <a name="reports"></a>报告
要使用用户委派的权限获取 Microsoft 365 使用情况报告，管理员必须向该用户分配 Azure AD 受限管理员角色。 可以是以下角色之一：公司管理员、Exchange 管理员、SharePoint 管理员、Lync 管理员、全局读取者或报告读取者。 有关详细信息，请参阅[授权 API 读取 Microsoft 365 使用情况报告](reportroot-authorization.md)。

### <a name="toolkit"></a>工具包
Microsoft Graph 工具包 v1.1 已发布。有关增强功能和 bug 修复的列表，请参阅更改日历的“[2019 年 12 月部分](changelog.md#december-2019)”。

## <a name="december-2019-new-in-preview"></a>2019年12月：预览版新增功能

### <a name="cloud-communications"></a>云通信
- 使用新的[状态](/graph/api/resources/presence?view=graph-rest-beta&preserve-view=true)资源了解一名或多名用户的忙闲状态和当前活动。
- [删除](/graph/api/onlinemeeting-delete?view=graph-rest-beta&preserve-view=true)[联机会议](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true)资源的实例。
- 要重命名和删除[呼叫](/graph/api/resources/call?view=graph-rest-beta&preserve-view=true)和[联机会议](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true)资源的几个成员以便与这些资源的 v1 版本一致，请参阅更改日志的[“2019 年 12 月”部分](changelog.md#december-2019)。

### <a name="devices-and-apps"></a>设备和应用
Intune [12 月](changelog.md#december-2019)更新

### <a name="identity-and-access"></a>标识和访问 
- 修复了 [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true) 上 **appRoleAssignments** 和 **appRoleAssignedTo** 关系的行为。
- 使用 [Azure AD 权利管理](/graph/api/resources/entitlementmanagement-root?view=graph-rest-beta&preserve-view=true)中的 [accessPackageResourceRequest](/graph/api/resources/accesspackageresourcerequest?view=graph-rest-beta&preserve-view=true) 来请求将资源添加到 [目录](/graph/api/resources/accesspackagecatalog?view=graph-rest-beta&preserve-view=true)中，以便可在[访问包](/graph/api/resources/accesspackage?view=graph-rest-beta&preserve-view=true)中使用该资源的角色。
- 使用[威胁评估 API](/graph/api/resources/threatassessment-api-overview?view=graph-rest-beta&preserve-view=true) 帮助管理员报告可疑电子邮件、网络钓鱼 URL、电子邮件附件或其他文件。 然后，线程扫描判定会通知他们相应地调整组织策略。

### <a name="teamwork"></a>团队合作
- 针对[chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta&preserve-view=true)资源在 Microsoft 团队频道和聊天中[设置包含资源数据的更改通知](webhooks-with-resource-data.md)。
- 针对新的或已更改的[频道消息或聊天消息](/graph/api/resources/chatmessage?view=graph-rest-beta&preserve-view=true)[订阅通知](/graph/api/resources/subscription?view=graph-rest-beta&preserve-view=true)。
- 借助 [shiftPreferences](/graph/api/resources/shiftpreferences?view=graph-rest-beta&preserve-view=true) 资源，可在[日程安排](/graph/api/resources/schedule?view=graph-rest-beta&preserve-view=true)中将用户的忙线状态指定为“已分配排班”。 作为用户的[设置](/graph/api/resources/usersettings?view=graph-rest-beta&preserve-view=true)的一部分获取或设置此信息。


## <a name="november-2019-new-and-generally-available"></a>2019 年 11 月：新版本和正式版

### <a name="groups"></a>组
- 使用委派或应用程序权限GroupMember.Read.All和GroupMember.ReadWrite.Al，来列出组、读取基本组属性，读取（并更新，如有读写权限）能够访问应用程序组的成员身份。
- 使用应用程序权限Group.Create，创建不含已登录用户的组。
- 对于指定的 [组](/graph/api/resources/group?view=graph-rest-1.0&preserve-view=true)，在其它组或目录角色中[检查成员身份](/graph/api/group-checkmemberobjects?view=graph-rest-1.0&preserve-view=true)。

### <a name="identity-and-access"></a>身份和访问
- 注册通过 Azure Active Directory (Azure AD) 进行身份验证的[应用程序](/graph/api/resources/application?view=graph-rest-1.0&preserve-view=true)。 根据需要使用委派的[权限](./permissions-reference.md#application-resource-permissions)（即 Application.Read.All 和 Application.ReadWrite.All）或应用程序权限（即 Application.Read.All）。
- 对于指定的 [设备](/graph/api/resources/device?view=graph-rest-1.0&preserve-view=true)，在其它组或目录角色中[检查成员身份](/graph/api/device-checkmemberobjects?view=graph-rest-1.0&preserve-view=true)。

### <a name="mail"></a>邮件
- 使用 **conversationIndex** 属性可获取邮件在 Outlook 电子邮件对话中的位置。
- 使用委派权限Mail.ReadBasic和应用程序权限Mail.ReadBasic.All，来获取[邮件](/graph/api/resources/message?view=graph-rest-1.0&preserve-view=true)或[邮件文件夹](/graph/api/resources/mailfolder?view=graph-rest-1.0&preserve-view=true)资源，跟踪更改，并针对邮件的更改通知管理[订阅](/graph/api/resources/subscription?view=graph-rest-1.0&preserve-view=true)。

### <a name="users"></a>用户
- 针对指定的[用户](/graph/api/resources/user?view=graph-rest-1.0&preserve-view=true)，[检查组成员身份](/graph/api/user-checkmemberobjects?view=graph-rest-1.0&preserve-view=true)。
- 使用 **creationType** 属性查找用户帐户的创建方式，例如，是将帐户创建为普通学校或工作帐户还是作为外部帐户等。

## <a name="november-2019-new-in-preview"></a>2019 年 11 月：预览版中的新增功能

### <a name="calendar"></a>日历
- [使用 Outlook 组织或参加联机会议](outlook-calendar-online-meetings.md)。
- [为](/graph/api/place-update?view=graph-rest-beta&preserve-view=true)[会议室](/graph/api/resources/room?view=graph-rest-beta&preserve-view=true)和[会议室列表](/graph/api/resources/roomlist?view=graph-rest-beta&preserve-view=true)的丰富位置类型设置属性。

### <a name="cloud-communication"></a>云通信
[呼叫](/graph/api/resources/call?view=graph-rest-beta&preserve-view=true) 资源类型支持以下附加功能：

- [传入呼叫上下文](/graph/api/resources/incomingcontext?view=graph-rest-beta&preserve-view=true)
- 参与者的终结点类型，例如语音邮件或Skype for Business
- [更新](/graph/api/call-updaterecordingstatus?view=graph-rest-beta&preserve-view=true)[参与者](/graph/api/resources/participant?view=graph-rest-beta&preserve-view=true)[录制](/graph/api/resources/recordinginfo?view=graph-rest-beta&preserve-view=true)信息的能力

### <a name="devices-and-apps"></a>设备和应用
Intune [11 月](changelog.md#november-2019)更新

### <a name="education"></a>教育
管理员能够通过与 [类](/graph/api/resources/educationclass?view=graph-rest-beta&preserve-view=true)相关的 [团队](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true)  **classSettings** 属性启用全类设置。 .当前没有关于向监护人通知每周分配的设置。

### <a name="identity-and-access"></a>身份和访问
- 使用应用程序权限Policy.Read.All 读取组织的条件访问策略和命名位置，无需登录用户存在。
- 允许 [条件访问策略](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta&preserve-view=true) 处于仅报告状态，`enabledForReportingButNotEnforced`。
- 使用委派权限ThreatAssessment.ReadWrite.All 或应用程序权限ThreatAssessment.Read.All，来读取（或创建，如果有读写权限）组织威胁存取请求。

### <a name="mail"></a>邮件
使用委派权限Mail.ReadBasic和应用程序权限Mail.ReadBasic.All，来管理更改[消息](/graph/api/resources/message?view=graph-rest-beta&preserve-view=true)资源更改通知的[订阅](/graph/api/resources/subscription?view=graph-rest-beta&preserve-view=true) 。

### <a name="notifications"></a>通知
使用新的轻量级通知 [Web SDK](https://aka.ms/GNSDK) 代替 [Project Rome SDK](https://github.com/Microsoft/project-rome)，以利用改进的身份验证模型和对使用 Web 推送的 Web 应用的支持。 

### <a name="people-and-workplace-intelligence"></a>人员和工作场所智能
首次推出的[配置文件](/graph/api/resources/profile?view=graph-rest-beta&preserve-view=true)资源，这是 Microsoft 服务中下一代人脉实体的丰富表示形式。 此资源与常见和切实可行的人脉属性有关，包括任何有意义的日期（如[周年纪念日](/graph/api/resources/personanniversary?view=graph-rest-beta&preserve-view=true)）的信息、[教育](/graph/api/resources/educationalactivity?view=graph-rest-beta&preserve-view=true)、[就业岗位](/graph/api/resources/workposition?view=graph-rest-beta&preserve-view=true)、[兴趣](/graph/api/resources/personinterest?view=graph-rest-beta&preserve-view=true)、[语言](/graph/api/resources/languageproficiency?view=graph-rest-beta&preserve-view=true)和[技能](/graph/api/resources/skillproficiency?view=graph-rest-beta&preserve-view=true)熟练程度、[项目参与](/graph/api/resources/projectparticipation?view=graph-rest-beta&preserve-view=true)、[网站关联](/graph/api/resources/personwebsite?view=graph-rest-beta&preserve-view=true)以及其他[帐户](/graph/api/resources/useraccountinformation?view=graph-rest-beta&preserve-view=true)和联系人信息。

### <a name="search"></a>搜索
首次推出的 [Microsoft 搜索 API](search-concept-overview.md)，它使应用用户可以获得由 Microsoft Graph 支持的更多最新、个性化和相关的搜索结果。 使用[查询](/graph/api/search-query?view=graph-rest-beta&preserve-view=true)功能，该功能默认情况下在 Microsoft 云中搜索 Outlook 邮件和事件以及 OneDrive 和 SharePoint 文件。 使用 [Microsoft Graph 连接器库](/microsoftsearch/connectors-gallery)中的[连接器](/microsoftsearch/connectors-overview)，将搜索数据包括在 Microsoft 云外部。 或者，[生成自己的连接器](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true#common-use-cases)、索引外部自定义项目和文件以及查询特定外部数据源。

### <a name="teamwork"></a>团队合作
使用以下 HTTP 请求语法获取与[团队](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true)和[频道](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true)相关的[文件](/graph/api/resources/driveitem?view=graph-rest-beta&preserve-view=true)资源：

```http
GET /teams/{teamId}/channels/{channelId}/filesFolder
```

### <a name="users"></a>用户
使用 **creationType** 属性查找用户帐户的创建方式，例如，是将帐户创建为普通学校或工作帐户还是作为外部帐户等。


## <a name="october-2019-new-and-generally-available"></a>2019 年 10 月：新版本和正式版

### <a name="identity-and-access"></a>身份和访问
- 在生产应用中使用[组织联系人](/graph/api/resources/orgcontact?view=graph-rest-1.0&preserve-view=true)。组织联系人由组织管理员管理，可以从本地 Active Directory 或 Exchange Online 同步。
- 在[组织](/graph/api/resources/organization?view=graph-rest-1.0&preserve-view=true)中配置[基于证书的身份验证](/azure/active-directory/authentication/active-directory-certificate-based-authentication-get-started)。
- 为[应用程序](/graph/api/resources/application?view=graph-rest-1.0&preserve-view=true)添加和删除[密码凭据](/graph/api/resources/passwordcredential?view=graph-rest-1.0&preserve-view=true)。

### <a name="mail"></a>邮件
使用新的 **message** 参数更新 [回复](/graph/api/message-reply?view=graph-rest-1.0&preserve-view=true)邮件时任何可写的 [message](/graph/api/resources/message?view=graph-rest-1.0&preserve-view=true) 属性，例如，[将收件人添加到回复](/graph/api/message-reply#example?view=graph-rest-1.0&preserve-view=true)。

### <a name="microsoft-graph-data-connect"></a>Microsoft Graph 数据连接
开发人员和数据科学家现在可以使用[工具将 Office 365 数据转换为通用数据模型格式](https://github.com/OfficeDev/MS-Graph-Data-Connect/blob/master/Common-Data-Model/README.md)，从而使其与其他支持开放数据倡议 (ODI) 的数据集大致保持一致。 


### <a name="microsoft-graph-sdks"></a>Microsoft Graph SDK
- 使用 JavaScript SDK 中的混乱处理程序来验证应用程序是否可以应对棘手的服务器故障。
- 了解有关[使用 SDK 进行 API 调用](./sdks/create-requests.md)的信息。

### <a name="users"></a>用户
- [获取](/graph/api/user-get-mailboxsettings?view=graph-rest-1.0&preserve-view=true)或[设置](/graph/api/user-update-mailboxsettings?view=graph-rest-1.0&preserve-view=true)[用户邮箱](/graph/api/resources/mailboxsettings?view=graph-rest-1.0&preserve-view=true)的用户首选日期和时间格式设置。 
- 跟踪[用户](/graph/api/resources/user?view=graph-rest-1.0&preserve-view=true)上一次密码更改的日期/时间。

## <a name="october-2019-new-in-preview"></a>2019 年 10 月：预览版中的新增功能

### <a name="calendar"></a>日历
- 会议组织者可以[允许被邀请者提议备选会议时间](outlook-calendar-meeting-proposals.md)。 当收到包含建议的备选时间的会议响应时，组织者可以决定接受该建议并[更新](/graph/api/event-update?view=graph-rest-beta&preserve-view=true)会议时间。
- 编程日历共享与 Outlook 用户体验的奇偶校验更加接近。 除了跟踪日历的当前用户权限和共享状态之外：
  - 对于每个[日历](/graph/api/resources/calendar?view=graph-rest-beta&preserve-view=true)，你现在可以管理与之共享日历的每个用户的[权限](/graph/api/resources/calendarpermission?view=graph-rest-beta&preserve-view=true)。 
  - 对于每个[邮箱](/graph/api/resources/mailboxsettings?view=graph-rest-beta&preserve-view=true)，你现在可以指定代理人、邮箱所有者，还是两者同时接收会议邮件和会议响应。 
- 其他在线会议支持：
  - 对于每个 **日历**，指定允许的和默认的在线会议提供程序。
  - 创建或更新[事件](/graph/api/resources/event?view=graph-rest-beta&preserve-view=true)以使其在线可用，并提供详细信息供与会者加入在线会议。 
  - 具体来说，使用 **事件** 的新 **onlineMeetingProvider** 和 **onlineMeeting** 属性来将 Microsoft Teams 设置或标识为在线会议提供程序，这是 **onlineMeetingUrl** 属性的 [已知问题](known-issues.md#onlinemeetingurl-property-support-for-microsoft-teams)的解决方法。

### <a name="devices-and-apps"></a>设备和应用
Intune [10 月](changelog.md#october-2019)更新

### <a name="graph-explorer"></a>Graph 浏览器
尝试使用[下一版本的 Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer/preview)，并在新的“权限”、“身份验证”和“代码片段”选项卡中查看权限、访问令牌和 SDK 代码片段等便捷的上下文信息。 使用“预览”滑块在[生产](https://developer.microsoft.com/graph/graph-explorer)和 Graph Explorer 的新预览版本之间切换。

### <a name="groups"></a>组
- 使用 **hideFromAddressLists** 和 **hideFromOutlookClients** 属性在 Outlook 用户界面的某些部分或 Outlook 客户端中控制 [组](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true)的可见性。
- [分配](/graph/api/group-assignlicense?view=graph-rest-beta&preserve-view=true)或删除[组](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true)中用户的许可证。

### <a name="identity-and-access"></a>标识和访问
- 使用[条件访问策略](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta&preserve-view=true)自定义组织的访问规则。 这些规则会考虑有关用户或设备标识（如用户或组成员身份、IP 位置）的信号，以及尝试访问特定应用程序等行为和有风险的登录行为。
- 使用[权利管理](/graph/api/resources/entitlementmanagement-root?view=graph-rest-beta&preserve-view=true)来管理组织内外的用户对组、应用程序和 SharePoint Online 网站的访问。
- 为[应用程序](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true)和[服务主体](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true)添加和删除[密码凭据](/graph/api/resources/passwordcredential?view=graph-rest-beta&preserve-view=true)。
- 管理 Azure AD B2C [信任框架策略密钥](/graph/api/resources/trustframeworkkeyset?view=graph-rest-beta&preserve-view=true)。
- 定义 Azure AD B2C [用户流](/graph/api/resources/identityuserflow?view=graph-rest-beta&preserve-view=true)策略，用于登录、注册、合并注册和登录、密码重置和配置文件更新。
- 配置[信息保护标签](/graph/api/resources/informationprotectionlabel?view=graph-rest-beta&preserve-view=true)以对用户或租户的敏感度进行分类。
- 将 API 用于[标识风险事件](/graph/api/resources/identityriskevent?view=graph-rest-beta&preserve-view=true)的现有应用应转换为适用于 Azure AD Identity Protection 中[风险检测](/graph/api/resources/riskdetection?view=graph-rest-beta&preserve-view=true)的应用。 有关更多详细信息和弃用时间线，请参阅相关的[博客文章](https://developer.microsoft.com/graph/blogs/deprecatation-of-the-identityriskevents-api/)。


### <a name="mail"></a>邮件
通过创建[上载会话](/graph/api/resources/uploadsession?view=graph-rest-beta&preserve-view=true)，[将高达 150MB 的大文件附加到](outlook-large-attachments.md) [message](/graph/api/resources/message?view=graph-rest-beta&preserve-view=true) 实例，并迭代上载文件的范围，直至文件的所有字节都已上载。 

### <a name="microsoft-graph-security-api"></a>Microsoft Graph 安全性 API
- 预览版与 RSA NetWitness、ServiceNow 和 Splunk 集成，以关联和同步[警报](/graph/api/resources/security-api-overview?view=graph-rest-beta&preserve-view=true#alerts)，并改善威胁防护和响应。
- 已将新触发器添加到适用于逻辑应用和流的 [Microsoft Graph 安全连接器](/connectors/microsoftgraphsecurity/)和 [playbook](/azure/security-center/security-center-playbooks) 中。 请参阅 [playbook 示例](https://github.com/microsoftgraph/security-api-solutions/tree/master/Playbooks)。
- 支持向 Microsoft Defender ATP 发送[威胁指示器](/graph/api/resources/security-api-overview?view=graph-rest-beta&preserve-view=true#threat-indicators-preview)，以使用其自己的智能源阻止威胁或发出威胁警报。 通过与 ThreatConnect 等合作伙伴集成，客户能够直接从威胁智能和自动化解决方案发送指示器。 

### <a name="notifications"></a>通知
- [创建通知并将其发送给用户登录的所有设备终结点上的所有应用程序客户端](/graph/api/user-post-notifications?view=graph-rest-beta&preserve-view=true)，而无需管理用户委派的权限。
- 在用户[通知](/graph/api/resources/notification?view=graph-rest-beta&preserve-view=true)上使用[目标策略终结点](/graph/api/resources/targetpolicyendpoints?view=graph-rest-beta&preserve-view=true)，以便专门针对 Windows、iOS、Android 或 WebPush 平台投放通知。
- 在 iOS 终结点的通知上指定[回退策略](/graph/api/resources/fallbackpolicy?view=graph-rest-beta&preserve-view=true)，以便发送由于平台特定的限制（如节电模式）而可能无法传递到设备的高优先级原始通知。

 
### <a name="powershell-sdk"></a>PowerShell SDK 
开发人员和 IT 专业人员会注意到推出了 [Microsoft Graph Powershell SDK](https://github.com/microsoftgraph/msgraph-sdk-powershell)，该 SDK 将生成包含用于发出 Microsoft Graph REST API 请求的 cmdlet 的模块。

## <a name="september-2019-new-and-generally-available"></a>2019 年 9 月：新版本和正式版

### <a name="calendar-mail-and-group"></a>日历、邮件和组
[获取文件的原始内容或项目的 MIME 内容](/graph/api/attachment-get?view=graph-rest-1.0&preserve-view=true#get-the-raw-contents-of-a-file-or-item-attachment)，该项目已作为[附件](/graph/api/resources/attachment?view=graph-rest-1.0&preserve-view=true)添加到[事件](/graph/api/resources/event?view=graph-rest-1.0&preserve-view=true)、[邮件](/graph/api/resources/message?view=graph-rest-1.0&preserve-view=true)或组[帖子](/graph/api/resources/post?view=graph-rest-1.0&preserve-view=true)。

### <a name="calendar-mail-outlook-task-personal-contact"></a>日历、邮件、Outlook 任务、个人联系人
使用 [translateExchangeId](/graph/api/user-translateexchangeids?view=graph-rest-1.0&preserve-view=true) 函数在受支持的[格式](/graph/api/user-translateexchangeids?view=graph-rest-1.0&preserve-view=true#exchangeidformat-values)之间转换 Outlook 项目 ID，包括 Microsoft Graph 默认 ID 格式和不可变的 ID 格式。 

以下资源支持 ID 格式转换：

- [附件](/graph/api/resources/attachment?view=graph-rest-1.0&preserve-view=true)
- [联系人](/graph/api/resources/contact?view=graph-rest-1.0&preserve-view=true)
- [事件](/graph/api/resources/event?view=graph-rest-1.0&preserve-view=true)
- [eventMessage](/graph/api/resources/eventmessage?view=graph-rest-1.0&preserve-view=true)
- [邮件](/graph/api/resources/message?view=graph-rest-1.0&preserve-view=true)
- [outlookTask](/graph/api/resources/outlooktask?view=graph-rest-1.0&preserve-view=true)

### <a name="mail"></a>邮件
[获取邮件的 MIME 内容](outlook-get-mime-message.md)。

### <a name="microsoft-graph-toolkit"></a>Microsoft Graph 工具包
使用 [Microsoft Graph 工具包](toolkit/overview.md)开发生产应用，该应用提供一致的 Microsoft 365 外观，可以节省从 Microsoft Graph 进行身份验证和访问数据的时间。

## <a name="september-2019-new-in-preview"></a>2019 年 9 月：预览版中的新增功能

> [!IMPORTANT]
> _预览_ 状态下的功能（包括 API 和工具）可能会发生更改，恕不另行通知，有些功能可能永远不会提升为 GA 状态。 请不要在成品应用中使用它们。

### <a name="devices-and-apps"></a>设备和应用
Intune [9 月](changelog.md#september-2019)更新

### <a name="files"></a>文件
- 增强的同步支持：

  - 使用新的 **pendingOperations** 属性标识可能影响 [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta&preserve-view=true) 的二进制内容的操作。
  - [还原](/graph/api/driveitem-restore?view=graph-rest-beta&preserve-view=true)已删除的 **driveItem**。 
- 使用安全哈希算法 (SHA-256) 增强[文件](/graph/api/resources/file?view=graph-rest-beta&preserve-view=true)数据安全性和完整性。
- 获取或设置[照片](/graph/api/resources/photo?view=graph-rest-beta&preserve-view=true)的方向。 OneDrive 个人版上支持设置。

### <a name="identity-and-access"></a>标识和访问
- 使用新的 **identities** 属性并获取 [用户](/graph/api/resources/user?view=graph-rest-beta&preserve-view=true)可用于登录帐户的标识。 这些标识可由组织或诸如 Facebook、Google 和 Microsoft 等社交标识提供者提供。
- 用于在租户的云应用程序中[同步标识](/graph/api/resources/synchronization-overview?view=graph-rest-beta&preserve-view=true)的增强功能：

  - 存储[同步作业](/graph/api/resources/synchronization-synchronizationjob?view=graph-rest-beta&preserve-view=true)的设置
  - 指定对同步作业施加[隔离](/graph/api/resources/synchronization-quarantine?view=graph-rest-beta&preserve-view=true)的原因

### <a name="teamwork"></a>团队合作
使用 [团队](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true)的 **常规** 频道或自定义 [成员设置](/graph/api/resources/teammembersettings?view=graph-rest-beta&preserve-view=true)，让团队成员在 **团队** 中创建专用频道。

### <a name="users"></a>用户
- 获取或更新[用户](/graph/api/resources/user?view=graph-rest-beta&preserve-view=true)用于登录帐户的标识。 这些标识可由商业组织或诸如 Facebook、Google 和 Microsoft 等社交标识提供者提供。
- 获取或更新用户的[邮箱首选日期和时间格式设置](/graph/api/resources/mailboxsettings?view=graph-rest-beta&preserve-view=true)。


## <a name="august-2019-new-and-generally-available"></a>2019 年 8 月：新版本和正式版 

### <a name="reports"></a>报告
- 获取与已删除的项目计数和大小相关的其他[邮箱使用情况数据](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-1.0&preserve-view=true)。
- 在[获取组活动详细信息](/graph/api/reportroot-getoffice365groupsactivitydetail?view=graph-rest-1.0&preserve-view=true)时，跟踪 Microsoft 365 组 ID。
- 在获取 [OneDrive 使用帐户详细信息](/graph/api/reportroot-getonedriveusageaccountdetail?view=graph-rest-1.0&preserve-view=true)和 [SharePoint 网站使用情况详细信息](/graph/api/reportroot-getsharepointsiteusagedetail?view=graph-rest-1.0&preserve-view=true)时，跟踪所有者主体名称。
- 在[获取每 Microsoft 365 服务的用户计数报告](/graph/api/reportroot-getoffice365servicesusercounts?view=graph-rest-1.0&preserve-view=true)时，获取 Microsoft 365 上的活动和非活动用户数。

### <a name="security"></a>安全性
- 使用新的[适用于 Splunk 的 Microsoft Graph 安全性 API 加载项](https://aka.ms/graphsecuritysplunkaddon)将多个合作伙伴产品的安全警报和看法传输至 Splunk，从而更轻松地实时关联其安全性数据。 有关详细信息，请参阅[公告](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Introducing-the-new-Microsoft-Graph-Security-API-add-on-for/ba-p/815972)。 
- [查看由 Microsoft 或者与安全性 API 相关的 Microsoft 合作伙伴构建的其他解决方案和连接器列表](security-integration.md)，使你以统一的格式使用数据。


## <a name="august-2019-new-in-preview"></a>2019 年 8 月：预览版新增功能

> [!IMPORTANT]
> _预览_ 状态下的功能（包括 API 和工具）可能会发生变更，恕不另行通知；一些功能可能永远不会升级为 GA 状态。 请不要在成品应用中使用它们。

### <a name="devices-and-apps"></a>设备和应用
Intune [8 月](changelog.md#august-2019)更新

### <a name="education"></a>教育版
- 将[教师](/graph/api/resources/educationuser?view=graph-rest-beta&preserve-view=true)或[作业](/graph/api/resources/educationassignment?view=graph-rest-beta&preserve-view=true)与[评分标准](/graph/api/resources/educationrubric?view=graph-rest-beta&preserve-view=true)相关联，以解释特定作业质量和等级。 质量示例为拼写和语法，等级示例为“良好”和“不良”。 可以进一步将点数和权重与评分标准相关联。 有关详细信息，请参阅[教育版评分标准概述](education-rubric-overview.md)。
- 评估作业并从[反馈](/graph/api/resources/educationfeedbackoutcome?view=graph-rest-beta&preserve-view=true)、[数字等级](/graph/api/resources/educationpointsoutcome?view=graph-rest-beta&preserve-view=true)或[评分标准](/graph/api/resources/educationrubricoutcome?view=graph-rest-beta&preserve-view=true)方面展示结果。

### <a name="files"></a>文件
到目前为止，你已可以[关注](/graph/api/driveitem-follow?view=graph-rest-beta&preserve-view=true) [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta&preserve-view=true)，以便能够便捷访问或方便执行移动、复制和另存为等操作。 现在可以使用[取消关注](/graph/api/driveitem-unfollow?view=graph-rest-beta&preserve-view=true)操作来停止关注此类驱动器项。

### <a name="identity-and-access"></a>身份和访问
- 基于角色的访问控制 (RBAC) 提供商可以在 Azure Active Director 中[管理角色](/graph/api/resources/rolemanagement?view=graph-rest-beta&preserve-view=true)，方法是[定义可以在特定资源上执行的角色操作](/graph/api/resources/unifiedroledefinition?view=graph-rest-beta&preserve-view=true)，基于这些角色定义为用户[分配角色](/graph/api/resources/unifiedroleassignment?view=graph-rest-beta&preserve-view=true)，为他们授权相应的资源访问权限。
- 管理员可以[列出访问审查](/graph/api/accessreview-list?view=graph-rest-beta&preserve-view=true)，以高效地审核组成员身份、企业应用程序访问权限和角色分配。 定期访问审查可确保只有相应的人员才能继续以特定方式访问资源。

### <a name="social-and-workplace-intelligence"></a>社交和工作场所智能
最终用户可以使用 Microsoft 365 [MyAnalytics](social-intel-concept-overview.md#why-integrate-with-document-based-insights) 应用获取与管理时间、工作协作和工作生活平衡有关的见解。 现在，你可以使用[分析 API](/graph/api/resources/social-overview?view=graph-rest-beta&preserve-view=true#help-users-gain-insights-into-their-work-patterns) 整合与工作活动（如呼叫、聊天和电子邮件）所花时间相关的数据、以帮助提高用户的工作效率和幸福感。 


## <a name="july-2019-new-and-generally-available"></a>2019 年 7 月：新版本和正式版 

### <a name="example-code-snippets"></a>代码片段示例
现在 v1.0 和 beta 参考中的所有 API 主题中提供了 Objective-C 代码片段。 请参阅[获取事件](/graph/api/event-get?view=graph-rest-1.0&preserve-view=true&tabs=objective-c#example)的 Objective-C 示例。

### <a name="group"></a>Group
- 使用 [validateProperties](/graph/api/group-validateproperties?view=graph-rest-1.0&preserve-view=true) 函数确保现有 Microsoft 365 组的显示名称和邮件昵称符合命名策略。
- 或者，在创建组之前，可以为 [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0&preserve-view=true) 使用 [validateProperties](/graph/api/directoryobject-validateproperties?view=graph-rest-1.0&preserve-view=true) 函数来首先验证名称。

### <a name="identity-and-access"></a>身份和访问
- 使用 [新的委派和应用程序权限](permissions-reference.md#organization-permissions)、_Organization.Read.All_ 和 _Organization.ReadWrite.All_ 来访问 [组织](/graph/api/resources/organization?view=graph-rest-1.0&preserve-view=true)和相关资源，例如 [订阅的 SKU](/graph/api/resources/subscribedsku?view=graph-rest-1.0&preserve-view=true)。
- 使用 [新的委派和应用程序权限](permissions-reference.md#role-management-permissions)、_RoleManagement.Read.Directory_ 和 _RoleManagement.ReadWrite.Directory_，对于公司目录中的与角色的访问控制 (RBAC)：

  - 使用读取/写入权限来首先[激活](/graph/api/directoryrole-post-directoryroles?view=graph-rest-1.0&preserve-view=true)目录角色。 
  - 激活角色之后，可以使用读取权限来[读取目录角色](/graph/api/directoryrole-list?view=graph-rest-1.0&preserve-view=true)、[列出角色成员](/graph/api/directoryrole-list-members?view=graph-rest-1.0&preserve-view=true)和[列出目录角色模板](/graph/api/directoryroletemplate-list?view=graph-rest-1.0&preserve-view=true)。 
  - 还可以使用读取/写入权限来[添加](/graph/api/directoryrole-post-members?view=graph-rest-1.0&preserve-view=true)和[删除](/graph/api/directoryrole-delete-member?view=graph-rest-1.0&preserve-view=true)角色成员。


## <a name="july-2019-new-in-preview"></a>2019 年 7 月：预览版新增功能

> [!IMPORTANT]
> _预览_ 状态下的功能（包括 API 和工具）可能会发生更改，恕不另行通知，有些功能可能永远不会提升为 GA 状态。 请不要在生产应用中使用它们。

### <a name="calendar"></a>日历 
按照 Exchange Online 管理员的设置，使用新的[位置 API](/graph/api/resources/place?view=graph-rest-beta&preserve-view=true) 来使用诸如 [room](/graph/api/resources/room?view=graph-rest-beta&preserve-view=true) 和 [room list](/graph/api/resources/roomlist?view=graph-rest-beta&preserve-view=true) 之类的富位置类型。

### <a name="devices-and-apps"></a>设备和应用
Intune [7 月](changelog.md#july-2019)更新

### <a name="files"></a>文件 
在为文件、文件夹或其他 [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta&preserve-view=true) [创建共享链接](/graph/api/driveitem-createlink?view=graph-rest-beta&preserve-view=true)时，应用到期日期/时间或密码。

### <a name="identity-and-access"></a>标识和访问
- 使用 [新的应用程序权限](./permissions-reference.md#access-reviews-permissions) _AccessReview.ReadWrite.Membership_ 对 [访问权限审阅](/graph/api/resources/accessreviews-root?view=graph-rest-beta&preserve-view=true)执行 CRUD 操作。 
- 使用 [新的委派和应用程序权限](permissions-reference.md#administrative-units-permissions)、_AdministrativeUnit.Read.All_ 和 _AdministrativeUnit.ReadWrite.All_，以分别读取或写入（包括创建、更新、删除或管理成员身份）[管理单元](/graph/api/resources/administrativeunit?view=graph-rest-beta&preserve-view=true)资源。
- 使用 [新的委派和应用程序权限](permissions-reference.md#organization-permissions)、_Organization.Read.All_ 和 _Organization.ReadWrite.All_ 来访问 [组织](/graph/api/resources/organization?view=graph-rest-beta&preserve-view=true)和相关资源，例如 [订阅的 SKU](/graph/api/resources/subscribedsku?view=graph-rest-beta&preserve-view=true)。
- 使用新的 [discover](/graph/api/directorydefinition-discover?view=graph-rest-beta&preserve-view=true) 函数查找最新的目录[同步架构](/graph/api/resources/synchronization-synchronizationschema?view=graph-rest-beta&preserve-view=true)，以便将目录对象、属性及类型同步到应用。
- 使用[功能推出策略](/graph/api/resources/featureRolloutPolicy?view=graph-rest-beta&preserve-view=true)帮助租户管理员在为整个组织启用一些功能之前，针对特定组试用这些功能。

### <a name="mail"></a>邮件
使用更精确的应用程序权限 _Mail.ReadBasic.All_ 来读取用户邮箱（邮件正文除外）、预览正文、附件和扩展属性，不包括搜索邮箱。 现适用于 [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-beta&preserve-view=true) 以及针对 [邮件](/graph/api/resources/message?view=graph-rest-beta&preserve-view=true) 和 **mailFolder** 的 [更改跟踪](delta-query-overview.md)

### <a name="reports"></a>报告
- 获取与已删除的项目计数和大小相关的其他[邮箱使用情况数据](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-beta&preserve-view=true)。

### <a name="teamwork"></a>团队合作
- 为用户[安装](/graph/api/user-add-teamsappinstallation?view=graph-rest-beta&preserve-view=true)、[卸载](/graph/api/user-delete-teamsappinstallation?view=graph-rest-beta&preserve-view=true)、[升级](/graph/api/user-upgrade-teamsappinstallation?view=graph-rest-beta&preserve-view=true)和[列出已安装的 Microsoft Teams 应用](/graph/api/user-list-teamsappinstallation?view=graph-rest-beta&preserve-view=true)。
- 使用仅应用访问权限来读取频道消息、频道消息回复以及聊天中的消息。 [请求和批准](teams-protected-apis.md)此类访问。

## <a name="may---june-2019-new-and-generally-available"></a>2019 年 5 月 - 7 月：新版本和正式版

### <a name="calendar-mail-and-personal-contacts"></a>日历、邮件和个人联系人
Exchange 管理员可以向应用程序授予应用程序权限, 并[限制该应用仅访问邮箱 ](auth-limit-mailbox-access.md) 的子集, 而不是默认的访问组织中的所有邮箱。 此类受限访问适用于授予[日历](permissions-reference.md#calendars-permissions)、 [联系人](permissions-reference.md#contacts-permissions)及[邮件和邮箱设置](permissions-reference.md#mail-permissions)的应用的任何应用程序权限。 查看相关的[博客公告](https://developer.microsoft.com/graph/blogs/scoping-microsoft-graph-application-permissions-to-specific-exchange-online-mailboxes/)。

### <a name="mail"></a>邮件
使用[邮件搜索文件夹](/graph/api/resources/mailsearchfolder?view=graph-rest-1.0&preserve-view=true) API 来搜索邮件, 并访问 Outlook 电子邮件搜索结果。 查看相关的[博客公告](https://developer.microsoft.com/graph/blogs/mail-search-folder-support-for-microsoft-graph-apis/)。

### <a name="postman"></a>Postman
除 Graph 资源管理器外, 请在[Microsoft Graph Postman 集合](use-postman.md)中试用 Microsoft Graph API, 了解 API 行为并加速应用程序开发。

### <a name="tutorials"></a>教程
尝试使用新[教程构建 Java 控制台应用](/graph/tutorials/java) , 以获取有关用户日历的信息。

### <a name="user"></a>用户
管理员或用户可以[吊销](/graph/api/user-revokesigninsessions?view=graph-rest-1.0&preserve-view=true)用户的所有已颁发的刷新令牌。 通常用于防止已丢失或被盗设备上的应用访问组织的数据。


## <a name="may---june-2019-new-in-preview"></a>2019 年 5 月 - 7 月：预览版新增功能

> [!IMPORTANT]
> _预览_ 状态下的功能（包括 API 和工具）可能会发生更改，恕不另行通知，有些功能可能永远不会提升为 GA 状态。 请不要在成品应用中使用它们。

### <a name="devices-and-apps"></a>设备和应用
- Intune [5月](changelog.md#may-2019)更新 
- Intune [6月](changelog.md#june-2019)更新

### <a name="education"></a>教育
- [educationSchool](/graph/api/resources/educationschool?view=graph-rest-beta&preserve-view=true)的增量查询。
- [educationClass](/graph/api/resources/educationclass?view=graph-rest-beta&preserve-view=true) 和 [educationUser](/graph/api/resources/educationuser?view=graph-rest-beta&preserve-view=true)的增量查询和属性添加。 

### <a name="group"></a>Group
获取[敏感度标签](/graph/api/resources/assignedlabel?view=graph-rest-beta&preserve-view=true)，帮助保护 Microsoft 365 组的敏感数据并满足合规性策略。 这些标签是[assignedLabel](/graph/api/resources/assignedlabel?view=graph-rest-beta&preserve-view=true)对象，由 Microsoft 365 安全与合规性中心的管理员发布，作为 Microsoft 信息保护功能的一部分。 

### <a name="identity-and-access"></a>身份和访问控制
- 获取[应用程序](/graph/api/resources/applicationtemplate?view=graph-rest-beta&preserve-view=true)的实例，或将 Azure AD 应用程序库中的实例作为模板添加到目录中。
- 获取租户中所有[预配事件](/graph/api/resources/provisioningobjectsummary?view=graph-rest-beta&preserve-view=true)目录的列表。
- 获取有关 Azure AD 环境中[检测到的用户或登录风险](/graph/api/resources/riskdetection?view=graph-rest-beta&preserve-view=true)的信息。 此风险检测功能是 Azure AD 标识保护的一部分。

### <a name="mail"></a>邮件
使用更精确的代理权限 _Mail.ReadBasic_ 来读取用户邮箱（邮件正文除外）、预览正文、附件和扩展属性，不包括搜索邮箱。 可用于读取 [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-beta&preserve-view=true) 方法和更改 [message](/graph/api/resources/message?view=graph-rest-beta&preserve-view=true) 和 **mailFolder** 的 [跟踪](delta-query-overview.md)。

### <a name="microsoft-graph-toolkit"></a>Microsoft Graph 工具包
[Microsoft Graph 工具包](./toolkit/overview.md)是一组框架不可知的 web 组件和帮助器, 提供对 Microsoft Graph 中的数据进行身份验证和访问的便利。  由于 Microsoft Graph 工具包处于预览状态，请仅在非生产应用中使用工具包提供程序和组件。

### <a name="reports"></a>报告
- 获取组织中用户采用的[身份验证方法的报告](/graph/api/resources/authenticationmethods-usage-insights-overview?view=graph-rest-beta&preserve-view=true)，例如自助服务密码重置和多因素身份验证 (MFA).。

### <a name="sites"></a>网站
让用户[关注](/graph/api/site-follow?view=graph-rest-beta&preserve-view=true)或[取消关注](/graph/api/site-unfollow?view=graph-rest-beta&preserve-view=true) SharePoint 网站。

### <a name="teamwork"></a>团队合作
- 在 Microsoft 团队[聊天消息](/graph/api/resources/chatmessagehostedimage?view=graph-rest-beta&preserve-view=true)中存储[图像](/graph/api/resources/chatmessage?view=graph-rest-beta&preserve-view=true)。 
- 支持[配置](/graph/api/resources/teamdiscoverysettings?view=graph-rest-beta&preserve-view=true)私人团队的发现方式。


## <a name="january---april-2019-new-and-generally-available"></a>2019 年 1 月 - 4 月：新版本和正式版

[Microsoft Graph 数据连接](data-connect-concept-overview.md)

### <a name="calendar"></a>日历
[获取忙/闲日程安排](outlook-get-free-busy-schedule.md)

### <a name="identity-and-access"></a>身份和访问控制
[身份提供程序](/graph/api/resources/identityprovider?view=graph-rest-1.0&preserve-view=true)
[改进的身份验证指南](./auth/index.yml)
[将应用从 Azure AD Graph 迁移到 Microsoft Graph](migrate-azure-ad-graph-planning-checklist.md)

### <a name="sdks"></a>SDK
[SDK 指南](/sdks/sdks-overview.md) API 片段（[示例](/graph/api/user-get?view=graph-rest-1.0&preserve-view=true&tabs=cs#sdk-sample-code)）

### <a name="security"></a>安全性
[租户安全功能分数](/graph/api/resources/securescore?view=graph-rest-1.0&preserve-view=true)

## <a name="january---april-2019-new-in-preview"></a>2019 年 1 月 - 4 月：预览版中的新功能

### <a name="calendar-group-mail-to-do-tasks"></a>日历、群组、邮件、待办任务
[获取事件、消息、Outlook 任务或组帖子中文件或项目附件的原始/MIME 内容](/graph/api/attachment-get?view=graph-rest-beta&preserve-view=true#get-the-raw-contents-of-a-file-or-item-attachment)

### <a name="change-notifications"></a>更改通知
[减少缺失更改通知](webhooks-lifecycle.md)

### <a name="devices-and-apps"></a>设备和应用
- Intune [1 月](changelog.md#january-2019)更新 
- Intune [2 月](changelog.md#february-2019)更新
- Intune [3 月](changelog.md#march-2019)更新
- Intune [4 月](changelog.md#april-2019)更新

### <a name="files"></a>文件
[共享邀请](/graph/api/driveitem-invite?view=graph-rest-beta&preserve-view=true)包含过期时间和密码

### <a name="financials"></a>财务
[Dynamics 365 Business Central](dynamics-business-central-concept-overview.md)

### <a name="identity-and-access"></a>身份和访问控制
[访问评审](/graph/api/resources/accessreviews-root?view=graph-rest-beta&preserve-view=true)支持应用程序权限[审核和登录日志](/graph/api/resources/azure-ad-auditlog-overview?view=graph-rest-beta&preserve-view=true)
[Azure AD B2C 中的自定义注册和登录](/graph/api/resources/trustframeworkpolicy?view=graph-rest-beta&preserve-view=true)
[存在风险的用户](/graph/api/resources/riskyuser?view=graph-rest-beta&preserve-view=true)和[历史记录](/graph/api/resources/riskyuserhistoryitem?view=graph-rest-beta&preserve-view=true)

### <a name="mail"></a>邮件
[获取消息的 MIME 内容](outlook-get-mime-message.md)

### <a name="reports"></a>报表
[应用程序登录报表](/graph/api/resources/applicationsigninsummary?view=graph-rest-beta&preserve-view=true)

### <a name="security"></a>安全性
[安全操作](/graph/api/resources/securityaction?view=graph-rest-beta&preserve-view=true)
[威胁指示器](/graph/api/resources/tiindicator?view=graph-rest-beta&preserve-view=true)

### <a name="teamwork"></a>团队合作
[一对一聊天](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true)
[排班管理](/graph/api/resources/shift?view=graph-rest-beta&preserve-view=true)

## <a name="see-also"></a>另请参阅
- 请参阅 Microsoft Graph 中的[新增功能](whats-new-overview.md)。
- 定期查看 [Microsoft Graph 开发人员博客](https://developer.microsoft.com/graph/blogs/), 了解发布公告和有帮助的资源。 
- 浏览 Microsoft Graph API 新增功能的详细信息, 以及[changelog](changelog.md)中的 API 行为更新。