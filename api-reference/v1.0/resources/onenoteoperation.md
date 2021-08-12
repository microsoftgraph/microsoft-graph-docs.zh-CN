---
title: onenoteOperation 资源类型
description: 某些长时间运行的操作的状态OneNote状态。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: dd7d6cfc797416d0cc8922dac8305617bc46c4c8d26e0e138551a0f855cadcbb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54146445"
---
# <a name="onenoteoperation-resource-type"></a>onenoteOperation 资源类型

命名空间：microsoft.graph

某些长时间运行的操作的状态OneNote状态。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.operation",
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
|createdDateTime| DateTimeOffset |操作开始时间。|
|error|[onenoteOperationError](onenoteoperationerror.md)|操作返回的错误。|
|id|string|操作 ID。只读。|
|lastActionDateTime| DateTimeOffset |操作的最后一个操作的时间。|
|resourceId|string|资源 ID。|
|resourceLocation|string|对象的资源 URI。 例如，复制的页面或节的资源 URI。 |
|status|operationStatus|操作的当前状态 `NotStarted` `Running` ：、、、。 `Completed` `Failed` |
|percentComplete|string|如果操作仍处于状态，则操作完成百 `running` 分比。|

## <a name="relationships"></a>关系
无


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取操作](../api/onenoteoperation-get.md) | [onenoteOperation](onenoteoperation.md) |获取操作的状态。 |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

