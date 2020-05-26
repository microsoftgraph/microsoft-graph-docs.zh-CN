---
title: 将 Microsoft Graph API 与 Microsoft Teams 结合使用
description: Microsoft Teams 是 Office 365 中基于聊天的工作区，可提供对特定于团队的日历、文件、OneNote 笔记、规划器计划等对象的内置访问权限。
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
doc_type: conceptualPageType
ms.openlocfilehash: 34f5186e9933f5edcd8a91b1cb95b21b6deb4a50
ms.sourcegitcommit: ef9e0fd8fb6047fa9272e98310eaed2c4e0a2660
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/23/2020
ms.locfileid: "44353901"
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
|[调用](/graph/api/resources/communications-api-overview.md)（预览） | [应答](/graph/api/call-answer?view=graph-rest-beta)、[拒绝](/graph/api/call-reject?view=graph-rest-beta)、[重定向](/graph/api/call-redirect?view=graph-rest-beta)、[静音](/graph/api/call-mute?view=graph-rest-beta)、[取消静音](/graph/api/call-unmute?view=graph-rest-beta)、[更新元数据](/graph/api/call-updatemetadata?view=graph-rest-beta)、[更改屏幕共享角色](/graph/api/call-changescreensharingrole?view=graph-rest-beta)、[列出参与者](/graph/api/call-list-participants?view=graph-rest-beta)、[邀请参与者](/graph/api/participant-invite?view=graph-rest-beta)、[将所有参与者设为静音](/graph/api/participant-muteall?view=graph-rest-beta) |
|[计划](/graph/api/resources/schedule?view=graph-rest-beta)（预览）| [创建或替换](/graph/api/team-put-schedule?view=graph-rest-beta)、[获取](/graph/api/schedule-get?view=graph-rest-beta)、[共享](/graph/api/schedule-share?view=graph-rest-beta) |
|[schedulingGroup](/graph/api/resources/schedulinggroup?view=graph-rest-beta)（预览）| [创建](/graph/api/schedule-post-schedulinggroups?view=graph-rest-beta)、[列出](/graph/api/schedule-list-schedulinggroups?view=graph-rest-beta)、[获取](/graph/api/schedulinggroup-get?view=graph-rest-beta)、[替换](/graph/api/schedulinggroup-put?view=graph-rest-beta)、[删除](/graph/api/schedulinggroup-delete?view=graph-rest-beta) |
|[排班](/graph/api/resources/shift?view=graph-rest-beta)（预览）| [创建](/graph/api/schedule-post-shifts?view=graph-rest-beta)、[列出](/graph/api/schedule-list-shifts?view=graph-rest-beta)、[获取](/graph/api/shift-get?view=graph-rest-beta)、[替换](/graph/api/shift-put?view=graph-rest-beta)、[删除](/graph/api/shift-delete?view=graph-rest-beta) |
|[timeOff](/graph/api/resources/timeoff?view=graph-rest-beta)（预览）| [创建](/graph/api/schedule-post-timesoff?view=graph-rest-beta)、[列出](/graph/api/schedule-list-timesoff?view=graph-rest-beta)、[获取](/graph/api/timeoff-get?view=graph-rest-beta)、[替换](/graph/api/timeoff-put?view=graph-rest-beta)、[删除](/graph/api/timeoff-delete?view=graph-rest-beta) |
|[timeOffReason](/graph/api/resources/timeoffreason?view=graph-rest-beta)（预览）| [创建](/graph/api/schedule-post-timeoffreasons?view=graph-rest-beta)、[列出](/graph/api/schedule-list-timeoffreasons?view=graph-rest-beta)、[获取](/graph/api/timeoffreason-get?view=graph-rest-beta)、[替换](/graph/api/timeoffreason-put?view=graph-rest-beta)、[删除](/graph/api/timeoffreason-delete?view=graph-rest-beta) |

## <a name="microsoft-teams-limits"></a>Microsoft Teams 限制

