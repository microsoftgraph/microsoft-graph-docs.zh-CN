---
title: settingTemplateValue 资源类型
description: 表示单个模板设置定义，包括设置的默认值（如果未实例化该设置）。
ms.localizationpriority: medium
author: dkershaw10
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 307161ccb879985942f0973b29fc4cbc370c230c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59126651"
---
# <a name="settingtemplatevalue-resource-type"></a>settingTemplateValue 资源类型

命名空间：microsoft.graph

表示单个模板设置定义，包括设置的默认值（如果未实例化该设置）。

### <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
|defaultValue|String| 设置的默认值。 |
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

