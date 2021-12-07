---
title: meetingPolicyUpdatedEventMessageDetail 资源类型
description: 表示有关更新的会议策略的事件消息的详细信息。
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 256f50d33957ca76bdeedda604698c80739b431b
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322353"
---
# <a name="meetingpolicyupdatedeventmessagedetail-resource-type"></a>meetingPolicyUpdatedEventMessageDetail 资源类型

命名空间：microsoft.graph

表示有关更新的会议策略的事件消息的详细信息。
更新会议选项"允许会议聊天" **时，将生成** 此消息。


继承自 [eventMessageDetail](../resources/eventmessagedetail.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|initiator|[identitySet](../resources/identityset.md)|事件的发起人。|
|meetingChatEnabled|布尔值|表示 [是否启用](../resources/chat.md) 会议聊天。|
|meetingChatId|String|会议聊天的唯一 **标识符**。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.meetingPolicyUpdatedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.meetingPolicyUpdatedEventMessageDetail",
  "meetingChatId": "String",
  "meetingChatEnabled": "Boolean",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>另请参阅
- [有关更新的会议策略的事件消息的响应示例](/graph/system-messages/#meeting-policy-updated)
- 有关其他类型的事件详细信息，请参阅 [系统消息](/graph/system-messages)。
