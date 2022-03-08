---
title: Microsoft Graph 新增功能
description: Microsoft Graph 新增功能
author: angelgolfer-ms
ms.localizationpriority: high
ms.openlocfilehash: 79d281a04cf4ae1dc683efa93da394e59bdc9149
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63333832"
---
# <a name="whats-new-in-microsoft-graph"></a>Microsoft Graph 新增功能

查看 Microsoft Graph 中的最近两个月新增功能要点、[以前增加的内容](whats-new-earlier.md)以及如何[分享你的想法](#want-to-stay-in-the-loop)。 有关 API 级更新的详细列表，请参见 [API更改日志](https://developer.microsoft.com/graph/changelog/)。 

> [!IMPORTANT]
> 处于 _预览_ 状态的功能（包括 API 和工具）可能会发生更改，恕不另行通知，有些功能可能永远不会提升为正式发布 (GA) 状态。不要在生产应用中使用预览功能。


## <a name="february-2022-new-and-generally-available"></a>2022 年 2 月：新版本和正式版

### <a name="teamwork"></a>Teamwork
通过 **onlineMeetingInfo** 属性获取与 [聊天](/graph/api/resources/chat)关联的 [联机会议的详细信息](/graph/api/resources/teamworkOnlineMeetingInfo)。

## <a name="february-2022-new-in-preview-only"></a>2022 年 2 月：仅限预览版中的新增功能

### <a name="change-notifications"></a>更改通知
订阅 Outlook 联系人、事件或消息的更改，以接收有效负载中包含资源数据的通知。 有关详细信息，请参阅 [Microsoft Graph 中 Outlook 资源的更改通知](outlook-change-notifications-overview.md)。

### <a name="identity-and-access--directory-management"></a>身份和访问 | 目录管理
使用应用程序权限 `CustomSecAttributeAssignment.Read.All` 为没有登录用户的组织读取[自定义安全属性定义](/graph/api/resources/customsecurityattributedefinition?view=graph-rest-beta&preserve-view=true)。

### <a name="identity-and-access--governance"></a>标识和访问权限 | 治理
- 在多阶段访问评审中为每个[阶段](/graph/api/resources/accessreviewstage?view=graph-rest-beta&preserve-view=true)配置[设置](/graph/api/resources/accessreviewstagesettings?view=graph-rest-beta&preserve-view=true)。 除了[获取](/graph/api/accessreviewstage-get?view=graph-rest-beta&preserve-view=true)或[更新](/graph/api/accessreviewstage-update?view=graph-rest-beta&preserve-view=true)访问评审阶段外，还可以执行以下操作： 
  - [阻止](/graph/api/accessreviewstage-stop?view=graph-rest-beta&preserve-view=true)审阅者向阶段提供更多输入，并继续进行下一个阶段（如果适用）。 
  - [筛选](/graph/api/accessreviewstage-filterbycurrentuser?view=graph-rest-beta&preserve-view=true)并获取[访问评审实例](/graph/api/resources/accessreviewinstance?view=graph-rest-beta&preserve-view=true)的所有阶段，其中调用用户是其审阅者
  - [列出](/graph/api/accessreviewstage-list-decisions?view=graph-rest-beta&preserve-view=true)多阶段访问评审中的决策。
- 应用可以使用应用程序权限 `EntitlementManagement.ReadWrite.All` 来[创建访问包资源请求](/graph/api/entitlementmanagement-post-accesspackageresourcerequests?view=graph-rest-beta&preserve-view=true)，以向[访问包目录](/graph/api/resources/accesspackagecatalog?view=graph-rest-beta&preserve-view=true)添加或删除资源。

### <a name="identity-and-access--identity-and-sign-in"></a>标识和访问权限 | 标识和登录
- 使用大量新属性配置[组织的品牌](/graph/api/resources/organizationalbrandingproperties?view=graph-rest-beta&preserve-view=true)。 例如，登录页面的公司徽标的横幅版本、具有基于 CDN 的 URL 的自定义图标，以及供用户管理帐户的一些其他自定义属性。
- 在[条件访问策略](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta&preserve-view=true)中包括或排除 Linux 作为[平台](/graph/api/resources/conditionalaccessplatforms?view=graph-rest-beta&preserve-view=true)条件之一。
- 使用 Azure AD 确定组织中的[风险服务主体](/graph/api/resources/riskyserviceprincipal?view=graph-rest-beta&preserve-view=true)，它会持续根据各种信号和机器学习[检测和评估](/graph/api/resources/serviceprincipalriskdetection?view=graph-rest-beta&preserve-view=true)风险。 可以[确认](/graph/api/riskyserviceprincipal-confirmcompromised?view=graph-rest-beta&preserve-view=true)风险服务主体是否确实遭到入侵，Microsoft 将据此对其禁用该服务主体对象。 可以[消除](/graph/api/riskyserviceprincipal-dismiss?view=graph-rest-beta&preserve-view=true)风险服务主体的风险。 此外，还可以列出服务主体的[风险历史记录](/graph/api/riskyserviceprincipal-list-history?view=graph-rest-beta&preserve-view=true)。
- 使用[跨租户访问设置](/graph/api/resources/crosstenantaccesspolicy-overview?view=graph-rest-beta&preserve-view=true)来控制和管理组织中用户与其他组织之间的协作。 它们非常细化，可让你确定组织和外部组织中可以参与 Azure AD B2B 协作和 Azure AD B2B 直接连接的用户、组和应用程序。 
- 启用或禁用组织中的用户和组以使用 [Azure AD 本机基于证书的身份验证 (CBA)](/graph/api/resources/x509CertificateAuthenticationMethodConfiguration?view=graph-rest-beta&preserve-view=true)。

## <a name="january-2022-new-and-generally-available"></a>2022 年 1 月: 新版本和正式版

### <a name="devices-and-apps--service-health-and-communications"></a>设备和应用|服务运行状况和通信
获取 [服务更新消息](/graph/api/resources/serviceupdatemessage) 中添加的 [服务公告附件](/graph/api/resources/serviceAnnouncementAttachment)。

### <a name="identity-and-access--governance"></a>标识和访问权限 | 治理
- 获取[访问评审审阅者](/graph/api/resources/accessreviewreviewer)资源的集合，这些资源用于定义与[访问审阅实例](/graph/api/resources/accessReviewInstance)联系的审阅者。
- 区分通过 [访问评审决策](/graph/api/resources/accessreviewinstancedecisionitem) 表示其访问权限的 3 种类型的资源:
  - [访问包分配策略](/graph/api/resources/accessReviewInstanceDecisionItemAccessPackageAssignmentPolicyResource) 访问权限由访问评审决策确定。
  - [Azure 资源角色](/graph/api/resources/accessReviewInstanceDecisionItemAzureRoleResource) 访问权限由访问评审决策确定。
  - [服务主体](/graph/api/resources/accessReviewInstanceDecisionItemServicePrincipalResource) 对资源的访问权限由访问评审决策决定。

### <a name="identity-and-access--identity-and-sign-in"></a>标识和访问权限 | 标识和登录
强制执行 [会话控制](/graph/api/resources/conditionalAccessSessionControls) (通过设置 **disableResilienceDefaults** 属性) 来确定 Azure AD 是否应根据中断前收集的信息扩展现有会话。

### <a name="teamwork"></a>Teamwork
使用应用程序权限 [创建聊天](/graph/api/chat-post)。

## <a name="january-2022-new-in-preview-only"></a>2022 年 1 月: 仅限预览版新增功能

### <a name="compliance--ediscovery"></a>合规性 | 电子数据展示
获取保管人的 OneDrive for Business 站点的 URL（[userSource](/graph/api/resources/ediscovery-userSource?view=graph-rest-beta&preserve-view=true) 的 **siteWebUrl** 属性）。

### <a name="devices-and-apps--cloud-pc"></a>设备和应用 | 云电脑
- 获取或更新 [组织的设置](/graph/api/resources/cloudpcorganizationsettings?view=graph-rest-beta&preserve-view=true)，其中包括要在云电脑上预配的 Windows 操作系统版本，以及预配的云电脑上的用户帐户类型。
- [在指定的云电脑上更改用户帐户类型](/graph/api/cloudPC-changeUserAccountType?view=graph-rest-beta&preserve-view=true)。

### <a name="identity-and-access--governance"></a>标识和访问权限 | 治理
- 访问评审的审阅者可以 [记录](/graph/api/accessreviewinstancedecisionitem-recordalldecisions?view=graph-rest-beta&preserve-view=true) 当前用户为审阅者的决策。
- 配置 [用户作为见解最后一次登录的日期和时间](/graph/api/resources/userLastSignInRecommendationInsightSetting?view=graph-rest-beta&preserve-view=true)，以帮助审查员对 [访问审查时间表的定义](/graph/api/resources/accessreviewscheduledefinition?view=graph-rest-beta&preserve-view=true) 做出决定。
- 配置在 [审查实例中对用户或委托人访问权限决定](/graph/api/resources/accessreviewinstancedecisionitem?view=graph-rest-beta&preserve-view=true) 见解时的 [用户最后登录日期和时间](/graph/api/resources/userSignInInsight?view=graph-rest-beta&preserve-view=true)。
- 访问包的请求者可以提供自定义信息作为 [访问包资源](/graph/api/resources/accesspackageresource?view=graph-rest-beta&preserve-view=true) 的一部分，这些资源可用于为访问包做出审批决策。
- 请求者可以在 [访问包分配策略](/graph/api/resources/accesspackageassignmentpolicy?view=graph-rest-beta&preserve-view=true) 中编辑 [问题](/graph/api/resources/accessPackageQuestion?view=graph-rest-beta&preserve-view=true) 的答案。

### <a name="reports--identity-and-access-reports"></a>报告 | 身份和访问报告
- 获取 [为用户注册的身份验证方法](/graph/api/resources/userRegistrationDetails?view=graph-rest-beta&preserve-view=true) 的详细信息，例如多重身份验证、自助式密码重置和无密码身份验证。
- 为组织中的用户或应用程序的 [登录](/graph/api/resources/signIn?view=graph-rest-beta&preserve-view=true) 事件获取以下属性: 
  - 任何有条件的访问 [认证环境](/graph/api/resources/authenticationContext?view=graph-rest-beta&preserve-view=true)。
  - 任何有条件的访问 [会话寿命策略](/graph/api/resources/sessionLifetimePolicy?view=graph-rest-beta&preserve-view=true)。
  - 登录期间访问的 Azure 资源的 ID。
  - 应用程序的联合标识凭据 (如果用于登录) 的标识符。
  - 在登录事件中代表目标资源的服务主体标识符。

### <a name="reports--microsoft-365-usage-reports"></a>报告 | Microsoft 365 使用情况报告
获取美国政府 Microsoft Cloud 的 Outlook、OneDrive 和 SharePoint 使用情况报告。请参阅[云部署](/graph/api/resources/report?view=graph-rest-beta&preserve-view=true#cloud-deployments)摘要。

### <a name="sites-and-lists"></a>网站和列表
- 使用 [addCopyFromContentTypeHub](/graph/api/contenttype-addcopyfromcontenttypehub?view=graph-rest-beta&preserve-view=true) 操作，将内容类型从内容类型中心添加或同步到 [网站](/graph/api/resources/site?view=graph-rest-beta&preserve-view=true) 或 [列表](/graph/api/resources/list?view=graph-rest-beta&preserve-view=true)。 这使得内容类型或其更新可用于需要它的特定站点或列表。 这是对传统同步基础结构的一项改进，后者将内容类型推送到整个组织中的所有站点，从而减少了发布传播的等待时间。 
- 获取一个或多个在站点或列表上发生的[丰富的长时间运行的操作](/graph/api/resources/richlongrunningoperation?view=graph-rest-beta&preserve-view=true)，在同步添加内容类型时可能会发生这种情况。
- 通过使用 [getCompatibleHubContentTypes](/graph/api/contenttype-getcompatiblehubcontenttypes?view=graph-rest-beta&preserve-view=true)操作，从内容类型中心获取兼容的 [内容类型](/graph/api/resources/contentType?view=graph-rest-beta&preserve-view=true) 资源集合。 

### <a name="teamwork"></a>Teamwork
- 允许用户 [在列出聊天中的消息](/graph/api/chat-list-messages?view=graph-rest-beta&preserve-view=true) 时选择 **LastModifiedDateTime** 或 **CreatedDateTime** 作为排序顺序。
- 当机器人代表用户发送 [聊天消息](/graph/api/resources/chatmessage?view=graph-rest-beta&preserve-view=true) 时，请指定用户属性 (在 **onBehalfOf** 属性中)。
- 将以下类型的成员添加到 [聊天](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true) 中:
  - [匿名来宾](/graph/api/resources/anonymousGuestConversationMember?view=graph-rest-beta&preserve-view=true)
  - [Microsoft 账户用户](/graph/api/resources/microsoftAccountUserConversationMember?view=graph-rest-beta&preserve-view=true)
  - [Skype for Business 用户](/graph/api/resources/skypeForBusinessUserConversationMember?view=graph-rest-beta&preserve-view=true)
  - [Skype 用户](/graph/api/resources/skypeUserConversationMember?view=graph-rest-beta&preserve-view=true)
- 使用委派权限 `TeamworkTag.Read` 代表已登录用户读取 Teams 中的[标记](/graph/api/resources/teamworktag?view=graph-rest-beta&preserve-view=true)和[标记成员](/graph/api/resources/teamworktagmember?view=graph-rest-beta&preserve-view=true)。

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
