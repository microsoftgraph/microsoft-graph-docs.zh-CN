---
title: callTranscriptEventMessageDetail 资源类型
description: 表示有关呼叫脚本的事件消息的详细信息。
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5a57a6f5fc98fb518cf55d56c784fb86ec4c8aab
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322374"
---
# <a name="calltranscripteventmessagedetail-resource-type"></a>callTranscriptEventMessageDetail 资源类型

命名空间：microsoft.graph

表示有关呼叫脚本的事件消息的详细信息。
当脚本可用于呼叫时，将生成此消息。


继承自 [eventMessageDetail](../resources/eventmessagedetail.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|callId|String|调用的唯一标识符。|
|callTranscriptICalUid|String|呼叫脚本的唯一标识符。|
|meetingOrganizer|[identitySet](../resources/identityset.md)|会议的组织者。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.callTranscriptEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.callTranscriptEventMessageDetail",
  "callId": "String",
  "callTranscriptICalUid": "String",
  "meetingOrganizer": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>另请参阅
- [有关呼叫脚本的事件消息的响应示例](/graph/system-messages/#call-transcript)
- 有关其他类型的事件详细信息，请参阅 [系统消息](/graph/system-messages)。
