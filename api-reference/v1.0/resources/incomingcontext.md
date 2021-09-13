---
title: incomingContext 资源类型
description: 表示与传入呼叫关联的上下文。
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 80f300fc4f3cf051466b37c4445272444fdc71bc
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59123354"
---
# <a name="incomingcontext-resource-type"></a>incomingContext 资源类型

命名空间：microsoft.graph

表示与传入呼叫关联的上下文。

## <a name="properties"></a>属性

| 属性              | 类型                          | 说明                                                             |
|:----------------------|:------------------------------|:------------------------------------------------------------------------|
| sourceParticipantId   | String                        | 触发传入呼叫的参与者的 ID。 只读。  |
| observedParticipantId | String                        | 正在观察的参与者的 ID。 只读。         |
| onBehalfOf            | [identitySet](identityset.md) | 代表进行呼叫的标识。                   |
| transferor            | [identitySet](identityset.md) | 转接呼叫的标识。                                 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "sourceParticipantId",
    "observedParticipantId",
    "onBehalfOf",
    "transferor"
  ],
  "@odata.type": "microsoft.graph.incomingContext"
}-->
```json
{
  "sourceParticipantId": "String",
  "observedParticipantId": "String",
  "onBehalfOf": {"@odata.type": "#microsoft.graph.identitySet"},
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

