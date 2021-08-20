---
title: 将 Microsoft Graph API 与 Microsoft Teams 结合使用
description: Microsoft Teams 是 Microsoft 365 中基于聊天的工作区，可提供对特定于团队的日历、文件、OneNote 笔记、规划器计划等对象的内置访问权限。
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
doc_type: conceptualPageType
ms.openlocfilehash: fb3c4e58afcf8f2fd8909b956e78b1118f4bb529
ms.sourcegitcommit: 6f04ad0e0cde696661511dcdf343942b43f73fc6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2021
ms.locfileid: "58396730"
---
# <a name="use-the-microsoft-graph-api-to-work-with-microsoft-teams"></a>将 Microsoft Graph API 与 Microsoft Teams 结合使用

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Teams 是 Microsoft 365 中基于聊天的工作区，可提供对特定于团队的日历、文件、OneNote 笔记、规划器计划、排班计划等对象的内置访问权限。

## <a name="key-resources-in-microsoft-teams"></a>Microsoft Teams 中的重要资源

| 资源 | 方法 |
|:---------------|:--------|
|[team](../resources/team.md)| [列出你的团队](../api/user-list-joinedteams.md)、[列出所有团队](/graph/teams-list-all-teams)、[创建](../api/team-put-teams.md)、[读取](../api/team-get.md)、[更新](../api/team-update.md)、[删除](../api/group-delete.md)、[克隆](../api/team-clone.md)、[归档](../api/team-archive.md)[取消归档](../api/team-unarchive.md) |
|[组](../resources/group.md)| [添加成员](../api/group-post-members.md)、 [移除成员](../api/group-delete-members.md)、[添加所有者](../api/group-post-owners.md)、 [移除所有者](../api/group-delete-owners.md)、[获取文件](drive.md)、[获取笔记本](../resources/notebook.md)、[获取计划](plannergroup.md)、[获取日历](event.md) |
|[频道](../resources/channel.md)|[列出](../api/channel-list.md)、[创建](../api/channel-post.md)、[读取](../api/channel-get.md)、[更新](../api/channel-patch.md)、[删除](../api/channel-delete.md)|
|[teamsTab](../resources/teamstab.md) |[列出](../api/channel-list-tabs.md)、[创建](../api/channel-post-tabs.md)、[读取](../api/channel-get-tabs.md)、[更新](../api/channel-patch-tabs.md)、[删除](../api/channel-delete-tabs.md) |
|[teamsApp](../resources/teamsapp.md)|[列出](../api/appcatalogs-list-teamsapps.md)、[发布](../api/teamsapp-publish.md)、[更新](../api/teamsapp-update.md)、[移除](../api/teamsapp-delete.md)|
|[teamsAppInstallation](../resources/teamsappinstallation.md)| [列出](../api/team-list-installedapps.md)、[安装](../api/team-post-installedapps.md)、[升级](../api/team-delete-installedapps.md)、[移除](../api/team-delete-installedapps.md) |
|[chatMessage](../resources/chatmessage.md)| [在频道中列出](../api/channel-list-messages.md)、[在聊天中列出](../api/chat-list-messages.md)、[发送](../api/chatmessage-post.md)、[在频道中读取](../api/chatmessage-get.md)、[在聊天中读取](../api/chatmessage-get.md)|
|[聊天](../resources/chat.md)| [列出](../api/chat-list.md)、[读取](../api/chat-get.md)、
|[call](../resources/call.md)| [应答](../api/call-answer.md)、[拒绝](../api/call-reject.md)、[重定向](../api/call-redirect.md)、[静音](../api/call-mute.md)、[取消静音](../api/call-unmute.md)、[更改屏幕共享角色](../api/call-changescreensharingrole.md)、[列出参与者](../api/call-list-participants.md)、[邀请参与者](../api/participant-invite.md)、[将所有参与者静音](../api/participant-muteall.md) |
|[日程安排](../resources/schedule.md)| [创建或替换](../api/team-put-schedule.md)、[获取](../api/schedule-get.md)、[共享](../api/schedule-share.md) |
|[schedulingGroup](../resources/schedulinggroup.md)| [创建](../api/schedule-post-schedulinggroups.md)、[列出](../api/schedule-list-schedulinggroups.md)、[获取](../api/schedulinggroup-get.md)、[替换](../api/schedulinggroup-put.md)、[删除](../api/schedulinggroup-delete.md) |
|[shift](../resources/shift.md)| [创建](../api/schedule-post-shifts.md)、[列出](../api/schedule-list-shifts.md)、[获取](../api/shift-get.md)、[替换](../api/shift-put.md)、[删除](../api/shift-delete.md) |
|[timeOff](../resources/timeoff.md)| [创建](../api/schedule-post-timesoff.md)、[列出](../api/schedule-list-timesoff.md)、[获取](../api/timeoff-get.md)、[替换](../api/timeoff-put.md)、[删除](../api/timeoff-delete.md) |
|[timeOffReason](../resources/timeoffreason.md)| [创建](../api/schedule-post-timeoffreasons.md)、[列出](../api/schedule-list-timeoffreasons.md)、[获取](../api/timeoffreason-get.md)、[替换](../api/timeoffreason-put.md)、[删除](../api/timeoffreason-delete.md) |
|[标记](../resources/teamworkTag.md)|[列出](../api/teamworkTag-list.md)、 [创建](../api/teamworkTag-post.md)、 [获取](../api/teamworkTag-get.md)、 [更新](../api/teamworkTag-update.md)、 [删除](../api/teamworkTag-delete.md)|
|[tagMember](../resources/teamworkTagMember.md)|[列出](../api/teamworkTagMember-list.md)、[创建](../api/teamworkTagMember-post.md)、[获取](../api/teamworkTagMember-get.md)、[删除](../api/teamworkTagMember-delete.md)|

