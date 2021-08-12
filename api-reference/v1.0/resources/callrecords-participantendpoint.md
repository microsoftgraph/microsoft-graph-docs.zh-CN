---
title: participantEndpoint 资源类型
description: participantEndpoint 类型
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d83690c1209d845f00dc902170eb547c567d6ec0cc654d6c9e9c3778da0fc275
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54223730"
---
# <a name="participantendpoint-resource-type"></a>participantEndpoint 资源类型

命名空间：microsoft.graph.callRecords

表示呼叫中的参与者终结点。 终结点表示用户或类似用户的实体。 继承自 [终结点](callrecords-endpoint.md) 类型。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|userAgent|[microsoft.graph.callRecords.userAgent](callrecords-useragent.md)|此终结点报告的用户代理。|
|反馈|[microsoft.graph.callRecords.userFeedback](callrecords-userfeedback.md)|此终结点的用户提供有关会话质量的反馈。|
|identity|[identitySet](identityset.md)|与终结点关联的标识。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.participantEndpoint",
  "baseType": "microsoft.graph.callRecords.endpoint"
}-->

```json
{
  "userAgent": {"@odata.type": "microsoft.graph.callRecords.userAgent"},
  "feedback": {"@odata.type": "microsoft.graph.callRecords.userFeedback"},
  "identity": {"@odata.type": "microsoft.graph.identitySet"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "participantEndpoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
