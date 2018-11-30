---
title: networkLocationDetail 资源类型
description: 指示与的网络位置关联的详细信息。 .
ms.openlocfilehash: 5dd1410318d380a1b943de6a7dbb0d739172cc76
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045959"
---
# <a name="networklocationdetail-resource-type"></a>networkLocationDetail 资源类型
指示与的网络位置关联的详细信息。 .



## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|networkType|字符串|提供了网络的类型。 可能的值为`intranet`， `extranet`， `namedNetwork`，和`trusted`。|
|networkName|字符串|网络的名称。|


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.deviceDetail"
}-->

```json
{
  "networkTypes": "namedNetork",
  "networkName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "deviceDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->