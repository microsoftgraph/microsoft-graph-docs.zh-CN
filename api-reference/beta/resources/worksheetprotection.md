---
title: WorksheetProtection 资源类型
description: 表示对 sheet 对象的保护。
ms.openlocfilehash: 8886117df669201a0c8a6f9fda1df18bb47cc4a4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048766"
---
# <a name="worksheetprotection-resource-type"></a>WorksheetProtection 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

表示对 sheet 对象的保护。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 WorksheetProtection](../api/worksheetprotection-get.md) | [WorksheetProtection](worksheetprotection.md) |读取 worksheetProtection 对象的属性和关系。|
|[Protect](../api/worksheetprotection-protect.md)|无|保护工作表。如果工作表处于受保护状态，则会引发它。|
|[Unprotect](../api/worksheetprotection-unprotect.md)|无|解除工作表保护|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|protected|boolean|表示该工作表是否受保护。只读。|

## <a name="relationships"></a>Relationships
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|选项|[WorksheetProtectionOptions](worksheetprotectionoptions.md)|工作表保护选项。只读。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.worksheetProtection"
}-->

```json
{
  "protected": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->