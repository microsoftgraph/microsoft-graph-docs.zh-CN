---
title: Microsoft Graph 新增功能
description: Microsoft Graph 新增功能
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 1c4629b8fcfca5168a1e752a984f3e77e1018dd0
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547667"
---
# <a name="whats-new-in-microsoft-graph"></a>Microsoft Graph 新增功能

查看 Microsoft Graph 中的最近两个月新增功能要点、[以前增加的内容](whats-new-earlier.md)以及如何[分享你的想法](#want-to-stay-in-the-loop)。 有关 API 级更新的详细列表，请参见 [API更改日志](https://developer.microsoft.com/graph/changelog/)。 

> [!IMPORTANT]
> 处于 _预览_ 状态的功能（包括 API 和工具）可能会发生更改，恕不另行通知，有些功能可能永远不会提升为正式发布 (GA) 状态。不要在生产应用中使用预览功能。

## <a name="may-2021-new-and-generally-available"></a>2021 年 5 月：新版本和正式发布版本

### <a name="devices-and-apps--cloud-printing"></a>设备和应用 | 云打印
使用 [打印机](/graph/api/resources/printer)的 **lastSeenDateTime** 属性，查找打印机上次与“通用打印”交互的时间。

### <a name="identity-and-access--identity-and-sign-in"></a>身份和访问 | 身份和登录
使用 [authorizationPolicy](/graph/api/resources/authorizationpolicy) 的 **guestUserRoleId** 属性，获取或更新来宾用户的角色。

### <a name="reports--azure-ad-activity-reports"></a>报告 | Azure AD 活动报告
Azure AD 预配服务和其相关属性执行的向[列表](/graph/api/provisioningobjectsummary-list)报告 API 操作的正式发布。 将 API 之前的 Beta 版本与 v1.0 版本对齐。 

## <a name="may-2021-new-in-preview-only"></a>2021 年 5 月：仅限预览版新增功能

### <a name="devices-and-apps--cloud-pc"></a>设备和应用 | 云电脑
请求最小特权应用程序权限`CloudPC.Read.All`或`CloudPC.ReadWrite.All`以下资源的访问方法：
  - 读写操作和 [cloudPC](/graph/api/resources/cloudpc?view=graph-rest-beta&preserve-view=true) 的 [reprovision](/graph/api/cloudpc-reprovision?view=graph-rest-beta&preserve-view=true) 方法。
  - 读写操作和 [cloudPcDeviceImage](/graph/api/resources/cloudpcdeviceimage?view=graph-rest-beta&preserve-view=true) 的 [getSourceImages](/graph/api/cloudpcdeviceimage-getsourceimages?view=graph-rest-beta&preserve-view=true) 方法。
  - 读写操作和 [cloudPcOnPremisesConnection](/graph/api/resources/cloudpconpremisesconnection?view=graph-rest-beta&preserve-view=true) 的 [updateAdDomainPassword](/graph/api/cloudpconpremisesconnection-updateaddomainpassword?view=graph-rest-beta&preserve-view=true) 方法。
  - 读写操作和 [cloudPcProvisioningPolicy](/graph/api/resources/cloudpcprovisioningpolicy?view=graph-rest-beta&preserve-view=true) 的[分配](/graph/api/cloudpcprovisioningpolicy-assign?view=graph-rest-beta&preserve-view=true)方法。

### <a name="education"></a>教育版
[设置 SharePoint 资源文件夹](/graph/api/educationsubmission-setupresourcesfolder?view=graph-rest-beta&preserve-view=true)，[educationSubmission](/graph/api/resources/educationsubmission?view=graph-rest-beta&preserve-view=true) 的所有基于文件的资源（如 Word 或 Excel 文件）应上传到该文件夹。

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