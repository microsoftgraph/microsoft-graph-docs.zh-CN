---
title: membersAddedEventMessageDetail 资源类型
description: 表示有关已添加成员的事件消息的详细信息。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 43a9d93166968f92cde12f37b76b8da9062ee4c3
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/22/2021
ms.locfileid: "53534248"
---
# <a name="membersaddedeventmessagedetail-resource-type"></a>membersAddedEventMessageDetail 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关已添加成员的事件消息的详细信息。
将成员添加到聊天、频道或团队时，将生成此消息。


继承自 [eventMessageDetail](../resources/eventmessagedetail.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|initiator|[identitySet](../resources/identityset.md)|事件的发起人。|
|members|[teamworkUserIdentity](../resources/teamworkuseridentity.md) 集合|添加的成员列表。|

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
  }
}
```


## <a name="see-also"></a>另请参阅
- [有关已添加成员的事件消息的响应示例](/graph/system-messages/#members-added)
- 有关其他类型的事件详细信息，请参阅 [系统消息](/graph/system-messages)。