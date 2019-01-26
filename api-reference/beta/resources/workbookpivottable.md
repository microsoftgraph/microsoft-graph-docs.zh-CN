---
title: pivotTable 资源类型
description: 表示 Excel 数据透视表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 774c407022d700bc5856dc780eff3a6dafa6bc4e
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577457"
---
# <a name="pivottable-resource-type"></a>pivotTable 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Excel 数据透视表。

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[Get workbookPivotTable](../api/workbookpivottable-get.md) | [workbookPivotTable](workbookpivottable.md) |读取 workbookPivotTable 对象的属性和关系。|
|[Refresh](../api/workbookpivottable-refresh.md)|无|刷新数据透视表。 |
|[Refreshall](../api/workbookpivottable-refreshall.md)|无|刷新给定工作表内的所有表。请注意，只能对数据透视表集合执行此操作。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|String| 数据透视表的 ID。 只读。|
|name|String|数据透视表对象的名称。    |

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|worksheet|[WorkbookWorksheet](worksheet.md)| 包含当前 PivotTable 对象的工作表。只读。   |

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookPivotTable"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String"
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/workbookpivottable.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
