---
title: Microsoft Graph 新增功能
description: Microsoft Graph 新增功能
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 21bad04b4fceeecc1eddd18fbae1a1a20b50e50a
ms.sourcegitcommit: a1a57e803c334e11316dd571ad1b54c95406740e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/29/2020
ms.locfileid: "44413432"
---
# <a name="whats-new-in-microsoft-graph"></a>Microsoft Graph 新增功能

查看 Microsoft Graph 中的新增功能要点，并查看你可如何[分享你的想法](#want-to-stay-in-the-loop)。 有关 API 更新的完整列表，请参阅 API 更改日志的 "[可能](changelog.md#may-2020)" 和 "[四月](changelog.md#april-2020)" 部分。 

> [!IMPORTANT]
> _预览_状态下的功能（包括 API 和工具）可能会发生更改，恕不另行通知，有些功能可能永远不会提升为正式发布 (GA) 状态。 不要在成品应用中使用预览功能。

## <a name="may-2020-new-and-generally-available"></a>5月2020：新的和普遍可用的

### <a name="calendar--place"></a>日历 | 位置
在 v1.0 中的[位置 API](/graph/api/resources/place) GA-在生产应用程序中使用此 api 来获取、更新或删除租户中的[会议室](/graph/api/resources/room)或[会议室列表](/graph/api/resources/roomlist)。 了解有关位置 API 的[详细](outlook-calendar-concept-overview.md#build-apps-with-location-awareness-and-provide-intelligent-context)信息。

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理
Intune[可能会](changelog.md#may-2020)在 v1.0 中更新。

### <a name="graph-explorer"></a>Graph 浏览器
使用[Graph 浏览器](https://developer.microsoft.com/en-us/graph/graph-explorer)的许多新功能，以增强沙盒中的学习和原型。 例如：
- 查看与您输入的 REST API 查询相对应的代码段，以 c #、Java、JavaScript 和客观 C 为依据。
- 使用租户登录，查看并将访问令牌复制到您喜爱的 REST 客户端应用程序。

有关更多详细信息，请参阅[新的 Graph 浏览器现已公开](https://developer.microsoft.com/graph/blogs/new-graph-explorer-is-now-ga/)。

### <a name="identity-and-access"></a>身份和访问
- V1.0 中的 [服务主体 API] GA-在生产应用程序中使用[servicePrincipals](/graph/api/resources/serviceprincipal?view=graph-rest-1.0)以编程方式管理应用程序的实例，并控制应用程序可在租户中执行的操作。 您可以控制哪些用户可以使用应用程序，应用程序有权访问哪些资源，如添加密码凭据、即将过期的证书以及管理委派的权限授予和应用程序角色分配。
- 公开的[appRoleAssignment](/graph/api/resources/appRoleAssignment?view=graph-rest-1.0) API，用于记录[appRole](/graph/api/resources/approle?view=graph-rest-1.0) `roles` 对[用户](/graph/api/resources/user?view=graph-rest-1.0)、[组](/graph/api/resources/group?view=graph-rest-1.0)或[servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-1.0)的 appRole 分配（表示 ID 令牌和访问令牌中的声明）。
- 使用的委派或应用程序权限 `AppRoleAssignment.ReadWrite.All` 允许应用管理对任何 API （包括 Microsoft Graph）的应用程序权限和任何应用程序的应用程序分配的授予，分别与或不带登录用户。


### <a name="microsoft-graph-sdks"></a>Microsoft Graph SDK
有关以下内容，请参阅新的 SDK 指导：
- [分页](/graph/sdks/paging)
- [批处理](/graph/sdks/batch-requests)
- [在 OneDrive 上上传大文件](/graph/sdks/large-file-upload)
- [通过 HTTP 中间件组件自定义 SDK 服务客户端](/graph/sdks/customize-client)。

### <a name="teamwork"></a>团队合作
- 如果您的方案涉及团队中的联机会议，请参阅有关如何在[日历 API](outlook-calendar-online-meetings.md)和[云通信 API](cloud-communications-online-meetings.md)中进行[选择](choose-online-meeting-api.md)以创建和加入联机会议的新指导。
- [发送](/graph/api/channel-post-messages?view=graph-rest-1.0)和[回复](/graph/api/channel-post-messagereply?view=graph-rest-1.0)[频道](/graph/api/resources/channel?view=graph-rest-1.0)中的邮件。
- 通过使用**fileFolder**导航属性，获取[频道](/graph/api/resources/channel?view=graph-rest-1.0)的文件的 OneDrive for business 位置。

### <a name="teamwork--shifts"></a>团队合作 | 倒班
V1.0 中的[倒班 API](/graph/api/resources/shift?view=graph-rest-1.0) GA-在生产应用程序中使用此 api 创建、更新和管理 firstline 工作人员的日程安排，以让他们保持联系并有效地进行协作。


## <a name="may-2020-new-in-preview-only"></a>5月2020：仅预览中的新内容

### <a name="devices-and-apps--cloud-printing"></a>设备和应用 | 云打印
- [打印机](/graph/api/resources/printer?view=graph-rest-beta)和[printerShare](/graph/api/resources/printershare?view=graph-rest-beta)资源现在处于奇偶校验，并且彼此具有相同的属性。
- 打印机共享的一些属性和类型名称清理：
  - 使用 "[打印](/graph/api/resources/print?view=graph-rest-beta)" 的**共享**导航属性获取在租户中注册的打印机共享的列表。 
  - 请参阅[可能](changelog.md#may-2020)更改日志中的详细信息。

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理
Intune[可能会](changelog.md#may-2020)在 beta 中更新。

### <a name="groups"></a>组
- 使用[组](/graph/api/resources/group?view=graph-rest-beta)的现有规则或指定的规则[评估](/graph/api/group-evaluatedynamicmembership?view=graph-rest-beta)用户或设备是否为动态组的成员。 [基于规则的动态成员身份](/azure/active-directory/users-groups-roles/groups-dynamic-membership)可降低添加和删除成员的管理开销。
- 创建 Office 365[组](/graph/api/resources/group?view=graph-rest-beta)时，通过在**resourceBehaviorOptions**属性中指定组的行为来配置这些行为。 例如，允许成员张贴、订阅新成员到对话、禁用欢迎电子邮件以及在 Outlook 体验中隐藏组。
- 指定要在**resourceProvisioningOptions**属性中设置的资源，这些资源通常不是默认[组](/graph/api/resources/group?view=graph-rest-beta)创建的一部分。 目前支持将组设置为具有 Microsoft 团队功能的[团队](/graph/api/resources/team?view=graph-rest-beta)。

### <a name="identity-and-access"></a>身份和访问
- `$count` `$filter` `$search` 在获取派生自[directoryObject]()的实体的集合时应用 OData 系统查询选项（，，）。 您可以在这些实体的**displayName**和**description**属性中[搜索特定令牌](/graph/query-parameters?#using-search-on-directory-object-collections)，并使用 OData 强制转换将**directoryObject**结果修整为特定的派生类型。 有关[使用 $count、$filter、$search 和 $orderby 在 Microsoft Graph 中生成高级查询](https://developer.microsoft.com/en-us/graph/blogs/build-advanced-queries-with-count-filter-search-and-orderby/)的更多详细信息，请参阅。
- 作为[标识保护 API](/graph/api/resources/identityprotection-root?view=graph-rest-beta)的一部分，使用**riskEventType**属性来[获取检测到的风险类型](/graph/api/riskdetection-get?view=graph-rest-beta)，或[获取用户历史记录中的风险类型](/graph/api/riskyuser-list-history?view=graph-rest-beta)。 请勿使用**riskType**属性，因为它已被弃用。
- 在[条件访问策略](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta)的[条件集](/graph/api/resources/conditionalaccessconditionset?view=graph-rest-beta)的**clientAppTypes**属性中指定客户端应用程序类型。
- 使用委派的权限 `EntitlementManagement.Read.All` ，以允许应用代表登录用户读取访问包和相关的权限管理资源。

### <a name="teamwork"></a>团队合作
- [支持单一登录（SSO）](/microsoftteams/platform/tabs/how-to/authentication/auth-aad-sso)的团队应用可以 `WebApplicationInfo.id` 在[teamsAppDefinition](/graph/api/resources/teamsappdefinition?view=graph-rest-beta)的**azureADAppId**属性中指定团队应用程序清单中的。
- 使用[更](/graph/permissions-reference#teams-resource-specific-consent-permissions)精细的权限访问[团队](/graph/api/resources/team?view=graph-rest-beta)和[频道](/graph/api/resources/channel?view=graph-rest-beta)资源。


## <a name="april-2020-new-and-generally-available"></a>2020 年 4 月：新版本和正式版

### <a name="calendar"></a>日历
- 采用编程方式[共享或委派日历](outlook-share-or-delegate-calendar.md)，与 Outlook 用户体验的奇偶校验更加接近。 除了跟踪日历的当前用户权限和共享状态之外：
  - 对于每个[日历](/graph/api/resources/calendar?view=graph-rest-1.0)，你现在可以管理与之共享日历的每个用户的[权限](/graph/api/resources/calendarpermission?view=graph-rest-1.0)。 
  - 对于每个[邮箱](/graph/api/resources/mailboxsettings?view=graph-rest-1.0)，你现在可以指定代理人、邮箱所有者，还是两者同时接收会议邮件和会议响应。 
- [创建事件并作为联机会议更新](outlook-calendar-online-meetings.md)：
  - 对于每个**日历**，指定允许的和默认的在线会议提供程序。
  - 创建或更新[事件](/graph/api/resources/event?view=graph-rest-1.0)以使其在线可用，并提供详细信息供与会者加入在线会议。 
  - 具体来说，使用**事件**的新 **onlineMeetingProvider** 和 **onlineMeeting** 属性来将 Microsoft Teams 设置或标识为在线会议提供程序，这是 **onlineMeetingUrl** 属性的[已知问题](known-issues.md#onlinemeetingurl-property-support-for-microsoft-teams)的解决方法。
- 将[高达 150MB 的文件附件](outlook-large-attachments.md)添加到[event](/graph/api/resources/event?view=graph-rest-1.0)。

### <a name="files"></a>文件
- [签出](/graph/api/driveitem-checkout?view=graph-rest-1.0)或[签入](/graph/api/driveitem-checkin?view=graph-rest-1.0)文件到 OneDrive，以管理更新文件并在更新就绪后向其他人提供更新。
- 将可选密码和到期日期/时间应用为[邀请](/graph/api/driveitem-invite?view=graph-rest-1.0)的参数，并[创建共享链接](/graph/api/driveitem-createlink?view=graph-rest-1.0)操作以共享[driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0)。
- 获取或设置[权限](/graph/api/resources/permission?view=graph-rest-1.0)的密码和到期日期/时间，并跟踪已授予其共享**driveItem**权限的用户的[了解 identityset](/graph/api/resources/identityset?view=graph-rest-1.0) 。
- 使用**权限**导航属性获取[共享驱动器项](/graph/api/resources/shareddriveitem?view=graph-rest-1.0)的[权限](/graph/api/resources/permission?view=graph-rest-1.0)。
- 将仅具有[共享链接](/graph/api/resources/sharinglink?view=graph-rest-1.0)的用户限制为仅查看，并且可能不会在 OneDrive for Business 或 SharePoint 上下载共享**driveItem**的内容。

### <a name="identity-and-access"></a>身份和访问
- 若要在基于角色的访问控制（RBAC）提供程序中管理角色并分配资源访问权限，请使用 [unifiedRoleAssignmentMultiple](/graph/api/resources/unifiedroleassignmentmultiple?view=graph-rest-1.0)。 **unifiedRoleAssignmentMultiple** 资源支持在一系列作用域中定义单个角色，并将该角色分配给多个主体（例如用户）。
- 使用 `/policies` URL 段并指定策略类型，访问[组织的特定类型的策略](/graph/api/resources/policy-overview?view=graph-rest-1.0)。 例如，组织可以强制实施 Web 会话在一段时间不活动后自动从该会话注销用户的策略；请参阅 [activityBasedTimeoutPolicy](/graph/api/resources/activitybasedtimeoutpolicy?view=graph-rest-1.0) 的实例的 CRUD 操作。 这是一项[重大更改](https://developer.microsoft.com/identity/blogs/breaking-changes-policy-api-microsoft-graph-1.0/)，可以通过对 `/policies` 段下所有类型的策略进行分组，以便更易于发现所有策略。 采用类似的方法访问其他类型的策略：[claimsMappingPolicy](/graph/api/resources/claimsmappingpolicy?view=graph-rest-1.0)、[homeRealmDiscoveryPolicy](/graph/api/resources/homerealmdiscoverypolicy?view=graph-rest-1.0)、[tokenLifetimePolicy](/graph/api/resources/tokenlifetimepolicy?view=graph-rest-1.0) 和 [tokenIssuancePolicy](/graph/api/resources/tokenissuancetimepolicy?view=graph-rest-1.0)。 

### <a name="mail"></a>邮件
向 [message](/graph/api/resources/message?view=graph-rest-1.0) 添加了[高达 150MB 的文件附件](outlook-large-attachments.md)。

### <a name="sites-and-lists"></a>站点和列表
- [列出站点](/graph/api/sites-list-followed?view=graph-rest-1.0)，这些站点时已登录用户关注的。
- 使用**dataLocationCode**属性标识[网站集](/graph/api/resources/sitecollection?view=graph-rest-1.0)的地理区域。
- 通过访问作为[driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0)的**SharepointIds**一部分的**tenantId**属性，标识 SharePoint 上的文件、文件夹或其他项的租户。

## <a name="april-2020-new-in-preview-only"></a>2020 年 4 月：仅限预览版中的新增功能

### <a name="devices-and-apps--cloud-printing"></a>设备和应用 | 云打印

将允许的用户和组指定为在通用打印（Microsoft 365 基于云的打印基础结构）上使用特定的[打印机共享](/graph/api/resources/printershare?view=graph-rest-beta)。 若要体验可靠且集中的打印管理功能，并为打印用户提供简单而丰富安全的打印体验，请参阅[通用打印公告](https://techcommunity.microsoft.com/t5/windows-it-pro-blog/announcing-universal-print-a-cloud-based-print-solution/ba-p/1204775)并加入其预览计划。

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理
Intune [4 月](changelog.md#april-2020)更新。

### <a name="groups"></a>组
通过组的应用 ID 识别创建[组](/graph/api/resources/group?view=graph-rest-beta)的应用。

### <a name="identity-and-access"></a>身份和访问
- [管理单元](/graph/api/resources/administrativeunit?view=graph-rest-beta)[跟踪更改](/graph/api/administrativeunit-delta?view=graph-rest-beta)。
- [oAuth2PermissionGrant](/graph/api/resources/oauth2permissiongrant?view=graph-rest-beta)[跟踪更改](/graph/api/oauth2permissiongrant-delta?view=graph-rest-beta)。
- [管理](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta)用户的[身份验证方法](/graph/api/resources/authenticationmethod?view=graph-rest-beta)，其中包括[密码](/graph/api/resources/passwordauthenticationmethod?view=graph-rest-beta)或[电话](/graph/api/resources/phoneauthenticationmethod?view=graph-rest-beta)。 例如，[重置用户密码](/graph/api/passwordauthenticationmethod-resetpassword?view=graph-rest-beta)并[获取重置状态](/graph/api/authenticationoperation-get?view=graph-rest-beta)，或者为用户[添加电话号码](/graph/api/authentication-post-phonemethods?view=graph-rest-beta)以进行短信或语音通话身份验证（如果策略为用户启用）。

### <a name="reports--identity-and-access-reports"></a>报告 | 身份和访问报告
[列出](/graph/api/relyingpartydetailedsummary-list?view=graph-rest-beta) Active Directory 联合身份验证服务中配置的[依赖方](https://docs.microsoft.com/windows-server/identity/ad-fs/technical-reference/understanding-key-ad-fs-concepts)。

### <a name="reports--office-365-usage-reports"></a>报告 | Office 365 使用率报告
查看 CSV 报告中的**会议创建**和**会议互动**数据，以查看[电子邮件活动计数](/graph/api/reportroot-getemailactivitycounts?view=graph-rest-beta)、[电子邮件活动用户计数](/graph/api/reportroot-getemailactivityusercounts?view=graph-rest-beta)和[电子邮件活动用户详细信息](/graph/api/reportroot-getemailactivityuserdetail?view=graph-rest-beta)。


## <a name="want-to-stay-in-the-loop"></a>保持循环

我们可以通过以下方式进行参与：

- 是否有希望 Microsoft Graph 支持的方案？ 在 [Microsoft Graph 用户心声](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)中建议新功能并进行投票。
    某些新功能来源于开发人员社区的热门请求。 Microsoft Graph 团队会定期评估客户需求，并按以下顺序发布新功能：

    1. 处于**_预览_** 状态的 Debut。 任何相关的 REST API 更新都在 beta 终结点 (`https://graph.microsoft.com/beta`) 中。  

    2. 如果有足够的反馈表明具有可行性，则提升为 **_正式发布_ (GA)** 状态。 任何相关的 REST API 更新都添加到 v1.0 终结点 (`https://graph.microsoft.com/v1.0`)。 
- 成为 Microsoft Graph 社区中的活跃成员! [参与](https://aka.ms/microsoftgraphcall)Microsoft Graph 社区每月通话。
- 注册 [office 365 开发人员计划](https://developer.microsoft.com/office/dev-program)，免费订阅 Office 365, 然后开始开发! 


## <a name="see-also"></a>另请参阅
- 定期查看 [Microsoft Graph 开发人员博客](https://developer.microsoft.com/graph/blogs/), 了解发布公告和有帮助的资源。 
- 浏览 Microsoft Graph API 新增功能的详细信息, 以及[changelog](changelog.md)中的 API 行为更新。
- 查找[早期版本的重点内容](whats-new-earlier.md)。
- 了解有关 [Microsoft Graph 的版本控制、支持和中断性变更策略](versioning-and-support.md)。

