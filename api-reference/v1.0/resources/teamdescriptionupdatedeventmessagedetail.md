---
title: teamDescriptionUpdatedEventMessageDetail 资源类型
description: 表示有关更新的团队说明的事件消息的详细信息。
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8d7fbb900fb302f70a174d5549cba8feec740084
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322352"
---
# <a name="teamdescriptionupdatedeventmessagedetail-resource-type"></a>teamDescriptionUpdatedEventMessageDetail 资源类型

命名空间：microsoft.graph

表示有关更新的团队说明的事件 [消息](../resources/team.md) 的详细信息。
更新团队的描述 **时，将** 生成此消息。


继承自 [eventMessageDetail](../resources/eventmessagedetail.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|initiator|[identitySet](../resources/identityset.md)|事件的发起人。|
|teamDescription|String|团队 的更新 **说明**。|
|teamId|String|团队的唯一 **标识符**。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamDescriptionUpdatedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamDescriptionUpdatedEventMessageDetail",
  "teamId": "String",
  "teamDescription": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>另请参阅
- [有关更新的团队说明的事件消息 **的响应** 示例](/graph/system-messages/#team-description-updated)
- 有关其他类型的事件详细信息，请参阅 [系统消息](/graph/system-messages)。