Microsoft Teams 的已测试性能和容量限制将记录在 [Microsoft Teams 限制和规范](/microsoftteams/limits-specifications-teams)中。
无论是直接使用 Microsoft Teams 还是使用 Microsoft Graph API，这些限制均适用。
由于每个团队都有一个对应的组，并且每个组都是一个目录对象，因此对[组数](/microsoft-365/admin/create-groups/office-365-groups#group-limits)和[目录对象数目（“资源”）](/azure/active-directory/users-groups-roles/directory-service-limits-restrictions) 的限制也可以发挥作用。 

频道内的文件存储在 SharePoint 中；[SharePoint online 限制](/office365/servicedescriptions/sharepoint-online-service-description/sharepoint-online-limits)适用。

另请参阅 [Microsoft Teams 服务限制](/graph/throttling)。

## <a name="teams-and-groups"></a>用户和组

在 Microsoft Graph 中，Microsoft Teams 由[组](../resources/group.md)资源表示。 Microsoft Teams 和 Office 365 组均可满足组协作的各种需求。 几乎所有基于组的功能都适用于 Microsoft Teams 和 Office 365 组，例如组日历、文件、笔记、照片、计划等。 [团队](team.md)与 Office 365 组之间的主要区别在于成员之间的通信模式。 团队成员的通信方式是在特定团队的上下文中进行持久聊天。 Office 365 组成员通过组对话进行通信，它们是在 Outlook 的组上下文中发生的电子邮件对话。

具有团队的任何组都具有 **resourceProvisioningOptions** 属性，它包含“团队”。

>**注释：** 可以更改 **Group.resourceProvisioningOptions** 属性。
请不要在该集合中添加或删除“团队”；否则，当你列出所有团队时，你将获得错误结果。

以下是团队和组之间的 API 级别的区别：

- 持久聊天仅适用于 Microsoft Teams。 此功能由[频道](../resources/channel.md)和 [chatMessage](../resources/chatmessage.md) 资源按层次结构表示。
- 组对话仅适用于 Office 365 组。 此功能由[对话](../resources/conversation.md)、[conversationThread](../resources/conversationthread.md) 和[帖子](../resources/post.md)资源按层次结构表示。
- [列出加入的团队](../api/user-list-joinedteams.md)方法仅适用于 Microsoft Teams。
- [呼叫和在线会议 API](./communications-api-overview.md) 仅适用于 Microsoft Teams。
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

我们建议你在添加所有者时，还将该用户添加为成员。
如果团队的所有者不是其成员，则所有权和成员身份更改可能不会立即显示在 Microsoft Teams 中。
此外，不同的应用程序和 API 将以不同的方式进行处理。
例如，Microsoft Teams 将显示用户是其成员或所有者的团队，而 Microsoft Teams PowerShell cmdlet 和 /me/joinedTeams API 仅显示用户是其成员的团队。
为了避免混淆，请也将全部所有者添加到成员列表中。

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

> [!Note]
> 租户来宾始终通过慢速路径进行处理。

## <a name="polling-requirements"></a>轮询要求

如果应用程序轮询查看是否更改了某资源，则此操作每天只能执行一次。 （[teamsAsyncOperation](teamsasyncoperation.md) 是一种例外情况，因为需要频繁对其进行轮询。）如果需要更频繁了解更改，应[创建指向该资源的订阅](../api/subscription-post-subscriptions.md)并接收更改通知 (webhooks)。 如果找不到对所需订阅类型的支持，建议通过 [UserVoice](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests?category_id=359626) 提供反馈。 

轮询新邮件时，必须指定支持的日期范围。 有关详细信息，请参阅 [get channel messages delta](/graph/api/chatmessage-delta?view=graph-rest-beta)。

轮询是指对资源重复进行 GET 操作来了解资源是否变更。 只要同一资源未进行轮询，就可以一天多次对该资源进行 GET 操作。 例如，每次用户访问/刷新网页时都可以执行 GET /me/joinedTeams，但在每隔 30 秒执行一次的循环中执行 GET /me/joinedTeams 来刷新该网页则不可取。

未遵循这些轮询要求的应用将被视为违反了 [Microsoft API 使用条款](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use)。 这可能导致额外的[限制](/graph/throttling)或暂停/终止使用 Microsoft API。

## <a name="whats-new"></a>最近更新
查找有关此 API 集的[最新新功能和更新](/graph/whats-new-overview)。

## <a name="see-also"></a>另请参阅

[Microsoft Teams API 概述](/graph/teams-concept-overview)
