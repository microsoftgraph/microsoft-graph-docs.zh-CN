---
title: printerCreateOperation 资源类型
description: 表示长时间运行的打印机注册操作。 派生自 printOperation。
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 716c23603dd811ddad61dd604c9961d1df3f5297
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176532"
---
# <a name="printercreateoperation-resource-type"></a>printerCreateOperation 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示长时间运行的打印机注册操作。 派生自 [printOperation](printoperation.md)。

## <a name="methods"></a>方法

| 方法       | 返回类型 | Description |
|:-------------|:------------|:------------|
| [获取操作](../api/printoperation-get.md) | [printOperation](printoperation.md) | 检索当前用户或应用租户中长时间运行的操作。 |

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String|操作的标识符。 只读。|
|状态|[printOperationStatus](printoperationstatus.md)|注册操作的状态。 包含操作的进度以及是否已成功完成。 只读。|
|createdDateTime|DateTimeOffset|创建操作时的 DateTimeOffset。 只读。|
|证书|String|注册过程中创建的已签名证书。 只读。|
|打印机|[打印机](printer.md)|创建的打印机实体。 只读。|

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

