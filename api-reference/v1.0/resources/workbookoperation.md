---
title: workbookOperation 资源类型
description: 表示长时间运行的工作簿操作的状态。
ms.localizationpriority: medium
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 0ec98d72f56eb2f066f221a0c7aadc389d01109b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134162"
---
# <a name="workbookoperation-resource-type"></a>workbookOperation 资源类型

表示长时间运行的工作簿操作的状态。


## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [获取 workbookOperation](../api/workbookoperation-get.md) | [workbookOperation](workbookoperation.md) | 使用 获取 操作 `{operation-id}` 。 |


## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|status|String| 操作的当前状态。 可取值为：`NotStarted`、`Running`、`Completed`、`Failed`。|
|id|String| 操作 ID。只读。|
|error|[workbookOperationError](workbookoperationerror.md)| 操作返回的错误。|
|resourceLocation|String| 结果的资源 URI。|

## <a name="relationships"></a>关系

无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookOperation",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "status": {"@odata.type": "microsoft.graph.workbookOperationStatus"},
  "error": {"@odata.type": "microsoft.graph.workbookOperationError"},
  "resourceLocation": "String",
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
