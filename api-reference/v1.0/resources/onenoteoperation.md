---
title: onenoteOperation 资源类型
description: 某些长时间运行的 OneNote 操作的状态。
ms.openlocfilehash: 913562abf1d2f644bd621268c93768c7500f4399
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011608"
---
# <a name="onenoteoperation-resource-type"></a>onenoteOperation 资源类型

某些长时间运行的 OneNote 操作的状态。

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
|createdDateTime| DateTimeOffset |操作的开始时间。|
|error|[onenoteOperationError](onenoteoperationerror.md)|操作返回的错误。|
|id|string|操作 ID。只读。|
|lastActionDateTime| DateTimeOffset |操作的上次活动时间。|
|resourceId|string|资源 ID。|
|resourceLocation|string|对象的资源 URI。例如，复制页面或分区的资源 URI。 |
|status|string|操作的当前状态：`notstarted`、`running`、`completed`、`failed` |
|percentComplete|string|操作仍处于 `running` 状态时操作的完成百分比

## <a name="relationships"></a>关系
无


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[Get operation](../api/onenoteoperation-get.md) | [onenoteOperation](onenoteoperation.md) |获取操作状态。 |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
