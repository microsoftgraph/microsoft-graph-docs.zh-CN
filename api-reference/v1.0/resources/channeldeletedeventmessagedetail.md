---
title: channelDeletedEventMessageDetail 资源类型
description: 表示有关从团队中删除的频道的事件消息的详细信息。
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 99a009ac2fd967a8ebcc3a7a688f34e0f84cdfde
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322381"
---
# <a name="channeldeletedeventmessagedetail-resource-type"></a>channelDeletedEventMessageDetail 资源类型

命名空间：microsoft.graph

表示有关从团队 [中删除的频道](../resources/channel.md) 的事件消息 [的详细信息](../resources/team.md)。
从团队中删除 **标准频道时** ，将生成 **此消息**。


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
  "@odata.type": "microsoft.graph.channelDeletedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.channelDeletedEventMessageDetail",
  "channelId": "String",
  "channelDisplayName": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>另请参阅
- [有关从团队 **中删除的频道** 的事件消息的示例 **响应**](/graph/system-messages/#channel-deleted)
- 有关其他类型的事件详细信息，请参阅 [系统消息](/graph/system-messages)。
