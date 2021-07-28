---
title: meetingPolicyUpdatedEventMessageDetail 资源类型
description: 表示有关更新的会议策略的事件消息的详细信息。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2fb18c1275fe6b0d9979978a0d07b4247ddfcdce
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/22/2021
ms.locfileid: "53534250"
---
# <a name="meetingpolicyupdatedeventmessagedetail-resource-type"></a>meetingPolicyUpdatedEventMessageDetail 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关更新的会议策略的事件消息的详细信息。
更新会议选项"允许会议聊天" **时，将生成** 此消息。


继承自 [eventMessageDetail](../resources/eventmessagedetail.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|initiator|[identitySet](../resources/identityset.md)|事件的发起人。|
|meetingChatEnabled|Boolean|表示是否启用会议聊天。|
|meetingChatId|String|会议聊天的唯一标识符。|

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