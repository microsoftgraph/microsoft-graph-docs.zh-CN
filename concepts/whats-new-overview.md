---
title: Microsoft Graph 新增功能
description: Microsoft Graph 新增功能
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 94fab900fafb780c4561d82df4b82a8d210da4f0
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873375"
---
# <a name="whats-new-in-microsoft-graph"></a>Microsoft Graph 新增功能

查看 Microsoft Graph 中的最近两个月新增功能要点、[以前增加的内容](whats-new-earlier.md)以及如何[分享你的想法](#want-to-stay-in-the-loop)。 有关 API 级更新的详细列表，请参见 [API更改日志](changelog.md)。 

> [!IMPORTANT]
> _预览_状态下的功能（包括 API 和工具）可能会发生更改，恕不另行通知，有些功能可能永远不会提升为正式发布 (GA) 状态。 不要在成品应用中使用预览功能。

## <a name="august-2020-new-and-generally-available"></a>2020 年 8 月：新版本和正式版

### <a name="change-notifications"></a>更改通知
在 Microsoft Graph for US Government 国家云中[跟踪受支持资源的更改](delta-query-overview.md)。

### <a name="teamwork"></a>团队合作
- 通过[应用程序定义](/graph/api/resources/teamsappdefinition)的 **publishingState** 属性获取 Microsoft Teams [应用](/graph/api/resources/teamsapp)的发布状态。 可能的值为 `submitted`、`published` 和 `rejected`。 请参阅[示例](/graph/api/teamsapp-list?view=graph-rest-1.0&tabs=http#example-3-list-applications-with-a-given-id-and-return-the-submission-review-state)。
- 使用 `AppCatalog.Submit` 委派的权限，允许用户[提交应用](/graph/api/teamsapp-publish)并请求管理员审查。 对用户使用相同的权限来[取消](/graph/api/teamsapp-delete)过去提交的尚未发布的应用。 

## <a name="august-2020-new-in-preview-only"></a>2020 年 8 月：仅限预览版新增功能

### <a name="applications"></a>应用程序
在[服务主体](/graph/api/resources/serviceprincipal?view=graph-rest-beta)应用程序资源中支持基于密码的单点登录，并在 **passwordSingleSignOnSettings** 属性中指定此类[设置](/graph/api/resources/passwordsinglesignonsettings?view=graph-rest-beta)。 有关 Azure AD 中基于密码的单一登录的信息，请参阅[配置基于密码的单一登录](/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications)。

### <a name="calendar"></a>日历
增强对涉及定期[事件](/graph/api/resources/event?view=graph-rest-beta)的方案的编程支持：
- 通过使用 **occurrenceId** 属性，可以可靠地标识定期数据系列中的任何事件，包括已修改或已取消的事件。
- 通过使用 **exceptionOccurrences** 属性获取定期数据系列中的任何例外事件。
- 通过使用 **cancelledOccurrences** 属性获取数据系列中的任何取消事件。

### <a name="change-notifications"></a>更改通知
- 使用[订阅](/graph/api/resources/subscription?view=graph-rest-beta)的 **includeResourceData** 属性，以[设置包含资源数据的更改通知](webhooks-with-resource-data.md)。 不要使用 **includeProperties** 属性。
- 获取[通过事件中心发送的更改通知](change-notifications-delivery.md)。

### <a name="devices-and-apps--cloud-printing"></a>设备和应用 | 云打印
- 通过使用 **allowAllUser** 属性向所有用户和组授予对[打印机共享](/graph/api/resources/printershare?view=graph-rest-beta)的访问权限。
- 使用新的委派和应用程序权限来访问或管理[打印文档](/graph/api/resources/printDocument?view=graph-rest-beta)、[打印作业](/graph/api/resources/printjob?view=graph-rest-beta)、[打印机](/graph/api/resources/printer?view=graph-rest-beta)、[打印机共享](/graph/api/resources/printershare?view=graph-rest-beta)或[打印任务定义](/graph/api/resources/printtaskdefinition?view=graph-rest-beta)。 有关详细信息，请参阅云打印 [8 月](changelog.md#august-2020)更新。

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理
beta 版本中的 Intune [8 月](changelog.md#august-2020)更新。

### <a name="identity-and-access--governance"></a>身份和访问 | 治理
- 自定义[使用条款协议](/graph/api/resources/agreement?view=graph-rest-beta)，以支持协议的到期日和频率，要求用户按设备接受协议，或者按设定的频率重新接受协议。 
- 使用 **file** 属性导航到某个[自定义协议](/graph/api/resources/agreementfile?view=graph-rest-beta)以了解使用条款。 不要使用 **files** 属性。
- 添加、删除和列出内部或外部发起人，他们可以批准[互联组织](/graph/api/resources/connectedorganization?view=graph-rest-beta)关于访问组、应用程序或 SharePoint Online 网站的请求。 有关详细信息，请参阅[权利管理](/graph/api/resources/entitlementmanagement-root?view=graph-rest-beta)。

### <a name="people-and-workplace-intelligence--profile"></a>人员和工作场所智能 | 个人资料
在用户的[个人资料](/graph/api/resources/profile?view=graph-rest-beta)中添加和管理以下额外属性，这些属性可以在 Microsoft 365 和第三方应用程序的共享人员体验中体现：
- [地址](/graph/api/resources/itemAddress?view=graph-rest-beta)
- [纪念日](/graph/api/resources/personAnniversary?view=graph-rest-beta)
- [奖项](/graph/api/resources/personAward?view=graph-rest-beta)
- [证书](/graph/api/resources/personCertification?view=graph-rest-beta)
- [笔记](/graph/api/resources/personAnnotation?view=graph-rest-beta)：
- [专利](/graph/api/resources/itemPatent?view=graph-rest-beta)
- [出版物](/graph/api/resources/itemPublication?view=graph-rest-beta)


### <a name="reports--microsoft-365-usage-reports"></a>报告 | Microsoft 365 使用情况报告
获取[有关 Microsoft 365 应用使用情况的报告](/graph/api/resources/microsoft-365-apps-usage-report?view=graph-rest-beta)，特别是有关用户详细信息、用户数量和平台用户数量的报告。

### <a name="teamwork"></a>团队合作
获取[在聊天消息中托管的内容](/graph/api/resources/chatMessageHostedContent?view=graph-rest-beta)（如图像或代码段）。 请参阅[示例](/graph/api/chatmessagehostedcontent-get?view=graph-rest-beta&branch=master#example-2-get-hosted-content-bytes-for-an-image)，获取图像的内容字节。

### <a name="to-do-tasks"></a>待办任务
- 针对[微软待办](todo-concept-overview.md)推出了一组新 API，允许应用用户跨 Microsoft 365 客户端应用组织和跟踪个人任务。 有关详细信息，请参阅[使用微软待办 API](/graph/api/resources/todo-overview?view=graph-rest-beta)。
- 弃用 [Outlook 任务 API](/graph/api/resources/outlooktask?view=graph-rest-beta)。

## <a name="july-2020-new-and-generally-available"></a>2020 年 7 月：新版本和正式版

### <a name="calendar"></a>日历
正式发布一项功能，它允许组织者接受备选会议时间提案，并允许受邀者在[暂时接受](/graph/api/event-tentativelyaccept?view=graph-rest-1.0)或[拒绝](/graph/api/event-decline?view=graph-rest-1.0)事件时[为会议建议新时间](outlook-calendar-meeting-proposals.md)。

### <a name="change-notifications"></a>更改通知
已删除从 [changeNotification](/graph/api/resources/changenotification) 类型中错误引入的 **sequenceNumber** 资源。

### <a name="groups"></a>组
[group](/graph/api/resources/group?view=graph-rest-v1.0) 实体下列属性的通用版本：**assignedLabels**、**expirationDateTime**、**membershipRule**、**membershipRuleProcessingState**、**preferredLanguage** 和 **theme**。

### <a name="identity-and-access"></a>身份和访问
- 删除作为[设备](/graph/api/resources/device)的注册所有者或用户的用户。
- 跟踪对新创建、更新或删除的应用程序本地表示形式（由 [servicePrincipals](/graph/api/resources/serviceprincipal) 资源表示）和委派权限授予（由 [oAuth2PermissionGrant](/graph/api/resources/oauth2permissiongrant) 资源表示）的更改，而无需对整个资源集合执行完全读取操作。
- 正式发布[用于强制安全性默认设置的策略](/graph/api/resources/identitysecuritydefaultsenforcementpolicy)，可以保护组织免受常见攻击。

### <a name="identity-and-access--identity-and-sign-in"></a>身份和访问 | 身份和登录
- 正式发布[条件访问策略](/graph/api/resources/conditionalAccessPolicy)，它们是用于定义访问方案的自定义规则。
- 正式发布表示自定义规则的[命名位置](/graph/api/resources/namedLocation)，用于定义在条件访问策略中使用的网络位置。

### <a name="schema-extensions"></a>架构扩展
[架构扩展](/graph/api/resources/schemaextension)功能现在可在[Microsoft Cloud for US Government](/graph/deployments)使用。

### <a name="teamwork"></a>团队合作
使用 `TeamsAppInstallation.ReadForTeam` 或 `TeamsAppInstallation.ReadWriteForTeam` 的委派权限，或者使用 `TeamsAppInstallation.ReadForTeam.All` 或 `TeamsAppInstallation.ReadWriteForTeam.All` 的应用程序权限来[列出已在团队中安装的应用](/graph/api/teamsappinstallation-list)。

## <a name="july-2020-new-in-preview-only"></a>2020 年 7 月：预览版新增功能

### <a name="cloud-communications"></a>云通信
- 使用[更新](/graph/api/onlinemeeting-update?view=graph-rest-beta)操作来更新[联机会议](/graph/api/resources/onlinemeeting?view=graph-rest-beta)的 **startDateTime**、**endDateTime**、**participants** 或 **subject** 属性。
- 订阅有关 Microsoft Teams 上用户可用性更改的通知，如[状态](/graph/api/resources/presence?view=graph-rest-beta)资源所示。

### <a name="cloud-communications--call-records"></a>云通信 | 通话记录
- [获取](/graph/api/callrecords-callrecord-getpstncalls?view=graph-rest-beta)公用电话交换网 (PSTN) 通话的记录。
- [获取](/graph/api/callrecords-callrecord-getdirectroutingcalls?view=graph-rest-beta)直接路由通话的记录。

### <a name="compliance--ediscovery"></a>合规性 | 电子数据展示
首次推出的[电子数据展示事例](/graph/api/resources/ediscoverycase?view=graph-rest-beta)包含可在法律案件中作为证据的保管人、保留、集合、管理审阅集和导出。
应用现在可以对收集用于诉讼、调查或法规请求的[审阅集数据](/graph/api/resources/reviewset?view=graph-rest-beta)进行[查询](/graph/api/resources/reviewsetquery?view=graph-rest-beta)和挑选。 这一首次推出的内容是 Microsoft 365 [高级电子数据展示](/microsoft-365/compliance/overview-ediscovery-20?view=o365-worldwide)的一部分。

### <a name="devices-and-apps--cloud-printing"></a>设备和应用 | 云打印
- 使用应用程序权限 `Printer.ReadWrite.All` 和 [Internet 打印协议（IPP）编码](https://tools.ietf.org/html/rfc8010)至[更新打印机](/graph/api/printer-update?view=graph-rest-beta)。
- 使用以下应用权限之一、`PrintJob.ReadBasic.All`、`PrintJob.Read.All`、`PrintJob.ReadWriteBasic.All` 或 `PrintJob.ReadWrite.All`，来[获取打印作业](/graph/api/printjob-get?view=graph-rest-beta)或[列出打印机打印作业](/graph/api/printer-list-jobs?view=graph-rest-beta)。
- [获取打印作业](/graph/api/printjob-get?view=graph-rest-beta)时，请使用 `$expand` 获取对作业正在执行或已执行的[打印作业](/graph/api/resources/printtask?view=graph-rest-beta)。 [截取打印](universal-print-concept-overview.md#extending-universal-print-to-support-pull-printing)中使用打印任务、[任务定义](/graph/api/resources/printtaskdefinition?view=graph-rest-beta)、和[任务触发器](/graph/api/resources/printtasktrigger?view=graph-rest-beta)。
- [重定向打印作业](/graph/api/printjob-redirect?view=graph-rest-beta)至其他打印机，作为截取打印的组成部分。

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理
Intune [7 月](changelog.md#july-2020)试用版更新。

### <a name="groups"></a>组
使用 Microsoft 365 [组](/graph/api/resources/group?view=graph-rest-beta)的 **isAssignableToRole** 属性，并在创建组的过程中对其进行设置，以指示该组是否可以分配给 Azure AD 角色。 这[有助于在 Azure AD 中管理角色分配](/azure/active-directory/users-groups-roles/roles-groups-concept)，例如特权角色管理员或全局管理员可以创建 Microsoft 365 组并向该组分配 Azure AD 角色，而不是向单个用户分配这一角色，这样一来，用户加入该_组_后，他们会被间接分配既定角色。

### <a name="identity-and-access"></a>身份和访问
- [获取访问令牌](/graph/api/synchronization-synchronization-acquireAccessToken?view=graph-rest-beta)，以授权 Azure AD 预配服务将用户预配到应用程序。
- [获取](/graph/api/entitlementmanagementsettings-get?view=graph-rest-beta)或[更新](/graph/api/entitlementmanagementsettings-update?view=graph-rest-beta)权限管理设置，这些设置控制对组织内部和外部用户的组、应用程序和 SharePoint Online 网站的访问权限。 

### <a name="identity-and-access--identity-and-sign-in"></a>身份和访问 | 身份和登录
- 将用户风险级别（`low`、`medium`、`high`、`none`）包含为应用 [条件访问策略](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta)的注意事项。
- [使用密码更改作为授予控制](/graph/api/resources/conditionalaccessgrantcontrols?view=graph-rest-beta#special-considerations-when-using-passwordchange-as-a-control)，以便传递条件访问策略。
- 在 Azure AD 租户和 Azure AD B2C 租户中，将 [OpenID Connect 提供程序](/graph/api/resources/openidconnectprovider?view=graph-rest-beta) (OIDC) 用作标识提供程序。 其 **claimsMapping** 属性允许 Azure AD 将 OIDC 提供程序的[声明映射](/graph/api/resources/claimsmapping?view=graph-rest-beta)到 Azure AD 可识别和使用的声明。

### <a name="people-and-workplace-intelligence--insights"></a>人脉和工作场所智能|见解
在 Microsoft 365 中，对[项见解](/graph/api/resources/iteminsights?view=graph-rest-beta)的可用性和显示进行更[精细的隐私控制](insights-customize-item-insights-privacy.md)。 这些见解表示 OneDrive for Business 中的用户和文档之间的关系，并使用高级分析和机器学习技术进行计算。 

### <a name="people-and-workplace-intelligence--profile-card-customization"></a>人脉和工作区智能 | 个人资料卡片自定义
管理员可以使用[个人资料卡属性](/graph/api/resources/profilecardproperty?view=graph-rest-beta) API，[自定义显示在组织个人资料卡上的属性](add-properties-profilecard.md)。

### <a name="sites-and-lists"></a>网站和列表
访问 SharePoint [术语库](/graph/api/resources/termstore-store?view=graph-rest-beta)分类系统，该系统的层次结构包括 [group](/graph/api/resources/termstore-group?view=graph-rest-beta)、[set](/graph/api/resources/termstore-set?view=graph-rest-beta) 和 [term](/graph/api/resources/termstore-term?view=graph-rest-beta) 资源，以及术语之间的 [relation](/graph/api/resources/termstore-relation?view=graph-rest-beta) 资源。

### <a name="workbooks-and-charts"></a>工作簿和图表
[获取[工作簿](/graph/api/resources/workbook?view=graph-rest-beta)中长时间运行[操作](/graph/api/resources/workbookoperation?view=graph-rest-beta)的状态和任何结果](/graph/api/workbookoperation-get?view=graph-rest-beta)。


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

