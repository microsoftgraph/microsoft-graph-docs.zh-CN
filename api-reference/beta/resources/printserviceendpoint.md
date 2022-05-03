---
title: printServiceEndpoint 资源类型
description: 表示打印服务实例的 URI 和标识信息。
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 3c5d9085614b4c4ad99aa43cb8281a3123eb3741
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176753"
---
# <a name="printserviceendpoint-resource-type"></a>printServiceEndpoint 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示打印服务实例的 URI 和标识信息。

## <a name="methods"></a>方法

| 方法       | 返回类型 | Description |
|:-------------|:------------|:------------|
| [Get endpoint](../api/printserviceendpoint-get.md) | [printServiceEndpoint](printserviceendpoint.md) | 读取终结点对象的属性和关系。 |

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|displayName|String|终结点的可读显示名称。|
|name|字符串|标识终结点提供的服务的唯一名称。 可能的值包括： `discovery` (发现服务) 、 `notification` (通知服务) 、 `ipp` (IPP 服务) 和 `registration` (注册服务) 。 只读。|
|Uri|String|可用于访问服务的 URI。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printServiceEndpoint"
}-->

```json
{
  "displayName": "String",
  "name": "String (identifier)",
  "uri": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printServiceEndpoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

