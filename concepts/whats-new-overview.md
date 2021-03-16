---
title: Microsoft Graph 新增功能
description: Microsoft Graph 新增功能
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 7cbe064bb6e253d7e3c05648d0d531020cffb4b6
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761749"
---
# <a name="whats-new-in-microsoft-graph"></a>Microsoft Graph 新增功能

查看 Microsoft Graph 中的最近两个月新增功能要点、[以前增加的内容](whats-new-earlier.md)以及如何[分享你的想法](#want-to-stay-in-the-loop)。 有关 API 级更新的详细列表，请参见 [API更改日志](https://developer.microsoft.com/graph/changelog/)。 

> [!IMPORTANT]
> _预览_ 状态下的功能（包括 API 和工具）可能会发生更改，恕不另行通知，有些功能可能永远不会提升为正式发布 (GA) 状态。 不要在成品应用中使用预览功能。

## <a name="march-2021-new-and-generally-available"></a>2021 年 3 月: 新版本和正式版

### <a name="applications"></a>应用程序
支持在 Azure AD 应用程序库中 [列出](/graph/api/applicationtemplate-list) 应用程序，并将此类应用程序的实例 [添加](/graph/api/applicationtemplate-instantiate) 到目录中的 [applicationTemplate](/graph/api/resources/applicationtemplate) 资源的 GA。

### <a name="devices-and-apps--cloud-printing"></a>设备和应用 | 云打印
适用于通用打印的 [云打印](universal-print-concept-overview.md) GA! 查看 [公告](https://techcommunity.microsoft.com/t5/windows-it-pro-blog/universal-print-is-ready-for-business/ba-p/2176778)，并查看如何 [开始使用通用打印](https://docs.microsoft.com/universal-print/fundamentals/universal-print-license)。

### <a name="teamwork"></a>团队合作
- 代表了 Microsoft Teams 应用目录中应用版本细节的[teamsAppDefinition](/graph/api/resources/teamsAppDefinition) GA 的一些更多属性，其中包括:
  - **createdBy**、**描述**、**shortDescription**、**lastModifiedDateTime**
  - **publishingState**，可以是`submitted`中之一和由管理员发布的正在审核、`published`、或`rejected` 中的状态
  - [teamworkBot](/graph/api/resources/teamworkbot) 类型的 **机器人** 关系，表示 Teams 应用清单中指定的机器人的详细信息。
- [列表](/graph/api/chatmessage-list-chatmessagehostedcontents) 或 [获取](/graph/api/chatmessagehostedcontent-get) [chatMessage](/graph/api/resources/chatmessage) 中的丰富内容，如图片或代码片段。

## <a name="march-2021-new-in-preview-only"></a>2021 年 3 月：仅限预览版中的新增功能

### <a name="devices-and-apps--cloud-printing"></a>设备和应用 | 云打印
当打印机与通用打印交互时，获取最近日期/时间 (**lastSeenDateTime** 属性)。

### <a name="sites-and-lists"></a>网站和列表
- 通过 [contentType](/graph/api/resources/contentType?view=graph-rest-beta&preserve-view=true) 实体上的一组新属性和方法，支持特定站点集合中文档或文档集的特定内容类型或模板。 方法包括下列几种:
  - [addCopy](/graph/api/contenttype-addcopy?view=graph-rest-beta&preserve-view=true)
  - [associateWithHubSites](/graph/api/contenttype-associatewithhubsites?view=graph-rest-beta&preserve-view=true)
  - [copyToDefaultContentLocation](/graph/api/contenttype-copytodefaultcontentlocation?view=graph-rest-beta&preserve-view=true)
  - [isPublished](/graph/api/contenttype-ispublished?view=graph-rest-beta&preserve-view=true)
  - [发布](/graph/api/contenttype-publish?view=graph-rest-beta&preserve-view=true)
  - [取消发布](/graph/api/contenttype-unpublish?view=graph-rest-beta&preserve-view=true)
- 按其列标签自定义内容类型。 列由 [columnDefinition](/graph/api/resources/columndefinition?view=graph-rest-beta&preserve-view=true) 实体表示，并支持全套的 CRUD 操作。
- [获取可应用于列表上网站的内容类型](/graph/api/site-getApplicableContentTypesForList?view=graph-rest-beta&preserve-view=true)。
- 按 **columnDefinition** 实体中的下列属性来区分列类型: 布尔型、计算型、选择型、货币型、日期时间型、查找型、数字型、人或组型、文本型。 这些属性是相互排斥的。

### <a name="users"></a>用户
[通过](/graph/api/regionalandlanguagesettings-get?view=graph-rest-beta&preserve-view=true) 或 [更新](/graph/api/regionalandlanguagesettings-update?view=graph-rest-beta&preserve-view=true) 用户 [对翻译语言的偏好](/graph/api/resources/translationpreferences?view=graph-rest-beta&preserve-view=true)。 例如，是否翻译、自动翻译、或在翻译消息、聊天和网页中的特定语言之前提示，以及进行任何 [翻译覆盖](/graph/api/resources/translationlanguageoverride?view=graph-rest-beta&preserve-view=true)。

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
使用 [educationAssignmentDefaults](/graph/api/resources/educationAssignmentDefaults?view=graph-rest-beta&preserve-view=true) 来指定课堂作业的默认操作，例如，作业到期时间、作业通知的频道 URL。 仍然可以在创建任务时自定义值。

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



## <a name="want-to-stay-in-the-loop"></a>保持循环

我们可以通过以下方式进行参与：

- 是否有希望 Microsoft Graph 支持的方案？ 在 [Microsoft Graph 用户心声](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)中建议新功能并进行投票。
    某些新功能来源于开发人员社区的热门请求。 Microsoft Graph 团队会定期评估客户需求，并按以下顺序发布新功能：

    1. 处于 **_预览_** 状态的 Debut。 任何相关的 REST API 更新都在 beta 终结点 (`https://graph.microsoft.com/beta`) 中。  

    2. 如果有足够的反馈表明具有可行性，则提升为 **_正式发布_ (GA)** 状态。 任何相关的 REST API 更新都添加到 v1.0 终结点 (`https://graph.microsoft.com/v1.0`)。 
- 成为 Microsoft Graph 社区中的活跃成员! [参与](https://aka.ms/microsoftgraphcall)Microsoft Graph 社区每月通话。
- 注册 [Microsoft 365 开发人员计划](https://developer.microsoft.com/office/dev-program)，免费订阅 Microsoft 365, 然后开始开发! 


## <a name="see-also"></a>另请参阅
- 定期查看 [Microsoft Graph 开发人员博客](https://developer.microsoft.com/graph/blogs/), 了解发布公告和有帮助的资源。 
- 浏览 Microsoft Graph API 新增功能的详细信息, 以及[changelog](https://developer.microsoft.com/graph/changelog/)中的 API 行为更新。
- 查找[早期版本的重点内容](whats-new-earlier.md)。
- 了解有关 [Microsoft Graph 的版本控制、支持和中断性变更策略](versioning-and-support.md)。
