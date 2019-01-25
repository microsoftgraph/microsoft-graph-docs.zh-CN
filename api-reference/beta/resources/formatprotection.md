---
title: FormatProtection 资源类型
description: 表示对 range 对象的格式保护。
localization_priority: Normal
ms.openlocfilehash: 7bc27060567136386ef1f08e6fe46e95980788a9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509187"
---
# <a name="formatprotection-resource-type"></a>FormatProtection 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示对 range 对象的格式保护。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|获取 FormatProtection | [FormatProtection](formatprotection.md) |读取 formatProtection 对象的属性和关系。|
|[Update](../api/formatprotection-update.md) | [FormatProtection](formatprotection.md)  |更新 FormatProtection 对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|formulaHidden|布尔|表示 Excel 是否隐藏区域中的单元格公式。指示整个区域不具有统一公式隐藏设置的空值。|
|已锁定|布尔|指示 Excel 是否锁定对象中的单元格。指示整个区域不具有统一锁定设置的空值。|

## <a name="relationships"></a>关系
无


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.formatProtection"
}-->

```json
{
  "formulaHidden": true,
  "locked": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "FormatProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/formatprotection.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
