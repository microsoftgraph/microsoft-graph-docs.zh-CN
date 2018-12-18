---
title: onenoteOperation 资源类型
description: 某些长时间运行的 OneNote 操作的状态。
author: Jewan-microsoft
ms.openlocfilehash: 7835c150cbc06915aa8d4e8f8bf1e1257f341ee4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27338673"
---
# <a name="onenoteoperation-resource-type"></a>onenoteOperation 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

某些长时间运行的 OneNote 操作的状态。

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
