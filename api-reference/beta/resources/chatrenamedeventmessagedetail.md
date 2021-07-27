---
title: chatRenamedEventMessageDetail 资源类型
description: 表示有关重命名聊天的事件消息的详细信息。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5a247dd16674a6f7d3173ea5f3f5383d8fd2d68e
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/22/2021
ms.locfileid: "53534327"
---
# <a name="chatrenamedeventmessagedetail-resource-type"></a>chatRenamedEventMessageDetail 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关重命名聊天的事件消息的详细信息。
更新组或会议聊天主题时，将生成此消息。


继承自 [eventMessageDetail](../resources/eventmessagedetail.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|chatDisplayName|String|聊天的更新名称。|
|chatId|String|聊天的唯一标识符。|
|initiator|[identitySet](../resources/identityset.md)|事件的发起人。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.chatRenamedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.chatRenamedEventMessageDetail",
  "chatId": "String",
  "chatDisplayName": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>另请参阅
- [有关重命名聊天的事件消息的响应示例](/graph/system-messages/#chat-renamed)
- 有关其他类型的事件详细信息，请参阅 [系统消息](/graph/system-messages)。