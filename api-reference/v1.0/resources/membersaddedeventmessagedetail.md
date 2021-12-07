---
title: membersAddedEventMessageDetail 资源类型
description: 表示有关已添加成员的事件消息的详细信息。
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: df1bb119f115d047fb8d5ff6a426ae259d8fe55d
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322389"
---
# <a name="membersaddedeventmessagedetail-resource-type"></a>membersAddedEventMessageDetail 资源类型

命名空间：microsoft.graph

表示有关已添加成员的事件 [消息](../resources/conversationMember.md) 的详细信息。
将成员 **添加到聊天、** 频道或 [团队时](../resources/channel.md)，[](../resources/chat.md)将生成 [此消息](../resources/team.md)。
有关添加到频道的成员的事件的 **visibleHistoryStartDateTime** 属性始终设置为 ，这 `0001-01-01T00:00:00Z` 表示共享所有历史记录。

> **注意**：如果聊天中成员的选定 shareHistoryTime 值早于发起人可见的历史记录时间，则 [conversationMember](conversationmember.md)和 **membersAddedEventMessageDetail** 消息的 **visibleHistoryStartDateTime** 属性可能具有不同的值。 


继承自 [eventMessageDetail](../resources/eventmessagedetail.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|initiator|[identitySet](../resources/identityset.md)|事件的发起人。|
|members|[teamworkUserIdentity](../resources/teamworkuseridentity.md) 集合|添加 **的成员** 列表。|
|visibleHistoryStartDateTime|DateTimeOffset|表示对话历史记录与对话成员共享多远的时间戳。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.membersAddedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.membersAddedEventMessageDetail",
  "members": [
    {
      "@odata.type": "microsoft.graph.teamworkUserIdentity"
    }
  ],
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "visibleHistoryStartDateTime": "String (timestamp)"
}
```


## <a name="see-also"></a>另请参阅
- [有关添加成员的事件消息 **的响应** 示例](/graph/system-messages/#members-added)
- 有关其他类型的事件详细信息，请参阅 [系统消息](/graph/system-messages)。
