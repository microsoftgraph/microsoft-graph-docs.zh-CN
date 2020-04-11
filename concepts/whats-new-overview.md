---
title: Microsoft Graph 新增功能
description: Microsoft Graph 新增功能
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 0742ac1f35e10cfbed09ca164d4cb2af6a1c8484
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229365"
---
# <a name="whats-new-in-microsoft-graph"></a>Microsoft Graph 新增功能

查看 Microsoft Graph 中的新增功能要点，并查看你可如何[分享你的想法](#want-to-stay-in-the-loop)。 有关 API 更新的完整列表，请参阅 API 更改日志的 [4 月](changelog.md#april-2020)和 [3 月](changelog.md#march-2020)部分。 

> [!IMPORTANT]
> _预览_状态下的功能（包括 API 和工具）可能会发生更改，恕不另行通知，有些功能可能永远不会提升为正式发布 (GA) 状态。 不要在成品应用中使用预览功能。

## <a name="april-2020-new-and-generally-available"></a>2020 年 4 月：新版本和正式版

### <a name="calendar"></a>日历
- 采用编程方式[共享或委派日历](outlook-share-or-delegate-calendar.md)，与 Outlook 用户体验的奇偶校验更加接近。 除了跟踪日历的当前用户权限和共享状态之外：
  - 对于每个[日历](/graph/api/resources/calendar?view=graph-rest-1.0)，你现在可以管理与之共享日历的每个用户的[权限](/graph/api/resources/calendarpermission?view=graph-rest-1.0)。 
  - 对于每个[邮箱](/graph/api/resources/mailboxsettings?view=graph-rest-1.0)，你现在可以指定代理人、邮箱所有者，还是两者同时接收会议邮件和会议响应。 
- [创建事件并作为联机会议更新](outlook-calendar-online-meetings.md)：
  - 对于每个**日历**，指定允许的和默认的在线会议提供程序。
  - 创建或更新[事件](/graph/api/resources/event?view=graph-rest-1.0)以使其在线可用，并提供详细信息供与会者加入在线会议。 
  - 具体来说，使用**事件**的新 **onlineMeetingProvider** 和 **onlineMeeting** 属性来将 Microsoft Teams 设置或标识为在线会议提供程序，这是 **onlineMeetingUrl** 属性的[已知问题](known-issues.md#onlinemeetingurl-property-support-for-microsoft-teams)的解决方法。

## <a name="april-2020-new-in-preview-only"></a>2020 年 4 月：仅限预览版中的新增功能

### <a name="identity-and-access"></a>身份和访问
若要在基于角色的访问控制（RBAC）提供程序中管理角色并分配资源访问权限，请使用 [unifiedRoleAssignmentMultiple](/graph/api/resources/unifiedroleassignmentmultiple?view=graph-rest-beta)。 **unifiedRoleAssignmentMultiple** 资源支持在一系列作用域中定义单个角色，并将该角色分配给多个主体（例如用户）。 


## <a name="march-2020-new-and-generally-available"></a>2020 年 3 月：新版本和正式版

### <a name="cloud-communications"></a>云通信
- 获取呼叫路由和[呼叫](/graph/api/resources/call?view=graph-rest-1.0)的传入上下文。
- 对呼叫进行[录制状态更新](/graph/api/call-updaterecordingstatus?view=graph-rest-1.0)。
- 可为[参与者](/graph/api/resources/participant?view=graph-rest-1.0)指定录制信息，包括录制的发起人和状态。
- 使用 **callChainId** 属性唯一标识会议或参与者到参与者[呼叫](/graph/api/resources/call?view=graph-rest-1.0)中的参与者。
- 可将参与者的国家/地区代码和终结点类型（例如 Skype for Business 或 Skype for Business VOIP）标识为 [participantInfo](/graph/api/resources/participantinfo?view=graph-rest-1.0) 的组成部分。
- 第三方视频电话会议 (VTC) 设备合作伙伴可以通过云视频互操作 (CVI) 机器人和 [logTeleconferenceDeviceQuality](/graph/api/call-logteleconferencedevicequality?view=graph-rest-1.0) 函数，记录并提供视频电话会议设备的媒体质量数据。 媒体质量数据包括，[音频](/graph/api/resources/teleconferencedeviceaudioquality?view=graph-rest-1.0)、[视频](/graph/api/resources/teleconferencedevicevideoquality?view=graph-rest-1.0)和[屏幕共享](/graph/api/resources/teleconferencedevicescreensharingquality?view=graph-rest-1.0)的开放类型数据。

### <a name="files"></a>文件
- 与用户共享、添加至用户 OneDrive、或作为搜索结果返回的[远程项](/graph/api/resources/remoteitem?view=graph-rest-1.0)，包含图像或视频的元数据。
- [关注](/graph/api/driveitem-follow?view=graph-rest-1.0) [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0)，以便能够便捷访问或方便执行移动、复制和另存为等操作。 使用[取消关注](/graph/api/driveitem-unfollow?view=graph-rest-1.0)可停止关注驱动器项。
- 向用户[授予](/graph/api/permission-grant?view=graph-rest-1.0)访问共享链接的权限，以便共享相应的驱动器项。

### <a name="identity-and-access"></a>身份和访问
- [组织联系人](/graph/api/resources/orgcontact?view=graph-rest-1.0)[跟踪更改](/graph/api/orgcontact-delta?view=graph-rest-1.0)。
- 使用 **riskEventTypes_v2** 属性可获取与[登录](/graph/api/resources/signin?view=graph-rest-1.0)相关的风险事件类型。
- 使用 `User.ManageIdentities.All` 委托的权限，可允许应用读取、更新或删除与登录用户有权访问的用户帐户关联的标识。 在没有登录用户的情况下，在应用程序级别使用此权限。 这样，应用可以[管理](/graph/api/user-update?view=graph-rest-1.0)用户能够使用哪些标识来登录。

### <a name="reports"></a>报告
将 Teams 服务管理员和 Teams 通信管理员用作接受的用户角色，允许应用代表用户以[用户委派的授权的形式](reportroot-authorization.md)读取 Office 365 服务使用情况报告。 

### <a name="sites"></a>网站
- 让用户[关注](/graph/api/site-follow?view=graph-rest-1.0)或[取消关注](/graph/api/site-unfollow?view=graph-rest-1.0) SharePoint 网站。
- 针对 SharePoint [列表](/graph/api/resources/list?view=graph-rest-1.0)[订阅更改通知](/graph/api/resources/subscription?view=graph-rest-1.0)。 

## <a name="march-2020-new-in-preview-only"></a>2020 年 3 月：仅限预览版中的新增功能

### <a name="calendar"></a>日历
- 使用 **calendarGroupId** 属性可获取创建[日历](/graph/api/resources/calendar?view=graph-rest-beta)的[日历组](/graph/api/resources/calendargroup?view=graph-rest-beta)。
- 使用 **isDraft** 属性可将[事件](/graph/api/resources/event?view=graph-rest-beta)标识为用户已在 Outlook 中更新但尚未发送给更新与会者的会议。

### <a name="cloud-communications"></a>云通信
- 使用 [createOrGet](/graph/api/onlinemeeting-createorget?view=graph-rest-beta) 按自定义外部 ID 获取[联机会议](/graph/api/resources/onlinemeeting?view=graph-rest-beta)实例，并在不存在此实例时创建一个实例。
- 可选择使用 **externalId** 属性来标识具有自定义外部 ID 的联机会议。
- 使用可选的 `Accept-Language`HTTP 请求标头[创建](/graph/api/application-post-onlinemeetings?view=graph-rest-beta)或[获取](/graph/api/onlinemeeting-get?view=graph-rest-beta)联机会议实例，以在成功操作时，采用指定语言和区域设置显示 **joinInformation** 属性的内容。

### <a name="devices-and-apps"></a>设备和应用
Intune [3 月](changelog.md#march-2020)更新。

### <a name="identity-and-access"></a>标识和访问
- 使用 `Auditlogs.Read.All` 权限可列出[用户](/graph/api/resources/user?view=graph-rest-beta)的[登录活动](/graph/api/resources/signinactivity?view=graph-rest-beta)。
- 使用 [Azure 资源的 Privileged Identity Management (PIM)](/graph/api/resources/privilegedidentitymanagement-resources?view=graph-rest-beta) 的 `PrivilegedAccess.Read.AzureResources` 应用程序级别权限为管理组、订阅、资源组和资源级别的 Azure 基础结构角色设置实时访问工作流。
- 使用 [identitySecurityDefaultsEnforcementPolicy](/graph/api/resources/identitysecuritydefaultsenforcementpolicy?view=graph-rest-beta) 实体可[获取](/graph/api/identitysecuritydefaultsenforcementpolicy-get?view=graph-rest-beta)或[更新](/graph/api/identitysecuritydefaultsenforcementpolicy-update?view=graph-rest-beta)预配置的默认安全设置，以保护组织免受常见攻击。
- 调用条件访问 API 时，请使用 `identity` 段。 例如，要[获取](/graph/api/conditionalaccesspolicy-get?view=graph-rest-beta)[条件性访问策略](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta)：`GET https://graph.microsoft.com/beta/identity/conditionalAccess/policies/{id}`。
- 使用 **authenticationRequirement** 属性可获取通过所有登录步骤所需的最高级别的身份验证，以便[登录](/graph/api/resources/signin?view=graph-rest-beta)成功。
- 在[列出租户中发生的预配事件](/graph/api/provisioningobjectsummary-list?view=graph-rest-beta)时，请使用分页。

### <a name="search"></a>搜索
- 若要将文件中的数据添加到搜索结果中，只需将数据作为 [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta) 编制索引即可。 **externalFile** 类型已遭弃用。
- [更新](/graph/api/externalitem-update?view=graph-rest-beta)[索引中的项](/graph/api/resources/externalitem?view=graph-rest-beta)，具体方法为专门更新纯文本表示的项（用 **content** 属性表示），或项的属性包（用 **properties** 属性表示）。 由于更新属性包中的任何属性都会覆盖整个属性包，因此请务必在更新中显式添加项的所有属性。
- 在调用 **externalItem** 的 [create](/graph/api/externalconnection-put-items?view=graph-rest-beta)、[update](/graph/api/externalitem-update?view=graph-rest-beta) 或 [delete](/graph/api/externalitem-delete?view=graph-rest-beta) 操作后，检查 `HTTP 429` 和 `Retry-After` 响应头。 使用 `Retry-After` 延迟来回退请求是从[限制](throttling.md#best-practices-to-handle-throttling)中恢复的最快方法。

### <a name="teamwork"></a>团队合作
使用 `ChannelMessage.Read.All` 应用程序级别权限，在没有登录用户的情况下读取频道中的 [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta) 实例。

### <a name="universal-print"></a>通用打印
调试允许用户在 web 上或从应用程序上打印的[通用打印 API](universal-print-concept-overview.md)。 借助 API，IT 管理员能够在 Microsoft 365 云远程打印机中管理用户和组对打印机的访问权限，以保持可用性、监视打印机状态，报告存档的打印作业和使用情况。 

注意：自 2020 年 3 月起，通用打印_服务_仅在个人预览版中提供。 参见[宣布推出通用打印：基于云的打印解决方案](https://aka.ms/announcinguniversalprint)，了解有关参与的详细信息。


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

