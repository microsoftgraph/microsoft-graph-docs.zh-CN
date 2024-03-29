---
title: callStartedEventMessageDetail 资源类型
description: 表示有关呼叫开始的事件消息的详细信息。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: de887904a352749b2a8edd3e9b4d5554e0f34d49
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/22/2021
ms.locfileid: "53534234"
---
# <a name="callstartedeventmessagedetail-resource-type"></a>callStartedEventMessageDetail 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关呼叫开始的事件消息的详细信息。
此消息在呼叫开始时生成。


继承自 [eventMessageDetail](../resources/eventmessagedetail.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|callEventType|teamworkCallEventType|表示呼叫事件类型。 可取值为：`call`、`meeting`、`screenShare`、`unknownFutureValue`。|
|callId|String|调用的唯一标识符。|
|initiator|[identitySet](../resources/identityset.md)|事件的发起人。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.callStartedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.callStartedEventMessageDetail",
  "callId": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "callEventType": "String"
}
```


## <a name="see-also"></a>另请参阅
- [有关已启动呼叫的事件消息的响应示例](/graph/system-messages/#call-started)
- 有关其他类型的事件详细信息，请参阅 [系统消息](/graph/system-messages)。