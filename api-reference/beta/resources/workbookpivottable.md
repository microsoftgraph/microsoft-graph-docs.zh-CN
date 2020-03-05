---
title: workbookPivotTable 资源类型
description: 表示 Excel 数据透视表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: a086a5f91ad93497b6aa1d841e5baa7ee7e72f96
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519202"
---
# <a name="workbookpivottable-resource-type"></a>workbookPivotTable 资源类型

命名空间： microsoft. graph

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
|worksheet|[workbookWorksheet](workbookworksheet.md)| 包含当前 PivotTable 对象的工作表。 只读。   |

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
