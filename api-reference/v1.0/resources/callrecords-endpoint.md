---
title: 终结点资源类型
description: 终结点类型
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 4fe19bd5a69b456a0e74e70b118477131f7c8f2cb0011eac4270dad956d6667c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54252121"
---
# <a name="endpoint-resource-type"></a>终结点资源类型

命名空间：microsoft.graph.callRecords

表示呼叫中的终结点。 终结点可以是用户的设备、会议、应用程序/机器人等。 [participantEndpoint 和](callrecords-participantendpoint.md) [serviceEndpoint](callrecords-serviceendpoint.md) 类型继承自此类型。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|userAgent|[microsoft.graph.callRecords.userAgent](callrecords-useragent.md)|此终结点报告的用户代理。|

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
