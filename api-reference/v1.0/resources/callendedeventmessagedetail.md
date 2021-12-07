---
title: callEndedEventMessageDetail 资源类型
description: 表示有关已结束呼叫的事件消息的详细信息。
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9a441f7f3562f7f07db93764544ab419e46fa16f
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322409"
---
# <a name="callendedeventmessagedetail-resource-type"></a>callEndedEventMessageDetail 资源类型

命名空间：microsoft.graph

表示有关已结束呼叫的事件消息的详细信息。
此消息在呼叫结束时生成。


继承自 [eventMessageDetail](../resources/eventmessagedetail.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|callDuration|期限|呼叫的持续时间。|
|callEventType|teamworkCallEventType|表示呼叫事件类型。 可能的值是：`call`、`meeting`、`screenShare`、`unknownFutureValue`。|
|callId|String|调用的唯一标识符。|
|callParticipants|[callParticipantInfo](../resources/callparticipantinfo.md) 集合|呼叫参与者列表。|
|initiator|[identitySet](../resources/identityset.md)|事件的发起人。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.callEndedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.callEndedEventMessageDetail",
  "callId": "String",
  "callParticipants": [
    {
      "@odata.type": "microsoft.graph.callParticipantInfo"
    }
  ],
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "callDuration": "String (duration)",
  "callEventType": "String"
}
```

## <a name="see-also"></a>另请参阅
- [有关已结束呼叫的事件消息的响应示例](/graph/system-messages/#call-ended)
- 有关其他类型的事件详细信息，请参阅 [系统消息](/graph/system-messages)。

