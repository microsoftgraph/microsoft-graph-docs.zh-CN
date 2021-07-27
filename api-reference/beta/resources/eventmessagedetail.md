---
title: eventMessageDetail 资源类型
description: 表示事件消息详细信息的基本类型。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: da40b7413bc52a2ec0d663e2b7e0467f0e5e06fd
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/22/2021
ms.locfileid: "53535709"
---
# <a name="eventmessagedetail-resource-type"></a>eventMessageDetail 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

此抽象类型表示系统事件消息的详细信息。

系统消息是针对事件（如添加到频道的成员、添加到聊天的成员和更新的团队说明）生成的消息。

支持的事件列表

| 事件 | 说明 |
| :---- | :---------- |
| [callEndedEventMessageDetail](../resources/callStartedEventMessageDetail.md) | 呼叫已结束。 |
| [callRecordingEventMessageDetail](../resources/callRecordingEventMessageDetail.md) | 呼叫录制可用。 |
| [callStartedEventMessageDetail](../resources/callStartedEventMessageDetail.md) | 呼叫已启动。 |
| [callTranscriptEventMessageDetail](../resources/callTranscriptEventMessageDetail.md) | 呼叫脚本可用。 |
| [channelAddedEventMessageDetail](../resources/channelAddedEventMessageDetail.md) | 已添加频道。 |
| [channelDeletedEventMessageDetail](../resources/channelDeletedEventMessageDetail.md) | 频道已删除。 |
| [channelDescriptionUpdatedEventMessageDetail](../resources/channelDescriptionUpdatedEventMessageDetail.md) | 频道说明已更新。 |
| [channelRenamedEventMessageDetail](../resources/channelRenamedEventMessageDetail.md) | 频道已重命名。 |
| [channelSetAsFavoriteByDefaultEventMessageDetail](../resources/channelSetAsFavoriteByDefaultEventMessageDetail.md) | 默认情况下，频道已设置为收藏。 |
| [channelUnsetAsFavoriteByDefaultEventMessageDetail](../resources/channelUnsetAsFavoriteByDefaultEventMessageDetail.md) | 默认情况下，频道已取消设置为收藏。 |
| [chatRenamedEventMessageDetail](../resources/chatRenamedEventMessageDetail.md) | 聊天已重命名。 |
| [conversationMemberRoleUpdatedEventMessageDetail](../resources/conversationMemberRoleUpdatedEventMessageDetail.md) | 角色已更新为成员。 |
| [meetingPolicyUpdatedEventMessageDetail](../resources/meetingPolicyUpdatedEventMessageDetail.md) | 会议策略已更新。 |
| [membersAddedEventMessageDetail](../resources/membersAddedEventMessageDetail.md) | 已添加成员。 |
| [membersDeletedEventMessageDetail](../resources/membersDeletedEventMessageDetail.md) | 已删除成员。 |
| [membersJoinedEventMessageDetail](../resources/membersJoinedEventMessageDetail.md) | 成员已加入。 |
| [membersLeftEventMessageDetail](../resources/membersLeftEventMessageDetail.md) | 成员已离开。 |
| [tabUpdatedEventMessageDetail](../resources/tabUpdatedEventMessageDetail.md) | 选项卡已更新。 |
| [teamArchivedEventMessageDetail](../resources/teamArchivedEventMessageDetail.md) | 团队已存档。 |
| [teamCreatedEventMessageDetail](../resources/teamCreatedEventMessageDetail.md) | 已创建团队。 |
| [teamDescriptionUpdatedEventMessageDetail](../resources/teamDescriptionUpdatedEventMessageDetail.md) | 团队的说明已更新。 |
| [teamJoiningDisabledEventMessageDetail](../resources/teamJoiningDisabledEventMessageDetail.md) | 团队加入已禁用。 |
| [teamJoiningEnabledEventMessageDetail](../resources/teamJoiningEnabledEventMessageDetail.md) | 已启用团队加入。 |
| [teamRenamedEventMessageDetail](../resources/teamRenamedEventMessageDetail.md) | 团队已重命名。 |
| [teamsAppInstalledEventMessageDetail](../resources/teamsAppInstalledEventMessageDetail.md) | Teams应用已安装。 |
| [teamsAppRemovedEventMessageDetail](../resources/teamsAppRemovedEventMessageDetail.md) | Teams已删除应用。 |
| [teamsAppUpgradedEventMessageDetail](../resources/teamsAppUpgradedEventMessageDetail.md) | Teams应用已升级。 |
| [teamUnarchivedEventMessageDetail](../resources/teamUnarchivedEventMessageDetail.md) | 团队已取消存档。 |

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

