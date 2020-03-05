---
title: workbookWorksheetProtection 资源类型
description: 表示对工作表对象的保护。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: ab5d3101b1b9cabf8843d3726f036de74bf3a258
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519097"
---
# <a name="workbookworksheetprotection-resource-type"></a>workbookWorksheetProtection 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示对工作表对象的保护。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 workbookWorksheetProtection](../api/worksheetprotection-get.md) | [workbookWorksheetProtection](workbookworksheetprotection.md) |读取 workbookWorksheetProtection 对象的属性和关系。|
|[保护](../api/worksheetprotection-protect.md)|无|保护工作表。如果工作表处于受保护状态，则会引发它。|
|[解除保护](../api/worksheetprotection-unprotect.md)|无|解除工作表保护|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|选项|[workbookWorksheetProtectionOptions](workbookworksheetprotectionoptions.md)|工作表保护选项。 只读。|
|protected|boolean|表示该工作表是否受保护。只读。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "options"
  ],
  "@odata.type": "microsoft.graph.workbookWorksheetProtection"
}-->

```json
{
  "protected": "boolean"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "workbookWorksheetProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
