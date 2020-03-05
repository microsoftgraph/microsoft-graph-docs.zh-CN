---
title: incomingContext 资源类型
description: 与来电相关的上下文。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: a7eba09d18b2b60c3a5ae45a8ad335d8971d2c77
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42496374"
---
# <a name="incomingcontext-resource-type"></a>incomingContext 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

与来电相关的上下文。

## <a name="properties"></a>属性

| 属性              | 类型                          | 说明                                                             |
|:----------------------|:------------------------------|:------------------------------------------------------------------------|
| observedParticipantId | String                        | 正在观察的参与者的 id。 只读。         |
| onBehalfOf            | [identitySet](identityset.md) | 代表调用所发生的标识。                   |
| sourceParticipantId   | String                        | 触发传入呼叫的参与者的 id。 只读。  |
| transferor            | [identitySet](identityset.md) | 转接呼叫的标识。                                 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "observedParticipantId",
    "onBehalfOf",
    "transferor"
  ],
  "@odata.type": "microsoft.graph.incomingContext"
}-->
```json
{
  "observedParticipantId": "String",
  "onBehalfOf": {"@odata.type": "#microsoft.graph.identitySet"},
  "sourceParticipantId": "String",
  "transferor": {"@odata.type": "#microsoft.graph.identitySet"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "incomingContext resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
