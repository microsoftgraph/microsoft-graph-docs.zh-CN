---
title: settingTemplateValue 资源类型
description: 表示单个模板设置定义, 包括设置的默认值 (如果未实例化设置)。
localization_priority: Normal
ms.openlocfilehash: 2277f4b7bb66839164a1b09011d20886baf2bd1f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343183"
---
# <a name="settingtemplatevalue-resource-type"></a>settingTemplateValue 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示单个模板设置定义, 包括设置的默认值 (如果未实例化设置)。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|默认|string|设置的默认值。 只读。|
|说明|string|设置的说明。 只读。|
|name|string|设置的名称。 只读。|
|类型|string|设置的类型。 只读。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingTemplateValue"
}-->

```json
{
  "defaultValue": "string",
  "description": "string",
  "name": "string",
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "settingTemplateValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
