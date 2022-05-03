---
title: printOperation 资源类型
description: 表示长时间运行的通用打印操作。 打印机CreateOperation 等操作类型的基类。
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 5e3d53d9fbdc5fbb4dd1bda2aa477581df5c838e
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176663"
---
# <a name="printoperation-resource-type"></a>printOperation 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示长时间运行的通用打印操作。 打印 [机CreateOperation](printercreateoperation.md) 等操作类型的基类。

## <a name="methods"></a>方法

| 方法       | 返回类型 | Description |
|:-------------|:------------|:------------|
| [获取操作](../api/printoperation-get.md) | [printOperation](printoperation.md) | 检索当前用户或应用租户中长时间运行的操作。 |

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String|操作的标识符。 只读。|
|状态|[printOperationStatus](printoperationstatus.md)|操作的状态。 只读。|
|createdDateTime|DateTimeOffset|创建操作时的 DateTimeOffset。 只读。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printOperation",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
    "id": "String (identifier)",
    "status": {"@odata.type": "microsoft.graph.printOperationStatus"},
    "createdDateTime": "2020-06-15T19:54:14.853Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


