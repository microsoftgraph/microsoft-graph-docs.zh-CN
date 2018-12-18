---
title: WorksheetProtectionOptions 资源类型
description: 代表工作表保护中的选项。
author: lumine2008
ms.openlocfilehash: d7217c825e1ac1fef297882ddf984bc94b10cc12
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27335187"
---
# <a name="worksheetprotectionoptions-resource-type"></a>WorksheetProtectionOptions 资源类型

代表工作表保护中的选项。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|allowAutoFilter|boolean|表示允许使用自动筛选功能的工作表保护选项。|
|allowDeleteColumns|boolean|表示允许删除列的工作表保护选项。|
|allowDeleteRows|boolean|表示允许删除行的工作表保护选项。|
|allowFormatCells|boolean|表示允许格式化单元格的工作表保护选项。|
|allowFormatColumns|boolean|表示允许格式化列的工作表保护选项。|
|allowFormatRows|boolean|表示允许格式化行的工作表保护选项。|
|allowInsertColumns|boolean|表示允许插入列的工作表保护选项。|
|allowInsertHyperlinks|boolean|表示允许插入超链接的工作表保护选项。|
|allowInsertRows|boolean|表示允许插入行的工作表保护选项。|
|allowPivotTables|boolean|表示允许使用数据透视表功能的工作表保护选项。|
|allowSort|boolean|表示允许使用排序功能的工作表保护选项。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookWorksheetProtectionOptions"
}-->

```json
{
  "allowAutoFilter": true,
  "allowDeleteColumns": true,
  "allowDeleteRows": true,
  "allowFormatCells": true,
  "allowFormatColumns": true,
  "allowFormatRows": true,
  "allowInsertColumns": true,
  "allowInsertHyperlinks": true,
  "allowInsertRows": true,
  "allowPivotTables": true,
  "allowSort": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetProtectionOptions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->