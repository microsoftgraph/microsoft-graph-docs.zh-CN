---
title: Microsoft Graph 新增功能
description: Microsoft Graph 新增功能
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 5a69232c58469f09e953af9e9d06667509a76568
ms.sourcegitcommit: a700f1c283a5d847cd1697e26bcd47bc8625384e
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/01/2019
ms.locfileid: "36049615"
---
# <a name="whats-new-in-microsoft-graph"></a>Microsoft Graph 新增功能

你是否知道 Microsoft Graph 中的一些新功能来源于开发人员社区的热门请求？ 

Microsoft Graph 团队会定期评估客户需求，并按以下顺序发布新功能：

1. 处于**_预览_** 状态的 Debut。 任何相关的 REST API 更新都处于 beta 终结点 (`https://graph.microsoft.com/beta`) 中。 预览版中的功能可能会发生更改，恕不另行通知。 请不要在生产应用中使用它们。 

2. 如果有足够的反馈表明具有可行性，则提升为 **_正式发布_ (GA)** 状态。 任何相关的 REST API 更新都添加到 v1.0 终结点 (`https://graph.microsoft.com/v1.0`)。 仅在生产应用中使用具有 GA 状态的功能。

让我们来看看 Microsoft Graph 中的最新动态，以及如何[分享你的想法](#want-to-stay-in-the-loop)。 有关 API 更新的详细信息，请参阅更改日志的[五月](changelog.md#may-2019)、[六月](changelog.md#june-2019)和[七月](changelog.md#july-2019)部分。 

## <a name="new-and-generally-available-released-may---july-2019"></a>新增及常用功能（2019 年 5 月 - 7 月发布）

### <a name="calendar-mail-and-personal-contacts"></a>日历、邮件和个人联系人
Exchange 管理员可以向应用程序授予应用程序权限, 并[限制该应用仅访问邮箱 ](auth-limit-mailbox-access.md) 的子集, 而不是默认的访问组织中的所有邮箱。 此类受限访问适用于授予[日历](permissions-reference.md#calendars-permissions)、 [联系人](permissions-reference.md#contacts-permissions)及[邮件和邮箱设置](permissions-reference.md#mail-permissions)的应用的任何应用程序权限。 查看相关的[博客公告](https://developer.microsoft.com/en-us/graph/blogs/scoping-microsoft-graph-application-permissions-to-specific-exchange-online-mailboxes/)。

### <a name="example-code-snippets"></a>代码段示例
除了 C# 和 JavaScript 之外 , v 1.0 和 beta 参考中的所有 API 主题中现在有 Objective-C 代码段。 请参阅[获取事件](/graph/api/event-get?view=graph-rest-1.0&tabs=objective-c#example)的 Objective-C 示例。

### <a name="group"></a>组
- 使用 [validateProperties](/graph/api/group-validateproperties?view=graph-rest-1.0) 函数确保现有 Office 365 组的显示名称和邮件昵称符合命名策略。
- 或者，在创建组之前，可以为 [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0) 使用 [validateProperties](/graph/api/directoryobject-validateproperties?view=graph-rest-1.0) 函数来首先验证名称。

### <a name="identity-and-access"></a>身份和访问
- 使用[新的委派和应用程序权限](permissions-reference.md#organization-permissions)、_Organization.Read.All_ 和 _Organization.ReadWrite.All_ 来访问[组织](/graph/api/resources/organization?view=graph-rest-1.0)和相关资源，例如[订阅的 SKU](/graph/api/resources/subscribedsku?view=graph-rest-1.0)。
- 使用[新的委派和应用程序权限](permissions-reference.md#role-management-permissions)、_RoleManagement.Read.Directory_ 和 _RoleManagement.ReadWrite.Directory_，对于公司目录中的与角色的访问控制 (RBAC)：

  - 使用读取/写入权限来首先[激活](/graph/api/directoryrole-post-directoryroles?view=graph-rest-1.0)目录角色。 
  - 激活角色之后，可以使用读取权限来[读取目录角色](/graph/api/directoryrole-list?view=graph-rest-1.0)、[列出角色成员](/graph/api/directoryrole-list-members?view=graph-rest-1.0)和[列出目录角色模板](/graph/api/directoryroletemplate-list?view=graph-rest-1.0)。 
  - 还可以使用读取/写入权限来[添加](/graph/api/directoryrole-post-members?view=graph-rest-1.0)和[删除](/graph/api/directoryrole-delete-member?view=graph-rest-1.0)角色成员。 

### <a name="mail"></a>邮件
使用[邮件搜索文件夹](/graph/api/resources/mailsearchfolder?view=graph-rest-1.0) API 来搜索邮件, 并访问 Outlook 电子邮件搜索结果。 查看相关的[博客公告](https://developer.microsoft.com/en-us/graph/blogs/mail-search-folder-support-for-microsoft-graph-apis/)。

### <a name="postman"></a>Postman
除 Graph 资源管理器外, 请在[Microsoft Graph Postman 集合](use-postman.md)中试用 Microsoft Graph API, 了解 API 行为并加速应用程序开发。

### <a name="tutorials"></a>教程
尝试使用新[教程构建 Java 控制台应用](/graph/tutorials/java) , 以获取有关用户日历的信息。

### <a name="user"></a>用户
管理员或用户可以[吊销](/graph/api/user-revokesigninsessions?view=graph-rest-1.0)用户的所有已颁发的刷新令牌。 通常用于防止已丢失或被盗设备上的应用访问组织的数据。


## <a name="new-in-preview-released-may---july-2019"></a>预览版中的新增功能（2019 年 5 月 - 7 月发布）

> [!IMPORTANT]
> _预览_状态下的功能（包括 API 和工具）可能会发生更改，恕不另行通知，有些功能可能永远不会提升为 GA 状态。 请不要在生产应用中使用它们。

### <a name="calendar"></a>日历 
按照 Exchange Online 管理员的设置，使用新的[位置 API](/graph/api/resources/place?view=graph-rest-beta) 来使用诸如 [room](/graph/api/resources/room?view=graph-rest-beta) 和 [room list](/graph/api/resources/roomlist?view=graph-rest-beta) 之类的富位置类型。

### <a name="devices-and-apps"></a>设备和应用
- Intune [5月](changelog.md#may-2019)更新 
- Intune [6 月](changelog.md#june-2019)更新
- Intune [7 月](changelog.md#july-2019)更新

### <a name="education"></a>教育
- [educationSchool](/graph/api/resources/educationschool?view=graph-rest-beta)的增量查询。
- [educationClass](/graph/api/resources/educationclass?view=graph-rest-beta) 和 [educationUser](/graph/api/resources/educationuser?view=graph-rest-beta)的增量查询和属性添加。

### <a name="files"></a>文件 
在为文件、文件夹或其他 [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) [创建共享链接](/graph/api/driveitem-createlink?view=graph-rest-beta)时，应用到期日期/时间或密码。

### <a name="group"></a>组
获取[敏感度标签](/graph/api/resources/assignedlabel?view=graph-rest-beta) , 帮助保护 Office 365 组的敏感数据并满足合规性策略。 这些标签是[assignedLabel](/graph/api/resources/assignedlabel?view=graph-rest-beta)对象，由 Microsoft 365 安全与合规性中心的管理员发布，作为 Microsoft 信息保护功能的一部分。 

### <a name="identity-and-access"></a>身份和访问控制
- 获取[应用程序](/graph/api/resources/applicationtemplate?view=graph-rest-beta)的实例，或将 Azure AD 应用程序库中的实例作为模板添加到目录中。
- 获取租户中所有[预配事件](/graph/api/resources/provisioningobjectsummary?view=graph-rest-beta)目录的列表。
- 使用新的 [discover](/graph/api/directorydefinition-discover?view=graph-rest-beta) 函数查找最新的目录[同步架构](/graph/api/resources/synchronization-synchronizationschema?view=graph-rest-beta)，以便将目录对象、属性及类型同步到应用。
- 获取有关 Azure AD 环境中[检测到的用户或登录风险](/graph/api/resources/riskdetection?view=graph-rest-beta)的信息。 此风险检测功能是 Azure AD 标识保护的一部分。
- 使用[新的委派和应用程序权限](permissions-reference.md#administrative-units-permissions)、_AdministrativeUnit.Read.All_ 和 _AdministrativeUnit.ReadWrite.All_，以分别读取或写入（包括创建、更新、删除或管理成员身份）[管理单元](/graph/api/resources/administrativeunit?view=graph-rest-beta)资源。
- 使用[新的委派和应用程序权限](permissions-reference.md#organization-permissions)、_Organization.Read.All_ 和 _Organization.ReadWrite.All_ 来访问[组织](/graph/api/resources/organization?view=graph-rest-beta)和相关资源，例如[订阅的 SKU](/graph/api/resources/subscribedsku?view=graph-rest-beta)。

### <a name="mail"></a>邮件
使用更精确的委派权限、_Mail.ReadBasic_ 和应用程序权限 _Mail.ReadBasic.All_ 来读取用户邮箱（邮件正文除外）、预览正文、附件和扩展属性，不包括搜索邮箱。 先前适用于[列出](/graph/api/user-list-messages?view=graph-rest-beta)和[获取](/graph/api/message-get?view=graph-rest-beta)邮件，现在也适用于 [message](/graph/api/resources/message?view=graph-rest-beta) 和 **mailFolder** 的 [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-beta) 和 [change notifications](webhooks.md)。

### <a name="microsoft-graph-toolkit"></a>Microsoft Graph 工具包
[Microsoft Graph 工具包](/graph/toolkit/overview)是一组框架不可知的 web 组件和帮助器, 提供对 Microsoft Graph 中的数据进行身份验证和访问的便利。  由于 Microsoft Graph 工具包处于预览状态，请仅在非生产应用中使用工具包提供程序和组件。

### <a name="reports"></a>报告
- 获取组织中用户采用的[身份验证方法的报告](/graph/api/resources/authenticationmethods-usage-insights-overview?view=graph-rest-beta)，例如自助服务密码重置和多因素身份验证 (MFA).。
- 获取与已删除的项目计数和大小相关的其他[邮箱使用情况数据](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-beta)。

### <a name="sites"></a>网站
让用户[关注](/graph/api/site-follow?view=graph-rest-beta)或[取消关注](/graph/api/site-unfollow?view=graph-rest-beta) SharePoint 网站。

### <a name="teamwork"></a>团队合作
- 在 Microsoft 团队[聊天消息](/graph/api/resources/chatmessagehostedimage?view=graph-rest-beta)中存储[图像](/graph/api/resources/chatmessage?view=graph-rest-beta)。 
- 支持[配置](/graph/api/resources/teamdiscoverysettings?view=graph-rest-beta)私人团队的发现方式。
- 为用户[安装](/graph/api/user-add-teamsappinstallation?view=graph-rest-beta)、[卸载](/graph/api/user-delete-teamsappinstallation?view=graph-rest-beta)、[升级](/graph/api/user-upgrade-teamsappinstallation?view=graph-rest-beta)和[列出已安装的 Microsoft Teams 应用](/graph/api/user-list-teamsappinstallation?view=graph-rest-beta)。
- 使用仅应用访问权限来读取频道消息、频道消息回复以及聊天中的消息。 [请求和批准](teams-protected-apis.md)此类访问。


## <a name="want-to-stay-in-the-loop"></a>保持循环
- 是否有希望 Microsoft Graph 支持的方案？ 在 [Microsoft Graph 用户心声](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)中建议新功能并进行投票。
- 成为 Microsoft Graph 社区中的活跃成员! [参与](https://aka.ms/microsoftgraphcall)Microsoft Graph 社区每月通话。
- 注册 [office 365 开发人员计划](https://developer.microsoft.com/zh-CN/office/dev-program)，免费订阅 Office 365, 然后开始开发! 


## <a name="see-also"></a>另请参阅
- 定期查看 [Microsoft Graph 开发人员博客](https://developer.microsoft.com/en-us/graph/blogs/), 了解发布公告和有帮助的资源。 
- 浏览 Microsoft Graph API 新增功能的详细信息, 以及[changelog](changelog.md)中的 API 行为更新。
- 查找[早期版本的重点内容](whats-new-earlier.md)。
- 了解有关 [Microsoft Graph 的版本控制、支持和中断性变更策略](versioning-and-support.md)。

