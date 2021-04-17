---
title: Microsoft Graph 新增功能
description: Microsoft Graph 新增功能
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: f841dec2b6de97ca7a67b01bf0d9e4b16dade843
ms.sourcegitcommit: 3eb37e0621540bee91f42a7c2d8457310e90f8b7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51870035"
---
# <a name="whats-new-in-microsoft-graph"></a>Microsoft Graph 新增功能

查看 Microsoft Graph 中的最近两个月新增功能要点、[以前增加的内容](whats-new-earlier.md)以及如何[分享你的想法](#want-to-stay-in-the-loop)。 有关 API 级更新的详细列表，请参见 [API更改日志](https://developer.microsoft.com/graph/changelog/)。 

> [!IMPORTANT]
> _预览_ 状态下的功能（包括 API 和工具）可能会发生更改，恕不另行通知，有些功能可能永远不会提升为正式发布 (GA) 状态。 不要在成品应用中使用预览功能。

## <a name="april-2021-new-and-generally-available"></a>2021 年 4 月：新增功能，正式可用

### <a name="teamwork"></a>团队合作
- 如果 [chatMessage](/graph/api/resources/chatmessage) 在 [频道](/graph/api/resources/channel)内，则通过 **channelIdentity** 属性标识频道。
- 如果 **[chatMessage](/graph/api/resources/chatmessage)** 在 [聊天](/graph/api/resources/chat)中，则通过 **chatId** 属性识别聊天。
- 使用 **关系** ，通过聊天或 [获取](/graph/api/resources/chatmessage) 聊天中的 [邮件](/graph/api/resources/chat)。

## <a name="april-2021-new-in-preview-only"></a>2021 年 4 月：仅预览版新增功能

### <a name="teamwork"></a>团队合作
使用 [资源特定的权限](/graph/api/resources/resourcespecificpermissiongrant?view=graph-rest-beta&preserve-view=true) ，列出有权访问指定的 [组或](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) 或 [权限的应用](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true)。

## <a name="march-2021-new-and-generally-available"></a>2021 年 3 月: 新版本和正式版

### <a name="applications"></a>应用程序
- 支持在 Azure AD 应用程序库中 [列出](/graph/api/applicationtemplate-list) 应用程序，并将此类应用程序的实例 [添加](/graph/api/applicationtemplate-instantiate) 到目录中的 [applicationTemplate](/graph/api/resources/applicationtemplate) 资源的 GA。
- 添加此类实例 `Application.ReadWrite.OwnedBy` 时 [仅](/graph/api/applicationtemplate-instantiate) 权限。
- 使用 [servicePrincipal](/graph/api/resources/serviceprincipal) 的 **signInAudience** 属性获取当前应用程序支持的用户帐户。

### <a name="devices-and-apps--cloud-printing"></a>设备和应用 | 云打印
- 适用于通用打印的 [云打印](universal-print-concept-overview.md) GA! 查看 [公告](https://techcommunity.microsoft.com/t5/windows-it-pro-blog/universal-print-is-ready-for-business/ba-p/2176778)，并查看如何 [开始使用通用打印](https://docs.microsoft.com/universal-print/fundamentals/universal-print-license)。
- 在 [打印任务定义](/graph/api/resources/printtaskdefinition)上[订阅更改通知](universal-print-webhook-notifications.md)或[打印机](/graph/api/resources/printer)资源。

### <a name="identity-and-access--governance"></a>身份和访问 | 治理
- 使用 Azure Active Directory （Azure AD） [许可请求](/graph/api/resources/consentrequests-root) 管理尝试访问需要管理员审批的应用的用户的请求工作流。 API 利用下列资源：
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
- 将用户的消息历史记录和数据从外部系统迁移到 Teams 频道，使用户能够顺畅地继续通信。 使用以下支持迁移方案的方法：
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
[创建自签名证书证书](/graph/api/servicePrincipal-addTokenSigningCertificate?view=graph-rest-beta&preserve-view=true) 添加到 SAML 应用程序。 借助此功能，允许 Azure AD 对 SAML 响应进行签名，帮助租户中启用 Azure AD 库应用单一登录。

### <a name="devices-and-apps--cloud-pc"></a>设备和应用 | 云电脑
添加到 [cloudPcDeviceImage](/graph/api/resources/cloudpcdeviceimage?view=graph-rest-beta&preserve-view=true) 资源之后，上传设备源映像失败再出现两个原因：操作系统不受支持 （`osVersionNotSupported`）， 或者预配 Windows 虚拟机 （`sourceImageInvalid`） 的源映像无效。

### <a name="devices-and-apps--cloud-printing"></a>设备和应用 | 云打印
当打印机与通用打印交互时，获取最近日期/时间 (**lastSeenDateTime** 属性)。

### <a name="devices-and-apps--corporate-management"></a>设备和应用 | 公司管理
Intune [3](https://developer.microsoft.com/graph/changelog/?from=2021-03-01&to=2021-03-31&filterBy=Corporate%20management) beta 版更新。

### <a name="identity-and-access--governance"></a>身份和访问 | 治理
将新模型 [访问权限审阅](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true) 组成员身份和所有其他支持的资源类型。 在 <a0/ [中弃用旧版 Access 审阅](/graph/api/resources/accessreviews-root?view=graph-rest-beta&preserve-view=true)。

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

### <a name="sites-and-lists--taxonomy"></a>网站和列表 | 分类
- 使用术语库 [关系](/graph/api/resources/site?view=graph-rest-beta&preserve-view=true)[termStore](/graph/api/resources/termstore-store?view=graph-rest-beta&preserve-view=true)导航到 **术语** 存储。
- 反之，则使用 **parentSiteId** 属性获取术语库的父站点的ID。

### <a name="users"></a>用户
- [通过](/graph/api/regionalandlanguagesettings-get?view=graph-rest-beta&preserve-view=true) 或 [更新](/graph/api/regionalandlanguagesettings-update?view=graph-rest-beta&preserve-view=true) 用户 [对翻译语言的偏好](/graph/api/resources/translationpreferences?view=graph-rest-beta&preserve-view=true)。 例如，是否翻译、自动翻译、或在翻译消息、聊天和网页中的特定语言之前提示，以及进行任何 [翻译覆盖](/graph/api/resources/translationlanguageoverride?view=graph-rest-beta&preserve-view=true)。
- [为用户激活](/graph/api/user-activateServicePlan?view=graph-rest-beta&preserve-view=true) 计划许可证。

## <a name="want-to-stay-in-the-loop"></a>保持循环

我们可以通过以下方式进行参与：

- 是否有希望 Microsoft Graph 支持的方案？ 在 [Microsoft 技术社区](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph)中建议新功能并进行投票。
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
