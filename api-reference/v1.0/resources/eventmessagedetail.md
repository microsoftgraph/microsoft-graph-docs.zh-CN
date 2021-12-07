---
title: eventMessageDetail 资源类型
description: 表示系统事件消息的详细信息。
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ec2d6e8af1faecb92fb73b2fd04150c7fd29eb00
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322378"
---
# <a name="eventmessagedetail-resource-type"></a>eventMessageDetail 资源类型

命名空间：microsoft.graph

表示系统事件消息的详细信息。

系统消息是针对事件（如添加到频道的成员[](../resources/conversationMember.md)、添加到聊天的成员[](../resources/channel.md)和更新的团队[说明）生成](../resources/team.md)的消息[](../resources/chat.md)。

支持的事件列表

| 事件 | 说明 |
| :---- | :---------- |
| [callEndedEventMessageDetail](../resources/callStartedEventMessageDetail.md) | 呼叫已结束。 |
| [callRecordingEventMessageDetail](../resources/callRecordingEventMessageDetail.md) | 呼叫录制可用。 |
| [callStartedEventMessageDetail](../resources/callStartedEventMessageDetail.md) | 呼叫已启动。 |
| [callTranscriptEventMessageDetail](../resources/callTranscriptEventMessageDetail.md) | 呼叫脚本可用。 |
| [channelAddedEventMessageDetail](../resources/channelAddedEventMessageDetail.md) | 已 **添加** 频道。 |
| [channelDeletedEventMessageDetail](../resources/channelDeletedEventMessageDetail.md) | **频道** 已删除。 |
| [channelDescriptionUpdatedEventMessageDetail](../resources/channelDescriptionUpdatedEventMessageDetail.md) | **频道说明** 已更新。 |
| [channelRenamedEventMessageDetail](../resources/channelRenamedEventMessageDetail.md) | **频道** 已重命名。 |
| [channelSetAsFavoriteByDefaultEventMessageDetail](../resources/channelSetAsFavoriteByDefaultEventMessageDetail.md) | 默认情况下 **，** 频道已设置为收藏。 |
| [channelUnsetAsFavoriteByDefaultEventMessageDetail](../resources/channelUnsetAsFavoriteByDefaultEventMessageDetail.md) | 默认情况下 **，** 频道已取消设置为收藏。 |
| [chatRenamedEventMessageDetail](../resources/chatRenamedEventMessageDetail.md) | 聊天已重命名。 |
| [conversationMemberRoleUpdatedEventMessageDetail](../resources/conversationMemberRoleUpdatedEventMessageDetail.md) | 角色已更新为 **成员**。 |
| [meetingPolicyUpdatedEventMessageDetail](../resources/meetingPolicyUpdatedEventMessageDetail.md) | 会议策略已更新。 |
| [membersAddedEventMessageDetail](../resources/membersAddedEventMessageDetail.md) | **已** 添加成员。 |
| [membersDeletedEventMessageDetail](../resources/membersDeletedEventMessageDetail.md) | **已删除** 成员。 |
| [membersJoinedEventMessageDetail](../resources/membersJoinedEventMessageDetail.md) | **成员** 已加入。 |
| [membersLeftEventMessageDetail](../resources/membersLeftEventMessageDetail.md) | **成员** 已离开。 |
| [tabUpdatedEventMessageDetail](../resources/tabUpdatedEventMessageDetail.md) | 选项卡已更新。 |
| [teamArchivedEventMessageDetail](../resources/teamArchivedEventMessageDetail.md) | **团队** 已存档。 |
| [teamCreatedEventMessageDetail](../resources/teamCreatedEventMessageDetail.md) | **已** 创建团队。 |
| [teamDescriptionUpdatedEventMessageDetail](../resources/teamDescriptionUpdatedEventMessageDetail.md) | **团队的说明** 已更新。 |
| [teamJoiningDisabledEventMessageDetail](../resources/teamJoiningDisabledEventMessageDetail.md) | **团队** 加入已禁用。 |
| [teamJoiningEnabledEventMessageDetail](../resources/teamJoiningEnabledEventMessageDetail.md) | **已启用** 团队加入。 |
| [teamRenamedEventMessageDetail](../resources/teamRenamedEventMessageDetail.md) | 团队 **已** 重命名。 |
| [teamsAppInstalledEventMessageDetail](../resources/teamsAppInstalledEventMessageDetail.md) | [Teams应用](../resources/teamsApp.md)已安装。 |
| [teamsAppRemovedEventMessageDetail](../resources/teamsAppRemovedEventMessageDetail.md) | **Teams已删除** 应用。 |
| [teamsAppUpgradedEventMessageDetail](../resources/teamsAppUpgradedEventMessageDetail.md) | **Teams应用** 已升级。 |
| [teamUnarchivedEventMessageDetail](../resources/teamUnarchivedEventMessageDetail.md) | **团队** 已取消存档。 |

## <a name="properties"></a>属性
无。



## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.eventMessageDetail"
}
```

