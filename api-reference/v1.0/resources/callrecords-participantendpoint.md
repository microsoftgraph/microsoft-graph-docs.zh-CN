---
title: participantEndpoint 资源类型
description: ParticipantEndpoint 类型
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: ff590acb76d50da9d0772bdaece805a1db0cd26a
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44492021"
---
# <a name="participantendpoint-resource-type"></a>participantEndpoint 资源类型

命名空间：microsoft.graph.callRecords

表示呼叫中的参与者终结点。 终结点表示用户或用户-like 实体。 从[终结点](callrecords-endpoint.md)类型继承。

## <a name="properties"></a>属性

| 属性     | 类型        | Description |
|:-------------|:------------|:------------|
|userAgent|[callRecords。 userAgent](callrecords-useragent.md)|此终结点报告的用户代理。|
|反馈|[callRecords。 userFeedback](callrecords-userfeedback.md)|此终结点的用户提供的有关会话质量的反馈。|
|窃取|[identitySet](identityset.md)|与终结点关联的标识。|

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