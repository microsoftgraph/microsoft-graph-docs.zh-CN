---
title: eventMessageDetail 资源类型
description: 表示事件消息详细信息的基类型。
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 79dad5d78b3e6804a0f0b950a37dd3bce5c057e1
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2022
ms.locfileid: "65399493"
---
# <a name="eventmessagedetail-resource-type"></a>eventMessageDetail 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

此抽象类型表示系统事件消息的详细信息。

系统消息是为事件生成的消息，例如添加到频道的成员、添加到聊天中的成员和更新的团队说明。

支持的事件列表

| 事件 | 说明 |
| :---- | :---------- |
| [callEndedEventMessageDetail](../resources/callEndedEventMessageDetail.md) | 呼叫已结束。 |
| [callRecordingEventMessageDetail](../resources/callRecordingEventMessageDetail.md) | 呼叫录制可用。 |
| [callStartedEventMessageDetail](../resources/callStartedEventMessageDetail.md) | 呼叫已启动。 |
| [callTranscriptEventMessageDetail](../resources/callTranscriptEventMessageDetail.md) | 呼叫脚本可用。 |
| [channelAddedEventMessageDetail](../resources/channelAddedEventMessageDetail.md) | 已添加通道。 |
| [channelDeletedEventMessageDetail](../resources/channelDeletedEventMessageDetail.md) | 已删除通道。 |
| [channelDescriptionUpdatedEventMessageDetail](../resources/channelDescriptionUpdatedEventMessageDetail.md) | 频道的说明已更新。 |
| [channelRenamedEventMessageDetail](../resources/channelRenamedEventMessageDetail.md) | 通道已重命名。 |
| [channelSetAsFavoriteByDefaultEventMessageDetail](../resources/channelSetAsFavoriteByDefaultEventMessageDetail.md) | 默认情况下，通道已设置为收藏夹。 |
| [channelUnsetAsFavoriteByDefaultEventMessageDetail](../resources/channelUnsetAsFavoriteByDefaultEventMessageDetail.md) | 默认情况下，通道已取消设置为收藏夹。 |
| [chatRenamedEventMessageDetail](../resources/chatRenamedEventMessageDetail.md) | 聊天已重命名。 |
| [conversationMemberRoleUpdatedEventMessageDetail](../resources/conversationMemberRoleUpdatedEventMessageDetail.md) | 已更新成员的角色。 |
| [meetingPolicyUpdatedEventMessageDetail](../resources/meetingPolicyUpdatedEventMessageDetail.md) | 会议策略已更新。 |
| [membersAddedEventMessageDetail](../resources/membersAddedEventMessageDetail.md) | 已添加成员。 |
| [membersDeletedEventMessageDetail](../resources/membersDeletedEventMessageDetail.md) | 成员已被删除。 |
| [membersJoinedEventMessageDetail](../resources/membersJoinedEventMessageDetail.md) | 成员已加入。 |
| [membersLeftEventMessageDetail](../resources/membersLeftEventMessageDetail.md) | 成员已离开。 |
| [tabUpdatedEventMessageDetail](../resources/tabUpdatedEventMessageDetail.md) | 选项卡已更新。 |
| [teamArchivedEventMessageDetail](../resources/teamArchivedEventMessageDetail.md) | 已存档团队。 |
| [teamCreatedEventMessageDetail](../resources/teamCreatedEventMessageDetail.md) | 已创建一个团队。 |
| [teamDescriptionUpdatedEventMessageDetail](../resources/teamDescriptionUpdatedEventMessageDetail.md) | 团队的说明已更新。 |
| [teamJoiningDisabledEventMessageDetail](../resources/teamJoiningDisabledEventMessageDetail.md) | 团队加入已禁用。 |
| [teamJoiningEnabledEventMessageDetail](../resources/teamJoiningEnabledEventMessageDetail.md) | 已启用团队加入。 |
| [teamRenamedEventMessageDetail](../resources/teamRenamedEventMessageDetail.md) | 已重命名团队。 |
| [teamsAppInstalledEventMessageDetail](../resources/teamsAppInstalledEventMessageDetail.md) | 已安装Teams应用。 |
| [teamsAppRemovedEventMessageDetail](../resources/teamsAppRemovedEventMessageDetail.md) | 已删除Teams应用。 |
| [teamsAppUpgradedEventMessageDetail](../resources/teamsAppUpgradedEventMessageDetail.md) | Teams应用已升级。 |
| [teamUnarchivedEventMessageDetail](../resources/teamUnarchivedEventMessageDetail.md) | 一个团队已经没有存档。 |

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

