---
title: messagePinnedEventMessageDetail 资源类型
description: 表示有关固定聊天消息的事件消息的详细信息。
author: sumanac
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: acec5aaf817549c6ac4913b2aced914ee6a497d2
ms.sourcegitcommit: 191b797b178f40fde6419719fcd75461e6869401
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/16/2022
ms.locfileid: "66118669"
---
# <a name="messagepinnedeventmessagedetail-resource-type"></a>messagePinnedEventMessageDetail 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关固定 [chatMessage](../resources/chatmessage.md) 的事件消息的详细信息。 在固定聊天消息时生成此消息。

继承自 [eventMessageDetail](../resources/eventmessagedetail.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|eventDateTime|DateTimeOffset|事件发生的日期和时间。|
|initiator|[identitySet](../resources/identityset.md)|事件的发起者。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.messagePinnedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.messagePinnedEventMessageDetail",
  "eventDateTime": "String (timestamp)",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>另请参阅
- [有关固定聊天消息的事件消息的示例响应](/graph/system-messages/#message-pinned)
- 有关其他类型的事件的详细信息，请参阅 [系统消息](/graph/system-messages)。
