---
title: teamJoiningEnabledEventMessageDetail 资源类型
description: 表示有关已启用团队加入的事件消息的详细信息。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 963e53cbb684ed0ab78e0c7eb2e1247f35b5eb2e
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/22/2021
ms.locfileid: "53535714"
---
# <a name="teamjoiningenabledeventmessagedetail-resource-type"></a>teamJoiningEnabledEventMessageDetail 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关已启用团队加入的事件消息的详细信息。
为团队启用加入时，将生成此消息。


继承自 [eventMessageDetail](../resources/eventmessagedetail.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|initiator|[identitySet](../resources/identityset.md)|事件的发起人。|
|teamId|String|团队的唯一标识符。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamJoiningEnabledEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamJoiningEnabledEventMessageDetail",
  "teamId": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>另请参阅
- [有关已启用团队加入的事件消息的响应示例](/graph/system-messages/#team-joining-enabled)
- 有关其他类型的事件详细信息，请参阅 [系统消息](/graph/system-messages)。