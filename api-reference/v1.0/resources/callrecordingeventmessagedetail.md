---
title: callRecordingEventMessageDetail 资源类型
description: 表示有关呼叫记录的事件消息的详细信息。
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b37d49f0b13aa9da1445f74b74011f3bdc129112
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322405"
---
# <a name="callrecordingeventmessagedetail-resource-type"></a>callRecordingEventMessageDetail 资源类型

命名空间：microsoft.graph

表示有关呼叫记录的事件消息的详细信息。
呼叫录制开始时将生成此消息。


继承自 [eventMessageDetail](../resources/eventmessagedetail.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|callId|String|调用的唯一标识符。|
|callRecordingDisplayName|String|呼叫记录的显示名称。|
|callRecordingDuration|期限|呼叫录制的持续时间。|
|callRecordingStatus|callRecordingStatus|呼叫录制的状态。 可取值为：`success`、`failure`、`initial`、`chunkFinished`、`unknownFutureValue`。|
|callRecordingUrl|String|呼叫录制 URL。|
|initiator|[identitySet](../resources/identityset.md)|事件的发起人。|
|meetingOrganizer|[identitySet](../resources/identityset.md)|会议的组织者。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.callRecordingEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.callRecordingEventMessageDetail",
  "callId": "String",
  "callRecordingDisplayName": "String",
  "callRecordingUrl": "String",
  "callRecordingDuration": "String (duration)",
  "callRecordingStatus": "String",
  "meetingOrganizer": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>另请参阅
- [有关呼叫记录的事件消息的响应示例](/graph/system-messages/#call-recording)
- 有关其他类型的事件详细信息，请参阅 [系统消息](/graph/system-messages)。

