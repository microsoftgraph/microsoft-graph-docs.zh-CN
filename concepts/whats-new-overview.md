---
title: Microsoft Graph 新增功能
description: Microsoft Graph 新增功能
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: d1d7d483e6061c86cc25641fc1f02e0130c62d93
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48192726"
---
# <a name="whats-new-in-microsoft-graph"></a>Microsoft Graph 新增功能

查看 Microsoft Graph 中的最近两个月新增功能要点、[以前增加的内容](whats-new-earlier.md)以及如何[分享你的想法](#want-to-stay-in-the-loop)。 有关 API 级更新的详细列表，请参见 [API更改日志](changelog.md)。 

> [!IMPORTANT]
> _预览_状态下的功能（包括 API 和工具）可能会发生更改，恕不另行通知，有些功能可能永远不会提升为正式发布 (GA) 状态。 不要在成品应用中使用预览功能。


## <a name="september-2020-new-and-generally-available"></a>2020 年 9 月：新版本和正式版

### <a name="calendar"></a>日历
[事件](/graph/api/resources/event)资源的 **transactionId** 属性 GA，可选择由客户端应用程序设置，以避免客户端重试创建相同事件时出现多余的 POST 操作。 当低网络连接性导致客户端在从服务器中收到客户端先前创建事件请求的响应之前超时时，此功能很有用。

### <a name="cloud-communications"></a>云通信
[从[通话](/graph/api/resources/call)中删除参与者](/graph/api/participant-delete)。 即使在有必要删除活动通话的参与者的情况下，也可以使用此操作。

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理
Intune [v 1.0 版的 9 月](changelog.md#september-2020) 更新。

### <a name="identity-and-access--directory-management"></a>身份和访问 | 目录管理
GA [管理单元 API](/graph/api/resources/administrativeunit) ，允许组织细分其 Azure Active Directory、管理这些细分并将管理职责委派给这些细分。 这些细分项可以代表区域、部门、成本中心等。

### <a name="reports"></a>报告
[获取含 Outlook 2019 和 Outlook for Microsoft 365 唯一用户的计数报告](/graph/api/reportroot-getemailappusageversionsusercounts)。

<!--
### Use the SDKs
GA of the Microsoft Graph PowerShell SDK (https://github.com/microsoftgraph/msgraph-sdk-powershell) which enables access to the entire surface of Microsoft Graph in a straightforward and consistent way.
-->

### <a name="teamwork"></a>团队合作
- 获取 **lastEditedDateTime** 属性，确定发件人上次编辑[聊天](/graph/api/resources/chatmessage)邮件的时间。
- 获取 **lastModifiedDateTime** 属性，确定发件人何时创建聊天邮件，或者任何人以其他方式修改邮件，包括添加或删除反应。 

### <a name="use-the-toolkit"></a>使用工具包
尝试使用 Microsoft Graph 工具包的全新分步入门教程，并体验工具包带来的方便性：
- [使用 JavaScript 构建 Web 应用程序](/graph/toolkit/get-started/build-a-web-app)
- [构建 SharePoint Web 部件](/graph/toolkit/get-started/build-a-sharepoint-web-part)
- [构建 Microsoft Teams 选项卡](/graph/toolkit/get-started/build-a-microsoft-teams-tab)
- [使用 React 的工具包](/graph/toolkit/get-started/use-toolkit-with-react)
- [使用 Angular 的工具包](/graph/toolkit/get-started/use-toolkit-with-angular)

### <a name="users"></a>用户
除通过“**邮件**属性” 获取[用户](/graph/api/resources/user) 的 SMTP 地址之外，你现在可以设置该属性并更新用户的电子邮件地址。 

## <a name="september-2020-new-in-preview-only"></a>2020 年 9 月：仅限预览版的新增功能

### <a name="cloud-communications"></a>云通信
- 弃用了 [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true)的 **autoAdmittedUsers** 属性。 使用新的 **lobbyBypassSettings** 属性和 [值](/graph/api/resources/lobbybypasssettings?view=graph-rest-beta&preserve-view=true#lobbybypassscope-values)取而代之。
- 使用宣布呼叫者加入或离开联机会议的其他设置（**isEntryExitAnnounced** 属性），并允许在会议中使用特定演示者（**allowedPresenters** 属性）。

### <a name="devices-and-apps--cloud-printing"></a>设备和应用 | 云打印
- [应用 `$expand` [OData 系统查询选项](/graph/api/printer-list-jobs?view=graph-rest-beta&preserve-view=true#optional-query-parameters)获取每个与打印机相关联的打印作业的文档](/graph/api/printer-list-jobs?view=graph-rest-beta&preserve-view=true)。 
- 应用 `$filter` [OData 系统查询选项](/graph/api/printer-list-jobs?view=graph-rest-beta&preserve-view=true#optional-query-parameters)筛选创建打印作业的用户。

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理
Intune beta 版[ 9 月](changelog.md#september-2020)更新。

### <a name="identity-and-access--directory-management"></a>身份和访问 | 目录管理
[代表登录的用户（设备所有者或相应的角色）获取 BitLocker 恢复密钥](/graph/api/bitlockerrecoverykey-get?view=graph-rest-beta&preserve-view=true)。 获取恢复密钥会生成与最终用户体验存在奇偶校验的[审核日志](/azure/active-directory/reports-monitoring/concept-audit-logs)。

### <a name="identity-and-access--governance"></a>身份和访问 | 治理
在请求或删除 [给用户的访问权限包](/graph/api/resources/accesspackageassignment?view=graph-rest-beta&preserve-view=true)（用于指定对组、应用程序或 Microsoft Office SharePoint Online 网站的访问权限）时，可包括[计划](/graph/api/resources/requestschedule?view=graph-rest-beta&preserve-view=true)。

### <a name="identity-and-access--identity-and-sign-in"></a>身份和访问 | 身份和登录
组织可[获取](/graph/api/continuousaccessevaluationpolicy-get?view=graph-rest-beta&preserve-view=true)或[更新](/graph/api/continuousaccessevaluationpolicy-update?view=graph-rest-beta&preserve-view=true)[持续存取评估策略](/graph/api/resources/continuousAccessEvaluationPolicy?view=graph-rest-beta&preserve-view=true) 来实时管理身份验证会话。

### <a name="teamwork"></a>团队合作
- 获取 Teams [频道](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true)或[团队](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true)的创建日期/时间。
- [更新](/graph/api/chatmessage-update?view=graph-rest-beta&preserve-view=true)[频道](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true)或[聊天](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true)内 [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta&preserve-view=true) 的 **policyViolation** 属性，从而启用数据丢失防护 (DLP) 应用，以监控[聊天邮件策略冲突](/graph/api/resources/chatmessagepolicyviolation?view=graph-rest-beta&preserve-view=true) ，防止包含用户不应发送的数据的邮件。

### <a name="search"></a>搜索

- 在[适用于 OneDrive、SharePoint、Microsoft Graph 连接器的 Microsoft 搜索 API](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true) 中使用其他功能： 

  - 获取来自 OneDrive 和 SharePoint 的[附加类型](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true#scope-search-based-on-entity-types)内容： **驱动器**、 **列表**、 **listItem** 和**网站**。 
  - 搜索结果中的范围属性设为[所选属性](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true#get-selected-properties)。 
  - 获取 [listItem](/graph/api/resources/listitem?view=graph-rest-beta&preserve-view=true) 资源的自定义属性。
  - 对任何可排序属性上的 OneDrive 和 SharePoint 搜索结果进行[排序](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true#sort-search-results)。
  - [使用针对 OneDrive 和 SharePoint 的聚合](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true#refine-results-using-aggregations)优化结果。
- 查询通过 Microsoft Graph 连接器跨越[多个连接](/graph/search-concept-custom-types)摄取的外部数据。
- 充分利用 Microsoft Graph 连接器的增强内容，了解：
  - [管理连接](search-index-manage-connections.md)
  - [管理架构](search-index-manage-schema.md)
  - [管理项目](search-index-manage-items.md)

## <a name="august-2020-new-and-generally-available"></a>2020 年 8 月：新版本和正式版

### <a name="change-notifications"></a>更改通知
在 Microsoft Graph for US Government 国家云中[跟踪受支持资源的更改](delta-query-overview.md)。

### <a name="cloud-communications"></a>云通信
- [取消](/graph/api/call-cancelmediaprocessing)流程或队列中的任何交互式语音响应 (VR) 操作，这些操作可以是[播放音频提示](/graph/api/call-playprompt)或[录制响应](/graph/api/call-record)。
- 通过“**听录**”属性[调用听录信息](/graph/api/resources/calltranscriptioninfo)。

### <a name="teamwork"></a>团队合作
- 使用另一种方法，无需创建组即可直接[创建团队](/graph/api/team-post)。
- 使用 **members** 导航属性，以更可靠、低延迟的方式在团队中添加成员。
- 通过[应用程序定义](/graph/api/resources/teamsappdefinition)的 **publishingState** 属性获取 Microsoft Teams [应用](/graph/api/resources/teamsapp)的发布状态。 可能的值为 `submitted`、`published` 和 `rejected`。 请参阅[示例](/graph/api/teamsapp-list?view=graph-rest-beta&preserve-view=true#example-3-list-applications-with-a-given-id-and-return-the-submission-review-state)。
- 使用 `AppCatalog.Submit` 委派的权限，允许用户[提交应用](/graph/api/teamsapp-publish)并请求管理员审查。 对于用户[取消](/graph/api/teamsapp-delete)过去提交的尚未发布的应用使用相同的权限。 


## <a name="august-2020-new-in-preview-only"></a>2020 年 8 月：仅限预览版新增功能

### <a name="applications"></a>应用程序
在[服务主体](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true)应用程序资源中支持基于密码的单点登录，并在 **passwordSingleSignOnSettings** 属性中指定此类[设置](/graph/api/resources/passwordsinglesignonsettings?view=graph-rest-beta&preserve-view=true)。 有关 Azure AD 中基于密码的单一登录的信息，请参阅[配置基于密码的单一登录](/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications)。

### <a name="calendar"></a>日历
增强对涉及定期[事件](/graph/api/resources/event?view=graph-rest-beta&preserve-view=true)的方案的编程支持：
- 通过使用 **occurrenceId** 属性，可以可靠地标识定期数据系列中的任何事件，包括已修改或已取消的事件。
- 通过使用 **exceptionOccurrences** 属性获取定期数据系列中的任何例外事件。
- 通过使用 **cancelledOccurrences** 属性获取数据系列中的任何取消事件。

### <a name="change-notifications"></a>更改通知
- 使用[订阅](/graph/api/resources/subscription?view=graph-rest-beta&preserve-view=true)的 **includeResourceData** 属性，以[设置包含资源数据的更改通知](webhooks-with-resource-data.md)。 不要使用 **includeProperties** 属性。
- 获取[通过事件中心发送的更改通知](change-notifications-delivery.md)。

### <a name="devices-and-apps--cloud-printing"></a>设备和应用 | 云打印
- 通过使用 **allowAllUser** 属性向所有用户和组授予对[打印机共享](/graph/api/resources/printershare?view=graph-rest-beta&preserve-view=true)的访问权限。
- 使用新的委派和应用程序权限来访问或管理[打印文档](/graph/api/resources/printDocument?view=graph-rest-beta&preserve-view=true)、[打印作业](/graph/api/resources/printjob?view=graph-rest-beta&preserve-view=true)、[打印机](/graph/api/resources/printer?view=graph-rest-beta&preserve-view=true)、[打印机共享](/graph/api/resources/printershare?view=graph-rest-beta&preserve-view=true)或[打印任务定义](/graph/api/resources/printtaskdefinition?view=graph-rest-beta&preserve-view=true)。 有关详细信息，请参阅云打印 [8 月](changelog.md#august-2020)更新。

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理
beta 版本中的 Intune [8 月](changelog.md#august-2020)更新。

### <a name="identity-and-access--governance"></a>身份和访问 | 治理
- 自定义[使用条款协议](/graph/api/resources/agreement?view=graph-rest-beta&preserve-view=true)，以支持协议的到期日和频率，要求用户按设备接受协议，或者按设定的频率重新接受协议。 
- 使用 **file** 属性导航到某个[自定义协议](/graph/api/resources/agreementfile?view=graph-rest-beta&preserve-view=true)以了解使用条款。 不要使用 **files** 属性。
- 添加、删除和列出内部或外部发起人，他们可以批准[互联组织](/graph/api/resources/connectedorganization?view=graph-rest-beta&preserve-view=true)关于访问组、应用程序或 SharePoint Online 网站的请求。 有关详细信息，请参阅[权利管理](/graph/api/resources/entitlementmanagement-root?view=graph-rest-beta&preserve-view=true)。

### <a name="identity-and-access--identity-and-sign-in"></a>身份和访问 | 身份和登录
- 为租户启用进一步自定义[授权策略](/graph/api/resources/authorizationpolicy?view=graph-rest-beta&preserve-view=true)，例如允许[默认的用户角色](/graph/api/resources/defaultuserrolepermissions?view=graph-rest-beta&preserve-view=true)创建应用程序或安全组或读取其他用户，允许用户注册电子邮件订阅或通过电子邮件验证加入租户，或允许用户自行重置密码。
- 在 Azure Active Directory B2C 租户中，以用户流的形式管理[预定义的可配置策略](/graph/api/resources/b2cuserflows?view=graph-rest-beta&preserve-view=true)。 查看更多有关 [B2C 用户流](/azure/active-directory-b2c/user-flow-overview)的详细信息。
- 在 Azure Active Directory 租户中，启用[自助注册体验作为 B2X 用户流](/graph/api/resources/b2xuserflows?view=graph-rest-beta&preserve-view=true)。 查看更多有关[自助注册](/azure/active-directory/external-identities/self-service-sign-up-overview)的详细信息。

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
- 针对[微软待办](todo-concept-overview.md)推出了一组新 API，允许应用用户跨 Microsoft 365 客户端应用组织和跟踪个人任务。 有关详细信息，请参阅[使用微软待办 API](/graph/api/resources/todo-overview?view=graph-rest-beta&preserve-view=true)。
- 弃用 [Outlook 任务 API](/graph/api/resources/outlooktask?view=graph-rest-beta&preserve-view=true)。


## <a name="want-to-stay-in-the-loop"></a>保持循环

我们可以通过以下方式进行参与：

- 是否有希望 Microsoft Graph 支持的方案？ 在 [Microsoft Graph 用户心声](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)中建议新功能并进行投票。
    某些新功能来源于开发人员社区的热门请求。 Microsoft Graph 团队会定期评估客户需求，并按以下顺序发布新功能：

    1. 处于**_预览_** 状态的 Debut。 任何相关的 REST API 更新都在 beta 终结点 (`https://graph.microsoft.com/beta`) 中。  

    2. 如果有足够的反馈表明具有可行性，则提升为 **_正式发布_ (GA)** 状态。 任何相关的 REST API 更新都添加到 v1.0 终结点 (`https://graph.microsoft.com/v1.0`)。 
- 成为 Microsoft Graph 社区中的活跃成员! [参与](https://aka.ms/microsoftgraphcall)Microsoft Graph 社区每月通话。
- 注册 [Microsoft 365 开发人员计划](https://developer.microsoft.com/office/dev-program)，免费订阅 Microsoft 365, 然后开始开发! 


## <a name="see-also"></a>另请参阅
- 定期查看 [Microsoft Graph 开发人员博客](https://developer.microsoft.com/graph/blogs/), 了解发布公告和有帮助的资源。 
- 浏览 Microsoft Graph API 新增功能的详细信息, 以及[changelog](changelog.md)中的 API 行为更新。
- 查找[早期版本的重点内容](whats-new-earlier.md)。
- 了解有关 [Microsoft Graph 的版本控制、支持和中断性变更策略](versioning-and-support.md)。

