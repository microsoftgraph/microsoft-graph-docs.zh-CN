---
title: settingTemplateValue 资源类型
description: 表示单个模板设置定义，包括设置的默认值（如果未实例化该设置）。
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: e53a8f07f325b023deea32e01fe217feeb35f49d
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547048"
---
# <a name="settingtemplatevalue-resource-type"></a>settingTemplateValue 资源类型

命名空间：microsoft.graph

表示单个模板设置定义，包括设置的默认值（如果未实例化该设置）。

### <a name="properties"></a>属性

| 属性 | 类型 | 描述 |
|:---------------|:--------|:----------|
|defaultValue|字符串| 设置的默认值。 |
|说明|字符串| 设置的说明。 |
|name|字符串| 设置的名称。 |
|type|字符串| 设置的类型。 |

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

