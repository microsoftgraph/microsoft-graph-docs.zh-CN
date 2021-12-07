---
title: tabUpdatedEventMessageDetail 资源类型
description: 表示有关更新选项卡的事件消息的详细信息。
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 020adfcc34a8d2874e021d1b53441093c9f902f7
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322376"
---
# <a name="tabupdatedeventmessagedetail-resource-type"></a>tabUpdatedEventMessageDetail 资源类型

命名空间：microsoft.graph

表示有关更新选项卡的事件消息的详细信息。当频道或聊天中更新 [选项卡时，](../resources/channel.md) 将生成 [此消息](../resources/chat.md)。


继承自 [eventMessageDetail](../resources/eventmessagedetail.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|initiator|[identitySet](../resources/identityset.md)|事件的发起人。|
|tabId|String|选项卡的唯一标识符。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.tabUpdatedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.tabUpdatedEventMessageDetail",
  "tabId": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>另请参阅
- [有关更新选项卡的事件消息的响应示例](/graph/system-messages/#tab-updated)
- 有关其他类型的事件详细信息，请参阅 [系统消息](/graph/system-messages)。
