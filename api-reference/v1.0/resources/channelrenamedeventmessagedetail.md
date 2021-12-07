---
title: channelRenamedEventMessageDetail 资源类型
description: 表示有关重命名通道的事件消息的详细信息。
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e6f0b2ac19c9f51bbc0cc222bf81470509a2a265
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322379"
---
# <a name="channelrenamedeventmessagedetail-resource-type"></a>channelRenamedEventMessageDetail 资源类型

命名空间：microsoft.graph

表示有关重命名通道的事件消息 [的详细信息](../resources/channel.md)。
更新频道名称 **时，将** 生成此消息。


继承自 [eventMessageDetail](../resources/eventmessagedetail.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|channelDisplayName|String|频道的更新 **名称**。|
|channelId|String|频道的唯一 **标识符**。|
|initiator|[identitySet](../resources/identityset.md)|事件的发起人。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.channelRenamedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.channelRenamedEventMessageDetail",
  "channelId": "String",
  "channelDisplayName": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>另请参阅
- [有关重命名通道的事件消息的响应 **示例**](/graph/system-messages/#channel-renamed)
- 有关其他类型的事件详细信息，请参阅 [系统消息](/graph/system-messages)。
