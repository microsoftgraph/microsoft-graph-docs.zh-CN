---
title: teamJoiningDisabledEventMessageDetail 资源类型
description: 表示有关已禁用团队加入的事件消息的详细信息。
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a7082753265a6be3929f1b697e9e24f9b4e5f95a
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322392"
---
# <a name="teamjoiningdisabledeventmessagedetail-resource-type"></a>teamJoiningDisabledEventMessageDetail 资源类型

命名空间：microsoft.graph

表示有关已禁用 [团队加入的事件](../resources/team.md) 消息的详细信息。
为团队禁用加入时，将生成 **此消息**。


继承自 [eventMessageDetail](../resources/eventmessagedetail.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|initiator|[identitySet](../resources/identityset.md)|事件的发起人。|
|teamId|String|团队的唯一 **标识符**。|
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamJoiningDisabledEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamJoiningDisabledEventMessageDetail",
  "teamId": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>另请参阅
- [有关已禁用团队 **加入的事件消息** 的响应示例](/graph/system-messages/#team-joining-disabled)
- 有关其他类型的事件详细信息，请参阅 [系统消息](/graph/system-messages)。
