---
title: membersJoinedEventMessageDetail 资源类型
description: 表示有关已加入成员的事件消息的详细信息。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b5c95b230e31918ffce5a2a5588aed22e1a7dfd8
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/22/2021
ms.locfileid: "53534244"
---
# <a name="membersjoinedeventmessagedetail-resource-type"></a>membersJoinedEventMessageDetail 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关已加入成员的事件消息的详细信息。
当成员加入会议聊天时，将生成此消息。


继承自 [eventMessageDetail](../resources/eventmessagedetail.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|initiator|[identitySet](../resources/identityset.md)|事件的发起人。|
|members|[teamworkUserIdentity](../resources/teamworkuseridentity.md) 集合|加入聊天的成员列表。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.membersJoinedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.membersJoinedEventMessageDetail",
  "members": [
    {
      "@odata.type": "microsoft.graph.teamworkUserIdentity"
    }
  ],
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>另请参阅
- [有关已加入成员的事件消息的响应示例](/graph/system-messages/#members-joined)
- 有关其他类型的事件详细信息，请参阅 [系统消息](/graph/system-messages)。