---
title: Microsoft Graph 新增功能
description: Microsoft Graph 新增功能
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: ae6cd9109faf46aa9ab2b55c0015f846f494a619
ms.sourcegitcommit: 5f643d3b3f71a9711963c8953da2188539fc9b0c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/14/2020
ms.locfileid: "41119782"
---
# <a name="whats-new-in-microsoft-graph"></a>Microsoft Graph 新增功能

查看 Microsoft Graph 中的新增功能要点，并查看你可如何[分享你的想法](#want-to-stay-in-the-loop)。 有关 API 更新的完整列表，请参阅 API 更改日志的 [12 月](changelog.md#december-2019)和 [11 月](changelog.md#november-2019)部分。 

> [!IMPORTANT]
> _预览_状态下的功能（包括 API 和工具）可能会发生更改，恕不另行通知，有些功能可能永远不会提升为正式发布 (GA) 状态。 不要在成品应用中使用预览功能。

## <a name="january-2020-new-and-generally-available"></a>2020 年 1 月：新版本和正式版

### <a name="security"></a>安全性
作为客户警报管理的一部分，请使用 [update alert](/graph/api/alert-update?view=graph-rest-1.0) 方法并将“**注释**”字段更新为 `Closed in IPC` 或 `Closed in MCAS`。

## <a name="december-2019-new-and-generally-available"></a>2019 年 12 月：新版本和正式版

### <a name="cloud-communications"></a>云通信
云通信 API 已正式发布，适用于[呼叫](/graph/api/resources/call?view=graph-rest-1.0)和[联机会议](/graph/api/resources/onlinemeeting?view=graph-rest-1.0)的 API [在 v1.0 中可用](/graph/api/resources/communications-api-overview?view=graph-rest-1.0)。

### <a name="education"></a>教育
使用 **classSettings** 属性管理课程专属设置，例如启用发送每周作业摘要的操作。 当团队表示[教育课程](/graph/api/resources/educationclass?view=graph-rest-1.0)时，此属性可在[团队](/graph/api/resources/team?view=graph-rest-1.0)资源中使用。

### <a name="identity-and-access"></a>标识和访问 
[尝试使用有限权限获取容器对象会返回部分数据](permissions-reference.md#limited-information-returned-for-inaccessible-member-objects)。 例如，与[用户](/graph/api/resources/user?view=graph-rest-1.0)、另一个**组**和[设备](/graph/api/resources/device?view=graph-rest-1.0)关联的[组](/graph/api/resources/group?view=graph-rest-1.0)实例。 只有 User.Read.All 和 Group.Read.All 权限且正在尝试访问此**组**实例的应用将获取**用户**和**组**实例，但获得的**设备**对象数据有限（仅限数据类型和对象 ID，不包括属性值）。

### <a name="people-and-workplace-intelligence"></a>人员和工作场所智能
见解 API 已正式发布。 在生产应用中使用此 API 确定具有以下特征的相关文档：

- 用户的[常用文档](/graph/api/insights-list-trending?view=graph-rest-1.0)
- 用户[使用的](/graph/api/insights-list-used?view=graph-rest-1.0)文档
- [与用户共享由用户共享的](/graph/api/insights-list-shared?view=graph-rest-1.0)文档

### <a name="reports"></a>报告
要使用用户委派的权限获取 Office 365 使用情况报告，管理员必须向该用户分配 Azure AD 受限管理员角色。 可以是以下角色之一：公司管理员、Exchange 管理员、SharePoint 管理员、Lync 管理员、全局读取者或报告读取者。 有关详细信息，请参阅[授权 API 读取 Office 365 使用情况报告](reportroot-authorization.md)。

### <a name="toolkit"></a>工具包
Microsoft Graph 工具包 v1.1 已发布。 有关增强功能和 bug 修复的列表，请参阅更改日历的[“2019 年 12 月”部分](changelog.md#december-2019)。

## <a name="december-2019-new-in-preview"></a>2019年12月：预览版新增功能

### <a name="cloud-communications"></a>云通信
- 使用新的[状态](/graph/api/resources/presence?view=graph-rest-beta)资源了解一名或多名用户的忙闲状态和当前活动。
- [删除](/graph/api/onlinemeeting-delete?view=graph-rest-beta)[联机会议](/graph/api/resources/onlinemeeting?view=graph-rest-beta)资源的实例。
- 要重命名和删除[呼叫](/graph/api/resources/call?view=graph-rest-beta)和[联机会议](/graph/api/resources/onlinemeeting?view=graph-rest-beta)资源的几个成员以便与这些资源的 v1 版本一致，请参阅更改日志的[“2019 年 12 月”部分](changelog.md#december-2019)。

### <a name="devices-and-apps"></a>设备和应用
Intune [12 月](changelog.md#december-2019)更新

### <a name="identity-and-access"></a>标识和访问 
- 修复了 [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta) 上 **appRoleAssignments** 和 **appRoleAssignedTo** 关系的行为。
- 使用 [Azure AD 权利管理](/graph/api/resources/entitlementmanagement-root?view=graph-rest-beta)中的 [accessPackageResourceRequest](/graph/api/resources/accesspackageresourcerequest?view=graph-rest-beta) 来请求将资源添加到 [目录](/graph/api/resources/accesspackagecatalog?view=graph-rest-beta)中，以便可在[访问包](/graph/api/resources/accesspackage?view=graph-rest-beta)中使用该资源的角色。
- 使用[威胁评估 API](/graph/api/resources/threatassessment-api-overview?view=graph-rest-beta) 帮助管理员报告可疑电子邮件、网络钓鱼 URL、电子邮件附件或其他文件。 然后，线程扫描判定会通知他们相应地调整组织策略。

### <a name="teamwork"></a>团队合作
- 针对[chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta)资源在 Microsoft 团队频道和聊天中[设置包含资源数据的更改通知](webhooks-with-resource-data.md)。
- 针对新的或已更改的[频道消息或聊天消息](/graph/api/resources/chatmessage?view=graph-rest-beta)[订阅通知](/graph/api/resources/subscription?view=graph-rest-beta)。
- 借助 [shiftPreferences](/graph/api/resources/shiftpreferences?view=graph-rest-beta) 资源，可在[日程安排](/graph/api/resources/schedule?view=graph-rest-beta)中将用户的忙线状态指定为“已分配排班”。 作为用户的[设置](/graph/api/resources/usersettings?view=graph-rest-beta)的一部分获取或设置此信息。


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

