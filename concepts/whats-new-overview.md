---
title: Microsoft Graph 新增功能
description: Microsoft Graph 新增功能
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 3c7b076f08a9377c7b68b16d0a8b4c4cbb7c6afb
ms.sourcegitcommit: 35b37318d18b4a613b4702be1aa25b71525800c3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2020
ms.locfileid: "49721098"
---
# <a name="whats-new-in-microsoft-graph"></a>Microsoft Graph 新增功能

查看 Microsoft Graph 中的最近两个月新增功能要点、[以前增加的内容](whats-new-earlier.md)以及如何[分享你的想法](#want-to-stay-in-the-loop)。 有关 API 级更新的详细列表，请参见 [API更改日志](changelog.md)。 

> [!IMPORTANT]
> _预览_ 状态下的功能（包括 API 和工具）可能会发生更改，恕不另行通知，有些功能可能永远不会提升为正式发布 (GA) 状态。 不要在成品应用中使用预览功能。

## <a name="december-2020-new-and-generally-available"></a>2020 年 12 月：新版本和正式版

### <a name="calendar"></a>日历
- 会议组织者可以使用 [事件](/graph/api/resources/event)的 **hideAttendees** 属性来控制与会者是否可以在会议“**跟踪**”列表中看到彼此。
- 组织者可用的 **isDraft** 属性和 [cancel](/graph/api/event-cancel) 方法的 GA，以及组织者和与会者可用的 [forward](/graph/api/event-forward) 方法的 GA，以更好地管理日历中的[事件](/graph/api/resources/event)资源。
- [日历](/graph/api/resources/calendar) 的 **hexColor** 和 **isDefault** 属性的 GA 可以更好地管理日历。

### <a name="cloud-communications"></a>云通信
[状态](/graph/api/resources/presence)资源的 GA，允许获取一个或多个用户的状态信息，例如他们的可用性和用户活动。

### <a name="identity-and-access--identity-and-sign-in"></a>身份和访问 | 身份和登录
尝试新[教程](tutorial-riskdetection-api.md)，学习如何使用[身份保护 API ](/graph/api/resources/identityprotectionroot)来识别风险，并配置工作流以确认泄露或启用修复。

### <a name="teamwork"></a>团队合作
- [API 管理 Teams 应用安装](/graph/api/resources/teamsappinstallation) 的 GA，包括获取团队或用户个人范围内的 应用，或者添加、删除或更新该应用。
- [获取用户和 Teams 应用间的聊天](/graph/api/userscopeteamsappinstallation-get-chat)。

### <a name="use-the-toolkit"></a>使用工具包
Microsoft Graph 工具包 2.0 的 GA 版本 - 此版本包含新 [Microsoft Graph 待办任务组件](/graph/toolkit/components/todo)（与 [Planner 任务组件](/graph/toolkit/components/tasks)不同），以及增强的[个人卡片组件](/graph/toolkit/components/person-card)。 更多信息请参阅[相关的博客文章](https://developer.microsoft.com/zh-CN/graph/blogs/announcing-the-general-availability-of-microsoft-graph-toolkit-2-0/)。

## <a name="december-2020-new-in-preview-only"></a>2020 年 12 月：仅限预览版的新增功能

### <a name="compliance--ediscovery"></a>合规性 | 电子数据展示
继续实现 [Microsoft 365 合规 API](/graph/api/resources/ediscoveryapioverview?view=graph-rest-beta&preserve-view=true) 的管道是[保管人](/graph/api/resources/custodian?view=graph-rest-beta&preserve-view=true)资源及其相关操作和方法，以[释放](/graph/api/custodian-release?view=graph-rest-beta&preserve-view=true)或[激活](/graph/api/custodian-activate?view=graph-rest-beta&preserve-view=true)保管人。 使用 **保管人** 资源可以访问 Exchange Online 邮箱、OneDrive for Business、SharePoint 网站 ([siteSource](/graph/api/resources/siteSource?view=graph-rest-beta&preserve-view=true)) 和 Microsoft 365 组([unifiedGroupSource](/graph/api/resources/unifiedGroupSource?view=graph-rest-beta&preserve-view=true)) 中保管人的数据 ([userSource](/graph/api/resources/userSource?view=graph-rest-beta&preserve-view=true))。

### <a name="devices-and-apps--cloud-pc"></a>设备和应用 | 云电脑
在 [cloudPC](/graph/api/resources/cloudpc?view=graph-rest-beta&preserve-view=true) 资源的 **status** 属性中，将云管理虚拟机的故障状态统称为 `failed`。

### <a name="devices-and-apps--cloud-printing"></a>设备和应用 | 云打印
- [更新](/graph/api/printjob-update-configuration?view=graph-rest-beta&preserve-view=true)[打印作业](/graph/api/resources/printjob?view=graph-rest-beta&preserve-view=true)的[配置](/graph/api/resources/printjobconfiguration?view=graph-rest-beta&preserve-view=true)。
- 有关重命名一些属性和重新键入关系的详细信息，请参阅 [API 更改日志](changelog.md)的 [2020 年 12 月](changelog.md#december-2020)部分。

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
  - [Outlook 邮件](/graph/search-concept-messages)
  - [Outlook 日历事件](/graph/search-concept-events)
  - [OneDrive 和 SharePoint 资源](/graph/search-concept-files)。

### <a name="teamwork"></a>团队合作

- 特定资源 GA 允许（RSC）权限。 RSC 权限允许团队所有者向生产应用授予精确同意，以便访问和/或修改团队的特定数据，例如读取团队的设置，或者修改频道的名称、说明及其他设置。
- 适用于 [频道](/graph/api/resources/channel) 或频道内的邮件 Api 的 GA。 Api 包括：
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
可以聚合数值或字符串类型的搜索结果，[Microsoft Graph 连接器](/microsoftsearch/connectors-overview)导入这些结果，并将其在[架构](/graph/api/resources/schema?view=graph-rest-beta&preserve-view=true)中设置为可精简。 查看更多有关 [使用聚合优化搜索结果](search-concept-aggregation.md)的详细信息。


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
- 浏览 Microsoft Graph API 新增功能的详细信息, 以及[changelog](changelog.md)中的 API 行为更新。
- 查找[早期版本的重点内容](whats-new-earlier.md)。
- 了解有关 [Microsoft Graph 的版本控制、支持和中断性变更策略](versioning-and-support.md)。
