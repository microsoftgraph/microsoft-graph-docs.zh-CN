---
title: WorksheetProtectionOptions 资源类型
description: 代表工作表保护中的选项。
ms.openlocfilehash: 2944663c62edd6533a12afe8e24cdd4f84f038fc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042712"
---
# <a name="worksheetprotectionoptions-resource-type"></a>WorksheetProtectionOptions 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

表示工作表保护选项。

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
  "@odata.type": "microsoft.graph.worksheetProtectionOptions"
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