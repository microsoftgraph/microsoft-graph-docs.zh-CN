---
title: 将 Microsoft Graph API 与 Microsoft Teams 结合使用
description: Microsoft Teams 是 Office 365 中基于聊天的工作区，可提供对特定于团队的日历、文件、OneNote 笔记、规划器计划等对象的内置访问权限。
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: ba27e303ab05e3a9ea3e02f3d0a32066e60c82a6
ms.sourcegitcommit: 624ac42e74533a9bf0d0d22b3b15adbb258fd594
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/05/2019
ms.locfileid: "34709381"
---
# <a name="use-the-microsoft-graph-api-to-work-with-microsoft-teams"></a>将 Microsoft Graph API 与 Microsoft Teams 结合使用

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Teams 是 Office 365 中基于聊天的工作区，可提供对特定于团队的日历、文件、OneNote 笔记、规划器计划、排班计划等对象的内置访问权限。 

## <a name="key-resources-in-microsoft-teams"></a>Microsoft Teams 中的重要资源

| 资源 | 方法 |
|:---------------|:--------|
|[团队](../resources/team.md)| [列出你的团队](../api/user-list-joinedteams.md)、[列出所有团队](/graph/teams-list-all-teams)、[创建](../api/team-put-teams.md)、[读取](../api/team-get.md)、[更新](../api/team-update.md)、[删除](/graph/api/group-delete?view=graph-rest-1.0)、[克隆](../api/team-clone.md)、[归档](../api/team-archive.md)[取消归档](../api/team-unarchive.md) |
|[组](../resources/group.md)| [添加成员](../api/group-post-members.md)、 [移除成员](../api/group-delete-members.md)、[添加所有者](../api/group-post-owners.md)、 [移除所有者](../api/group-delete-owners.md)、[获取文件](drive.md)、[获取笔记本](/graph/api/resources/notebook?view=graph-rest-1.0)、[获取计划](plannergroup.md)、[获取日历](event.md) |
|[频道](../resources/channel.md)|[列出](../api/channel-list.md)、[创建](../api/channel-post.md)、[读取](../api/channel-get.md)、[更新](../api/channel-patch.md)、[删除](../api/channel-delete.md)|
|[teamsTab](../resources/teamstab.md) |[列出](../api/teamstab-list.md)、[创建](../api/teamstab-add.md)、[读取](../api/teamstab-get.md)、[更新](../api/teamstab-update.md)、[删除](../api/teamstab-delete.md) |
|[teamsApp](../resources/teamsapp.md)|[列出](../api/teamsapp-list.md)、[发布](../api/teamsapp-publish.md)、[更新](../api/teamsapp-update.md)、[移除](../api/teamsapp-delete.md)|
|[teamsAppInstallation](../resources/teamsappinstallation.md)| [列出](../api/teamsappinstallation-list.md)、[安装](../api/teamsappinstallation-add.md)、[升级](../api/teamsappinstallation-delete.md)、[移除](../api/teamsappinstallation-delete.md) |
|[chatMessage](../resources/chatmessage.md)（预览）| [列出](../api/channel-list-messages.md)、[发送](../api/channel-post-messages.md)、[读取](/graph/api/channel-get-message?view=graph-rest-beta) |
|[调用](/graph/api/resources/call?view=graph-rest-beta)（预览） | [应答](/graph/api/call-answer?view=graph-rest-beta)、[拒绝](/graph/api/call-reject?view=graph-rest-beta)、[重定向](/graph/api/call-redirect?view=graph-rest-beta)、[静音](/graph/api/call-mute?view=graph-rest-beta)、[取消静音](/graph/api/call-unmute?view=graph-rest-beta)、[更新元数据](/graph/api/call-updatemetadata?view=graph-rest-beta)、[更改屏幕共享角色](/graph/api/call-changescreensharingrole?view=graph-rest-beta)、[列出参与者](/graph/api/call-list-participants?view=graph-rest-beta)、[邀请参与者](/graph/api/participant-invite?view=graph-rest-beta)、[将所有参与者设为静音](/graph/api/participant-muteall?view=graph-rest-beta) |
|[计划](/graph/api/resources/schedule?view=graph-rest-beta)（预览）| [创建或替换](/graph/api/team-put-schedule?view=graph-rest-beta)、[获取](/graph/api/schedule-get?view=graph-rest-beta)、[共享](/graph/api/schedule-share?view=graph-rest-beta) |
|[schedulingGroup](/graph/api/resources/schedulinggroup?view=graph-rest-beta)（预览）| [创建](/graph/api/schedule-post-schedulinggroups?view=graph-rest-beta)、[列出](/graph/api/schedule-list-schedulinggroups?view=graph-rest-beta)、[获取](/graph/api/schedulinggroup-get?view=graph-rest-beta)、[替换](/graph/api/schedulinggroup-put?view=graph-rest-beta)、[删除](/graph/api/schedulinggroup-delete?view=graph-rest-beta) |
|[排班](/graph/api/resources/shift?view=graph-rest-beta)（预览）| [创建](/graph/api/schedule-post-shifts?view=graph-rest-beta)、[列出](/graph/api/schedule-list-shifts?view=graph-rest-beta)、[获取](/graph/api/shift-get?view=graph-rest-beta)、[替换](/graph/api/shift-put?view=graph-rest-beta)、[删除](/graph/api/shift-delete?view=graph-rest-beta) |
|[timeOff](/graph/api/resources/timeoff?view=graph-rest-beta)（预览）| [创建](/graph/api/schedule-post-timesoff?view=graph-rest-beta)、[列出](/graph/api/schedule-list-timesoff?view=graph-rest-beta)、[获取](/graph/api/timeoff-get?view=graph-rest-beta)、[替换](/graph/api/timeoff-put?view=graph-rest-beta)、[删除](/graph/api/timeoff-delete?view=graph-rest-beta) |
|[timeOffReason](/graph/api/resources/timeoffreason?view=graph-rest-beta)（预览）| [创建](/graph/api/schedule-post-timeoffreasons?view=graph-rest-beta)、[列出](/graph/api/schedule-list-timeoffreasons?view=graph-rest-beta)、[获取](/graph/api/timeoffreason-get?view=graph-rest-beta)、[替换](/graph/api/timeoffreason-put?view=graph-rest-beta)、[删除](/graph/api/timeoffreason-delete?view=graph-rest-beta) |


