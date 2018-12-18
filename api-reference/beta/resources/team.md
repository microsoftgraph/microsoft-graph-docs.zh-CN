---
title: 团队资源类型
description: '团队中的 Microsoft 团队是通道的集合。 '
author: nkramer
ms.openlocfilehash: 0ed654bf4c8d627dd9466f9263b121f85800b853
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27345478"
---
# <a name="team-resource-type"></a>团队资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

团队中的 Microsoft 团队是[通道](channel.md)的集合。 通道表示一个主题，因此讨论，团队中的逻辑隔离。

每个团队是与[组](../resources/group.md)关联。
组具有相同的 ID 团队-例如，/groups/ {id} / 球队是 /teams/ {id} 相同。
有关使用组和团队中的成员的详细信息，请参阅[使用 Microsoft Graph REST API 以使用 Microsoft 团队](teams-api-overview.md)。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[创建工作组](../api/team-post.md) | [teamsAsyncOperation](teamsasyncoperation.md) | 从头开始创建团队。 |
|[从组中创建工作组](../api/team-put-teams.md) | [团队](team.md) | 创建一个新的团队，或添加到现有组的团队。|
|[获取工作组](../api/team-get.md) | [团队](team.md) | 检索的属性和指定团队的关系。|
|[更新团队](../api/team-update.md) | [团队](team.md) |更新指定的团队的属性。 |
|[删除团队](/graph/api/group-delete?view=graph-rest-1.0) | 无 |删除团队和其关联的组。 |
|[克隆团队](../api/team-clone.md) | [teamsAsyncOperation](../resources/teamsasyncoperation.md) |复制团队和其关联的组。 |
|[存档团队](../api/team-archive.md) | [teamsAsyncOperation](../resources/teamsasyncoperation.md) |将团队放在只读状态。 |
|[Unarchive 团队](../api/team-unarchive.md) | [teamsAsyncOperation](../resources/teamsasyncoperation.md) |还原到读写状态团队。 |
|[列出您的团队](../api/user-list-joinedteams.md) | [团队](team.md)集合 | 列出您是成员的团队。 |
|[列出所有团队](/graph/teams-list-all-teams) | [组](group.md) 集合 | 列出具有团队的所有组。 |
|[将应用程序发布到您的组织](../resources/teamsapp.md)| [teamsApp](../resources/teamsapp.md) | 创建团队应用程序仅对您的组织可见。 |
|[将应用程序添加到团队](../api/teamsappinstallation-add.md) | [teamsappinstallation](teamsappinstallation.md) | 将 （安装） 添加到团队应用程序。|
|[选项卡添加到频道](../api/teamstab-add.md) | [teamsTab](../resources/teamstab.md) | 将 （安装） 添加到团队的通道选项卡。|
|[列表通道消息](../api/channel-list-messages.md)  | [chatMessage](../resources/chatmessage.md) | [在通道中收到消息](../api/channel-list-messages.md) |

## <a name="properties"></a>属性

| 属性 | 类型   | 说明 |
|:---------------|:--------|:----------|
|displayName|string| 工作组的名称。 |
|说明|string| 团队的可选说明。 |
|Classification|string| 可选标签。 通常介绍团队的数据或商业敏感度。 必须匹配一个预配置一租户的目录中。 |
|具专业性|[teamSpecialization](teamspecialization.md)| 可选。 指示是否团队适用于特定用例。  每个团队具专业性有权访问唯一行为和针对其用例的体验。 |
|visibility|[teamVisibilityType](teamvisibilitytype.md)| 可见性组和团队。 默认值为 Public。 |
|funSettings|[teamFunSettings](teamfunsettings.md) |要配置的团队中的使用 Giphy、 memes 和标签的设置。|
|guestSettings|[teamGuestSettings](teamguestsettings.md) |要配置的是否来宾可以创建、 更新或删除通道团队中的设置。|
|isArchived|Boolean|此团队是否处于只读模式。 |
|memberSettings|[teamMemberSettings](teammembersettings.md) |例如，要配置的成员可以执行某些操作时，是否设置创建通道，并将自动程序，添加团队中。|
|messagingSettings|[teamMessagingSettings](teammessagingsettings.md) |要配置的消息设置和团队中的提及。|
|WebUrl|字符串 （只读） | 将转到 Microsoft 团队客户端中的团队超链接。 这是当您右键单击在客户端中的 Microsoft 团队团队，然后选择**获取团队链接**获取的 URL。 此 URL 应是视为不透明 blob，并且未分列。 |

## <a name="relationships"></a>Relationships

| 关系 | 类型   | 说明 |
|:---------------|:--------|:----------|
|apps|[teamsApp](teamsapp.md)集合| （已过时）此团队中安装应用程序。|
|通道|[通道](channel.md)集合|通道邮件与团队关联的集合。|
|installedApps|[teamsAppInstallation](teamsappinstallation.md)集合|此团队中安装应用程序。|
|owners|[用户](user.md)| 此工作组的所有者的列表。 |
|template|[teamsTemplate](teamstemplate.md)| 从该团队创建模板。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.team",
  "baseType": "microsoft.graph.entity"
}-->

```json
{  
  "guestSettings": {"@odata.type": "microsoft.graph.teamGuestSettings"},
  "memberSettings": {"@odata.type": "microsoft.graph.teamMemberSettings"},
  "messagingSettings": {"@odata.type": "microsoft.graph.teamMessagingSettings"},
  "funSettings": {"@odata.type": "microsoft.graph.teamFunSettings"},
  "isArchived": false,
  "webUrl": "https://...longUrl..."
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="see-also"></a>另请参阅
- [与团队创建组](/graph/teams-create-group-and-team)
- [团队 API 概述](teams-api-overview.md)
