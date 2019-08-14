---
title: Microsoft Graph 新增功能
description: Microsoft Graph 新增功能
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 2e2c608cf05f22ccf9e296520624d7c96fe2b4ce
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36367104"
---
# <a name="whats-new-in-microsoft-graph"></a>Microsoft Graph 新增功能

你是否知道 Microsoft Graph 中的一些新功能来源于开发人员社区的热门请求？ 

Microsoft Graph 团队会定期评估客户需求，并按以下顺序发布新功能：

1. 处于**_预览_** 状态的 Debut。 任何相关的 REST API 更新都在 beta 终结点 (`https://graph.microsoft.com/beta`) 中。  

2. 如果有足够的反馈表明具有可行性，则提升为 **_正式发布_ (GA)** 状态。 任何相关的 REST API 更新都添加到 v1.0 终结点 (`https://graph.microsoft.com/v1.0`)。 

在下面查看 Microsoft Graph 中新增功能要点，并查看你可如何[分享你的想法](#want-to-stay-in-the-loop)。 有关 API 更新的详细信息，请参阅 API 更改日志的[八月](changelog.md#august-2019)、[六月](changelog.md#july-2019)部分。 


## <a name="july-2019-new-and-generally-available"></a>2019 年 7 月：新版本和正式发布版 

### <a name="example-code-snippets"></a>代码片段示例
现在 v1.0 和 beta 参考中的所有 API 主题中提供了 Objective-C 代码片段。 请参阅[获取事件](/graph/api/event-get?view=graph-rest-1.0&tabs=objective-c#example)的 Objective-C 示例。

### <a name="group"></a>组
- 使用 [validateProperties](/graph/api/group-validateproperties?view=graph-rest-1.0) 函数确保现有 Office 365 组的显示名称和邮件昵称符合命名策略。
- 或者，在创建组之前，可以为 [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0) 使用 [validateProperties](/graph/api/directoryobject-validateproperties?view=graph-rest-1.0) 函数来首先验证名称。

### <a name="identity-and-access"></a>身份和访问
- 使用[新的委派和应用程序权限](permissions-reference.md#organization-permissions)、_Organization.Read.All_ 和 _Organization.ReadWrite.All_ 来访问[组织](/graph/api/resources/organization?view=graph-rest-1.0)和相关资源，例如[订阅的 SKU](/graph/api/resources/subscribedsku?view=graph-rest-1.0)。
- 使用[新的委派和应用程序权限](permissions-reference.md#role-management-permissions)、_RoleManagement.Read.Directory_ 和 _RoleManagement.ReadWrite.Directory_，对于公司目录中的与角色的访问控制 (RBAC)：

  - 使用读取/写入权限来首先[激活](/graph/api/directoryrole-post-directoryroles?view=graph-rest-1.0)目录角色。 
  - 激活角色之后，可以使用读取权限来[读取目录角色](/graph/api/directoryrole-list?view=graph-rest-1.0)、[列出角色成员](/graph/api/directoryrole-list-members?view=graph-rest-1.0)和[列出目录角色模板](/graph/api/directoryroletemplate-list?view=graph-rest-1.0)。 
  - 还可以使用读取/写入权限来[添加](/graph/api/directoryrole-post-members?view=graph-rest-1.0)和[删除](/graph/api/directoryrole-delete-member?view=graph-rest-1.0)角色成员。


## <a name="july-2019-new-in-preview"></a>2019 年 7 月：预览版新增功能

> [!IMPORTANT]
> _预览_状态下的功能（包括 API 和工具）可能会发生更改，恕不另行通知，有些功能可能永远不会提升为 GA 状态。 请不要在生产应用中使用它们。

### <a name="calendar"></a>日历 
按照 Exchange Online 管理员的设置，使用新的[位置 API](/graph/api/resources/place?view=graph-rest-beta) 来使用诸如 [room](/graph/api/resources/room?view=graph-rest-beta) 和 [room list](/graph/api/resources/roomlist?view=graph-rest-beta) 之类的富位置类型。

### <a name="devices-and-apps"></a>设备和应用
Intune [7 月](changelog.md#july-2019)更新

### <a name="files"></a>文件 
在为文件、文件夹或其他 [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) [创建共享链接](/graph/api/driveitem-createlink?view=graph-rest-beta)时，应用到期日期/时间或密码。

### <a name="identity-and-access"></a>标识和访问
- 使用[新的应用程序权限](/graph/permissions-reference?#accessreviews-permissions) _AccessReview.ReadWrite.Membership_ 对[访问权限审阅](/graph/api/resources/accessreviews-root?view=graph-rest-beta)执行 CRUD 操作。 
- 使用[新的委派和应用程序权限](permissions-reference.md#administrative-units-permissions)、_AdministrativeUnit.Read.All_ 和 _AdministrativeUnit.ReadWrite.All_，以分别读取或写入（包括创建、更新、删除或管理成员身份）[管理单元](/graph/api/resources/administrativeunit?view=graph-rest-beta)资源。
- 使用[新的委派和应用程序权限](permissions-reference.md#organization-permissions)、_Organization.Read.All_ 和 _Organization.ReadWrite.All_ 来访问[组织](/graph/api/resources/organization?view=graph-rest-beta)和相关资源，例如[订阅的 SKU](/graph/api/resources/subscribedsku?view=graph-rest-beta)。
- 使用新的 [discover](/graph/api/directorydefinition-discover?view=graph-rest-beta) 函数查找最新的目录[同步架构](/graph/api/resources/synchronization-synchronizationschema?view=graph-rest-beta)，以便将目录对象、属性及类型同步到应用。
- 使用[功能推出策略](/graph/api/resources/featureRolloutPolicy?view=graph-rest-beta)帮助租户管理员在为整个组织启用一些功能之前，针对特定组试用这些功能。

### <a name="mail"></a>邮件
使用更精确的应用程序权限 _Mail.ReadBasic.All_ 来读取用户邮箱（邮件正文除外）、预览正文、附件和扩展属性，不包括搜索邮箱。 现适用于 [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-beta) 以及针对[邮件](/graph/api/resources/message?view=graph-rest-beta) 和 **mailFolder** 的[更改跟踪](delta-query-overview.md)

### <a name="reports"></a>报告
- 获取与已删除的项目计数和大小相关的其他[邮箱使用情况数据](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-beta)。

### <a name="teamwork"></a>团队合作
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

