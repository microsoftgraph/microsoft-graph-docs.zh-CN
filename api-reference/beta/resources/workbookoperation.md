---
title: workbookOperation 资源类型
description: 表示长时间运行的工作簿操作的状态。
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: bd015045b01d0a7f886ecf0f5165a347d76dc061
ms.sourcegitcommit: b469176f49aacbd02cd06838cc7c8d36cf5bc768
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2020
ms.locfileid: "45165125"
---
# <a name="workbookoperation-resource-type"></a>workbookOperation 资源类型

表示长时间运行的工作簿操作的状态。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [获取 workbookOperation](../api/workbookoperation-get.md) | [workbookOperation](workbookoperation.md) | 检索**workbookOperation**对象的状态。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String| 操作 id。只读。|
|状态|String| 操作的当前状态。 可取值为：`notStarted`、`running`、`succeeded`、`failed`。|
|error|[workbookOperationError](workbookoperationerror.md)| 操作返回的错误。|
|resourceLocation|String| 结果的资源 URI。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookOperation",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "status": {"@odata.type": "microsoft.graph.workbookOperationStatus"},
  "error": {"@odata.type": "microsoft.graph.workbookOperationError"},
  "resourceLocation": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workbookOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
