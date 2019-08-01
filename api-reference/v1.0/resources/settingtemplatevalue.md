---
title: settingTemplateValue 资源类型
description: 表示单个模板设置定义, 包括设置的默认值 (如果未实例化设置)。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f4ac39001e260d7f65b3a593d90976f94acd4693
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034389"
---
# <a name="settingtemplatevalue-resource-type"></a>settingTemplateValue 资源类型

表示单个模板设置定义, 包括设置的默认值 (如果未实例化设置)。

### <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
|默认|String| 设置的默认值。 |
|说明|String| 设置的说明。 |
|name|String| 设置的名称。 |
|type|String| 设置的类型。 |

### <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingTemplateValue"
}-->

```json
{
  "defaultValue": "String",
  "description": "String",
  "name": "String",
  "type": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "settingTemplateValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