## <a name="microsoft-teams-limits"></a>Microsoft Teams 限制

Microsoft Teams 的已测试性能和容量限制将记录在 [Microsoft Teams 限制和规范](/microsoftteams/limits-specifications-teams)中。
无论是直接使用 Microsoft Teams 还是使用 Microsoft Graph API，这些限制均适用。
由于每个团队都有一个对应的组，并且每个组都是一个目录对象，因此对[组数](/microsoft-365/admin/create-groups/office-365-groups#group-limits)和[目录对象数目（“资源”）](/azure/active-directory/users-groups-roles/directory-service-limits-restrictions) 的限制也可以发挥作用。 

频道内的文件存储在 SharePoint 中；[SharePoint online 限制](/office365/servicedescriptions/sharepoint-online-service-description/sharepoint-online-limits)适用。

另请参阅 [Microsoft Teams 服务限制](/graph/throttling#microsoft-teams-service-limits)。

## <a name="teams-and-groups"></a>用户和组

在 Microsoft Graph 中，Microsoft Teams 由[组](../resources/group.md)资源表示。 Microsoft Teams 和 Microsoft 365 组均可满足组协作的各种需求。 几乎所有基于组的功能都适用于 Microsoft Teams 和 Microsoft 365 组，例如组日历、文件、笔记、照片、计划等。 [团队](team.md)与 Microsoft 365 组之间的主要区别在于成员之间的通信模式。 团队成员的通信方式是在特定团队的上下文中进行持久聊天。 Microsoft 365 组成员通过组对话进行通信，它们是在 Outlook 的组上下文中发生的电子邮件对话。

具有团队的任何组都具有 **resourceProvisioningOptions** 属性，它包含“团队”。

>**注释：** 可以更改 **Group.resourceProvisioningOptions** 属性。
请不要在该集合中添加或删除“团队”；否则，当你列出所有团队时，你将获得错误结果。

以下是团队和组之间的 API 级别的区别：

- 持久聊天仅适用于 Microsoft Teams。 此功能由[频道](../resources/channel.md)和 [chatMessage](../resources/chatmessage.md) 资源按层次结构表示。
- 组对话仅适用于 Microsoft 365 组。 此功能由[对话](../resources/conversation.md)、[conversationThread](../resources/conversationthread.md) 和[帖子](../resources/post.md)资源按层次结构表示。
- [列出加入的团队](../api/user-list-joinedteams.md)方法仅适用于 Microsoft Teams。
- [呼叫和在线会议 API](./communications-api-overview.md) 仅适用于 Microsoft Teams。
- 另请参阅[已知问题](/graph/known-issues)以了解这些 API。

>注意：如果在 Microsoft Teams 应用（而非独立应用中）使用组 API（例如，作为 Microsoft Teams 中运行的选项卡或自动程序的一部分），请按照在 Microsoft Teams 页面中使用 Microsoft Graph 一文中的说明操作。

## <a name="membership-changes-in-microsoft-teams"></a>Microsoft Teams 中的成员身份更改

| 用例      | 谓词      | URL |
| ------------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| [添加成员](../api/team-post-members.md) | POST      | /teams/{team-id}/members  |
| [删除成员](../api/team-delete-members.md)    | DELETE    | /teams/{team-id}/members/{membership-id} |
| [更新成员角色](../api/team-update-members.md) | PATCH | /teams/{team-id}/members/{membership-id} |
| [更新团队](../api/team-update.md)  | PATCH     | /teams/{team-id} |

## <a name="polling-requirements"></a>轮询要求

如果应用程序轮询查看是否更改了某资源，则此操作每天只能执行一次。 （[teamsAsyncOperation](teamsasyncoperation.md) 是一种例外情况，因为需要频繁对其进行轮询。）如果需要更频繁了解更改，应[创建指向该资源的订阅](../api/subscription-post-subscriptions.md)并接收更改通知 (webhooks)。 如果找不到对所需订阅类型的支持，建议通过 [Microsoft 365 开发人员平台创意论坛](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph)提供反馈。 

轮询新邮件时，必须指定支持的日期范围。 有关详细信息，请参阅 [get channel messages delta](../api/chatmessage-delta.md)。

轮询是指对资源重复进行 GET 操作来了解资源是否变更。 只要同一资源未进行轮询，就可以一天多次对该资源进行 GET 操作。 例如，每次用户访问/刷新网页时都可以执行 GET /me/joinedTeams，但在每隔 30 秒执行一次的循环中执行 GET /me/joinedTeams 来刷新该网页则不可取。

未遵循这些轮询要求的应用将被视为违反了 [Microsoft API 使用条款](/legal/microsoft-apis/terms-of-use)。 这可能导致额外的[限制](/graph/throttling)或暂停/终止使用 Microsoft API。

## <a name="whats-new"></a>最近更新
了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。

## <a name="see-also"></a>另请参阅

- [Microsoft Teams API 概述](/graph/teams-concept-overview)
- 示例代码：[Contoso 航空](https://github.com/microsoftgraph/contoso-airlines-teams-sample)、[C# 迷你示例](https://github.com/microsoftgraph/csharp-teams-sample-graph)
