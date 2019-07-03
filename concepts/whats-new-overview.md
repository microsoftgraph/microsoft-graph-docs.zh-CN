---
title: Microsoft Graph 新增功能
description: Microsoft Graph 新增功能
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 416ba84527957b59ad4f8ff9e6d8c0194d60f245
ms.sourcegitcommit: ee710ff556f4a7907181df5c323e345f52808ce2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35420427"
---
# <a name="whats-new-in-microsoft-graph"></a>Microsoft Graph 新增功能

你是否知道 Microsoft Graph 中的一些新功能源于开发人员社区的热门请求？ 

我们来介绍新功能的典型生命周期、Microsoft Graph 中当前新增的功能以及[共享创意](#want-to-stay-in-the-loop)的方式。

## <a name="life-cycle-of-a-feature"></a>功能的生命周期

Microsoft Graph 服务所有者会定期评估功能创意和客户需求, 并选择要支持的新方案。 若要构建新功能, 可以添加或更新 REST API。 它们可以保留相同的 API 语法并扩展功能行为。 或者, 它们可以提供更好的学习或开发体验。

在大多数情况下, 服务所有者将按照以下顺序发布新功能:

1. **_预览_** 状态下的 Debut, 这意味着功能行为可能会随之更改, 恕不另行通知。 所有者将在 beta 端点 (`https://graph.microsoft.com/beta`) 中公开任何相关的 REST API 添加或更新。 不要在成品应用中使用预览功能, 包括其 API。

2. 如果服务所有者收到了足够的反馈, 并且认为该功能切实可行, 则所有者会将该功能升级到**_常规可用性_ (GA)** 状态。 所有者也将任何相关 API 的添加或更新添加到 v 1.0 终结点 (`https://graph.microsoft.com/v1.0`)。 可在成品应用中使用 GA 状态中的功能（包括其 API）。

以下各节介绍了2019年5月和6月的新增功能。 有关 API 更新的详细信息, 请参阅 changelog 的[5月](changelog.md#may-2019)和[6月](changelog.md#june-2019)部分。 

## <a name="new-and-generally-available-released-may---june-2019"></a>新增及常用功能（2019年5月 - 6月发布）

### <a name="calendar-mail-and-personal-contacts"></a>"日历"、"邮件" 和 "个人联系人"
Exchange 管理员可以向应用程序授予应用程序权限, 并[限制该应用仅访问](auth-limit-mailbox-access.md)中的邮箱子集, 而不是默认的访问组织中的所有邮箱。 此类受限访问适用于授予[日历](permissions-reference.md#calendars-permissions)、 [联系人](permissions-reference.md#contacts-permissions)及[邮件和邮箱设置](permissions-reference.md#mail-permissions)的应用的任何应用程序权限。 查看相关的[博客公告](https://developer.microsoft.com/en-us/graph/blogs/scoping-microsoft-graph-application-permissions-to-specific-exchange-online-mailboxes/)。

### <a name="example-code-snippets"></a>代码段示例
除了 C# 和 JavaScript 之外 , v 1.0 和 beta 参考中的所有 API 主题中现在有 Objective-C 代码段。 请参阅[获取事件](/graph/api/event-get?view=graph-rest-1.0&tabs=objective-c#example)的 Objective-C 示例。

### <a name="mail"></a>邮件
使用[邮件搜索文件夹](/graph/api/resources/mailsearchfolder?view=graph-rest-1.0) API 来搜索邮件, 并访问 Outlook 电子邮件搜索结果。 查看相关的[博客公告](https://developer.microsoft.com/en-us/graph/blogs/mail-search-folder-support-for-microsoft-graph-apis/)。

### <a name="postman"></a>Postman
除 Graph 资源管理器外, 请在[Microsoft Graph Postman 集合](use-postman.md)中试用 Microsoft Graph API, 了解 API 行为并加速应用程序开发。

### <a name="tutorials"></a>教程
尝试使用新[教程构建 Java 控制台应用](/graph/tutorials/java) , 以获取有关用户日历的信息。

### <a name="user"></a>用户
管理员或用户可以[吊销](/graph/api/user-revokesigninsessions?view=graph-rest-1.0)用户的所有已颁发的刷新令牌。 通常用于防止已丢失或被盗设备上的应用访问组织的数据。


## <a name="new-in-preview-released-may---june-2019"></a>预览版中的新增功能（2019年5月 - 6月发布）

> [!IMPORTANT]
> _预览_状态中的功能 (包括 API 和工具) 可能会随之更改, 而不会另行通知, 有些可能从未升级到 GA 状态。 请不要在成品应用中使用它们。

### <a name="devices-and-apps"></a>设备和应用
- Intune [5月](changelog.md#may-2019)更新 
- Intune [6月](changelog.md#june-2019)更新

### <a name="education"></a>教育
- [educationSchool](/graph/api/resources/educationschool?view=graph-rest-beta)的增量查询。
- [educationClass](/graph/api/resources/educationclass?view=graph-rest-beta) 和 [educationUser](/graph/api/resources/educationuser?view=graph-rest-beta)的增量查询和属性添加。 

### <a name="group"></a>组
获取[敏感度标签](/graph/api/resources/assignedlabel?view=graph-rest-beta) , 帮助保护 Office 365 组的敏感数据并满足合规性策略。 这些标签是[assignedLabel](/graph/api/resources/assignedlabel?view=graph-rest-beta)对象，由 Microsoft 365 安全与合规性中心的管理员发布，作为 Microsoft 信息保护功能的一部分。 

### <a name="identity-and-access"></a>身份和访问控制
- 获取[应用程序](/graph/api/resources/applicationtemplate?view=graph-rest-beta)的实例, 或将 Azure AD 应用程序库中的实例作为模板添加到目录中。
- 获取租户中所有[预配事件](/graph/api/resources/provisioningobjectsummary?view=graph-rest-beta)的列表。
- 获取有关 Azure AD 环境中[检测到的用户或登录风险](/graph/api/resources/riskdetection?view=graph-rest-beta)的信息。 此风险检测功能是 Azure AD 标识保护的一部分。

### <a name="mail"></a>邮件
在 [mailFolder](permissions-reference.md#mail-permissions) API 中以及[邮件](/graph/api/resources/mailfolder?view=graph-rest-beta)和 [mailFolder](webhooks.md)的[更改通知](/graph/api/resources/message?view=graph-rest-beta)中使用 **Mail.ReadBasic 权限**。

### <a name="microsoft-graph-toolkit"></a>Microsoft 图形工具包
[Microsoft Graph 工具包](/graph/toolkit/overview)是一组框架不可知的 web 组件和帮助器, 提供对 Microsoft Graph 中的数据进行身份验证和访问的便利。  由于 Microsoft Graph 工具包处于预览状态, 请仅在非成品应用中使用工具包提供的程序和组件。

### <a name="sites"></a>网站
让用户[关注](/graph/api/site-follow?view=graph-rest-beta)或[取消关注](/graph/api/site-unfollow?view=graph-rest-beta) SharePoint 网站。

### <a name="teamwork"></a>团队合作
在 Microsoft 团队[聊天消息](/graph/api/resources/chatmessagehostedimage?view=graph-rest-beta)中存储[图像](/graph/api/resources/chatmessage?view=graph-rest-beta)。 
支持[配置](/graph/api/resources/teamdiscoverysettings?view=graph-rest-beta)私人团队的发现方式。


## <a name="want-to-stay-in-the-loop"></a>保持循环
- 是否有希望 Microsoft Graph 支持的方案？ 在 [Microsoft Graph 用户心声](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)中建议新功能并进行投票。
- 成为 Microsoft Graph 社区中的活跃成员! [参与](https://aka.ms/microsoftgraphcall)Microsoft Graph 社区每月通话。
- 注册 [office 365 开发人员计划](https://developer.microsoft.com/zh-CN/office/dev-program)，免费订阅 Office 365, 然后开始开发! 


## <a name="see-also"></a>另请参阅
- 定期查看 [Microsoft Graph 开发人员博客](https://developer.microsoft.com/en-us/graph/blogs/), 了解发布公告和有帮助的资源。 
- 浏览 Microsoft Graph API 新增功能的详细信息, 以及[changelog](changelog.md)中的 API 行为更新。
- 查找[早期版本的重点内容](whats-new-earlier.md)。
- 了解有关 [Microsoft Graph 的版本控制、支持和中断性变更策略](versioning-and-support.md)。

