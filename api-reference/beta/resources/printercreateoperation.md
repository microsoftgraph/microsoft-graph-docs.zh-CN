---
title: printerCreateOperation 资源类型
description: 表示长时间运行的打印机注册操作。 派生自 printOperation。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 54f458e14cbda209d9c2d85f08df4c106db6ab00
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2020
ms.locfileid: "45007188"
---
# <a name="printercreateoperation-resource-type"></a>printerCreateOperation 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示长时间运行的打印机注册操作。 派生自[printOperation](printoperation.md)。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [Get 操作](../api/printoperation-get.md) | [printOperation](printoperation.md) | 在当前用户或应用程序的租户内检索长时间运行的操作。 |

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String|操作的标识符。 只读。|
|status|[printOperationStatus](printoperationstatus.md)|注册操作的状态。 包含操作的进度以及它是否成功完成。 只读。|
|createdDateTime|DateTimeOffset|创建操作时的 DateTimeOffset。 只读。|
|证书|String|注册过程中创建的签名证书。 只读。|
|印刷|[印刷](printer.md)|创建的打印机实体。 只读。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printerCreateOperation",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
    "id": "String (identifier)",
    "status": {"@odata.type": "microsoft.graph.printOperationStatus"},
    "createdDateTime": "2020-06-15T19:54:14.853Z",
    "certificate": "",
    "printer": {"@odata.type": "microsoft.graph.printer"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printerCreateOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->