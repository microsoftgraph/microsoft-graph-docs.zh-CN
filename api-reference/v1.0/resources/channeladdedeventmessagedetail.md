---
title: channelAddedEventMessageDetail 资源类型
description: 表示有关添加到团队的频道的事件消息的详细信息。
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2a93e6f24992d361f92eb0831f8334a225fc95bf
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322383"
---
# <a name="channeladdedeventmessagedetail-resource-type"></a>channelAddedEventMessageDetail 资源类型

命名空间：microsoft.graph

表示有关添加到团队 [的频道的事件](../resources/channel.md) 消息 [的详细信息](../resources/team.md)。
将标准频道添加到 **团队时，** 将生成 **此消息**。


继承自 [eventMessageDetail](../resources/eventmessagedetail.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|channelDisplayName|String|频道的显示 **名称**。|
|channelId|String|频道的唯一 **标识符**。|
|initiator|[identitySet](../resources/identityset.md)|事件的发起人。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.channelAddedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.channelAddedEventMessageDetail",
  "channelId": "String",
  "channelDisplayName": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>另请参阅
- [有关添加到团队的 **频道的事件消息** 的示例 **响应**](/graph/system-messages/#channel-added)
- 有关其他类型的事件详细信息，请参阅 [系统消息](/graph/system-messages)。
