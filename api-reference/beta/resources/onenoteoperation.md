---
title: onenoteOperation 资源类型
description: 特定的长时间运行的 OneNote 操作的状态。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 9e427776d1a001ad3be9badca2dd731c2b42a057
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039200"
---
# <a name="onenoteoperation-resource-type"></a>onenoteOperation 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

特定的长时间运行的 OneNote 操作的状态。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteOperation"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "error": {"@odata.type": "microsoft.graph.onenoteOperationError"},
  "id": "string (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "resourceId": "string",
  "resourceLocation": "string",
  "status": "string",
  "percentComplete": "string"
}

```
## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|createdDateTime| DateTimeOffset |操作的开始时间。|
|error|[onenoteOperationError](onenoteoperationerror.md)|操作返回的错误。|
|id|string|操作 id。只读。|
|lastActionDateTime| DateTimeOffset |操作的上一操作的时间。|
|resourceId|string|资源 id。|
|resourceLocation|string|对象的资源 URI。 例如，复制的页或节的资源 URI。 |
|状态|string|操作的当前状态： `notstarted` 、 `running` 、 `completed` 、 `failed` |
|percentComplete|string|如果操作仍处于状态，则操作完成百分比为 `running`

## <a name="relationships"></a>关系
无


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[Get 操作](../api/onenoteoperation-get.md) | [onenoteOperation](onenoteoperation.md) |获取操作的状态。 |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onenoteOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