## <a name="teams-and-groups"></a>用户和组

在 Microsoft Graph 中，Microsoft Teams 由[组](../resources/group.md)资源表示。 Microsoft Teams 和 Office 365 组均可满足组协作的各种需求。 几乎所有基于组的功能都适用于 Microsoft Teams 和 Office 365 组，例如组日历、文件、笔记、照片、计划等。 [团队](team.md)与 Office 365 组之间的主要区别在于成员之间的通信模式。 团队成员的通信方式是在特定团队的上下文中进行持久聊天。 Office 365 组成员通过组对话进行通信，它们是在 Outlook 的组上下文中发生的电子邮件对话。

具有团队的任何组都具有 **resourceProvisioningOptions** 属性，它包含“团队”。 

>**注释：** 可以更改 **Group.resourceProvisioningOptions** 属性。
请不要在该集合中添加或删除“团队”；否则，当你列出所有团队时，你将获得错误结果。

以下是团队和组之间的 API 级别的区别：

- 持久聊天仅适用于 Microsoft Teams。 此功能由[频道](../resources/channel.md)和 [chatMessage](../resources/chatmessage.md) 资源按层次结构表示。
- 组对话仅适用于 Office 365 组。 此功能由[对话](../resources/conversation.md)、[conversationThread](../resources/conversationthread.md) 和[帖子](../resources/post.md)资源按层次结构表示。 
- [列出加入的团队](../api/user-list-joinedteams.md)方法仅适用于 Microsoft Teams。
- [呼叫和在线会议 API](./calls-api-overview.md) 仅适用于 Microsoft Teams。
- 另请参阅[已知问题](/graph/known-issues)以了解这些 API。

>注意：如果在 Microsoft Teams 应用（而非独立应用中）使用组 API（例如，作为 Microsoft Teams 中运行的选项卡或自动程序的一部分），请按照在 Microsoft Teams 页面中使用 Microsoft Graph 一文中的说明操作。

## <a name="membership-changes-in-microsoft-teams"></a>Microsoft Teams 中的成员身份更改

若要向团队添加成员和所有者，请使用相同的 ID 更改[组](../resources/group.md)的成员身份。

| 用例      | 谓词      | URL |
| ------------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| [添加成员](../api/group-post-members.md)    | POST      | /groups/{id}/members/$ref  |
| [删除成员](../api/group-delete-members.md)   | DELETE    | /groups/{id}/members/{userId}/$ref |
| [添加所有者](../api/group-post-owners.md)     | POST       | /groups/{id}/owners/$ref |
| [移除所有者](../api/group-delete-owners.md) | DELETE    | /groups/{id}/owners/{userId}/$ref |
| [更新团队](../api/team-update.md)  | PATCH     | /teams/{id} |

我们建议你在添加所有者时，还将该用户添加为成员。 如果团队的所有者不是其成员，则所有权和成员身份更改可能不会立即显示在 Microsoft Teams 中。 此外，不同的应用程序和 API 将以不同的方式进行处理。 例如，Microsoft Teams 将显示用户是其成员或所有者的团队，而 Microsoft Teams PowerShell cmdlet 和 /me/joinedTeams API 仅显示用户是其成员的团队。 为了避免混淆，请也将全部所有者添加到成员列表中。 

已知问题：当调用 DELETE /groups/{id}/owners 时，也会从 /groups/{id}/members list 中移除用户。 若要解决此问题，我们建议你从所有者和成员中移除用户，等待 10 秒后，将其添加回成员。

在添加和移除成员和所有者时，请勿在 ID 两边添加大括号 { }。

| 速度 | 语法 | 
| ------ | ----- |
| 快速 | https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/members/48d31887-5fad-4d73-a9f5-3c356e68a038/$ref | 
| 慢速 | https://graph.microsoft.com/beta/groups/{02bd9fd6-8f93-4758-87c3-1fb73740a315}/members/{48d31887-5fad-4d73-a9f5-3c356e68a038}/$ref | 

同样，如果 URL 或有效负载中的 `userId` 显示为 UPN 而不是 GUID，则性能会变慢。

| 速度 | 语法 | 
| ------ | ----- |
| 快速 | 48d31887-5fad-4d73-a9f5-3c356e68a038 | 
| 慢速 | john@example.com | 

当采用较慢的路径时，如果当前团队成员或所有者登录到 Microsoft Teams 应用程序/网站，则更改将在一小时内反映出来。
如果这些用户都未登录到 Microsoft Teams 应用程序/网站，则更改将在其中一个用户登录后一小时内反映出来。

## <a name="see-also"></a>另请参阅

[Microsoft Teams API 概述](/graph/teams-concept-overview)
