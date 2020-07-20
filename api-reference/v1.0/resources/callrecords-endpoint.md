---
title: 终结点资源类型
description: 终结点类型
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 0dc1c8709eca693e883d03dfe96c869a021e799c
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44491948"
---
# <a name="endpoint-resource-type"></a>终结点资源类型

命名空间：microsoft.graph.callRecords

表示调用中的终结点。 终结点可以是用户的设备、会议、应用程序/机器人等。[ParticipantEndpoint](callrecords-participantendpoint.md)和[serviceEndpoint](callrecords-serviceendpoint.md)类型继承自此类型。

## <a name="properties"></a>属性

| 属性     | 类型        | Description |
|:-------------|:------------|:------------|
|userAgent|[callRecords。 userAgent](callrecords-useragent.md)|此终结点报告的用户代理。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.endpoint",
  "baseType": null
}-->

```json
{
  "userAgent": {"@odata.type": "microsoft.graph.callRecords.userAgent"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "endpoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->