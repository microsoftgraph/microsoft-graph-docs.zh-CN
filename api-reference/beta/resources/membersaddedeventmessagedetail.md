---
title: membersAddedEventMessageDetail 资源类型
description: 表示有关已添加成员的事件消息的详细信息。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 33d0c73ff5726310c1a4566813bd034cd9d5e9cc
ms.sourcegitcommit: 6f04ad0e0cde696661511dcdf343942b43f73fc6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2021
ms.locfileid: "58396989"
---
# <a name="membersaddedeventmessagedetail-resource-type"></a>membersAddedEventMessageDetail 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关已添加成员的事件消息的详细信息。
将成员添加到聊天、频道或团队时，将生成此消息。
频道 **中添加的成员事件的 visibleHistoryStartDateTime** 属性始终设置为 `0001-01-01T00:00:00Z` ，这表示共享所有历史记录。

> **注意**：对于聊天，当成员的所选共享历史记录时间早于 initator 的可见历史记录时间时 [，conversationMember](conversationmember.md)和 **membersAddedEventMessageDetail** 消息的 **visibleHistoryStartDateTime** 属性可能具有不同的值。 [conversationMember](conversationmember.md) 具有成员的有效可见历史记录时间，时间基于发起人可见的历史记录时间。


继承自 [eventMessageDetail](../resources/eventmessagedetail.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|initiator|[identitySet](../resources/identityset.md)|事件的发起人。|
|members|[teamworkUserIdentity](../resources/teamworkuseridentity.md) 集合|添加的成员列表。|
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
- [有关已添加成员的事件消息的响应示例](/graph/system-messages/#members-added)
- 有关其他类型的事件详细信息，请参阅 [系统消息](/graph/system-messages)。
