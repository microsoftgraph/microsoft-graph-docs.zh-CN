---
title: settingValue 资源类型
description: 由名称/值对表示的设置。
ms.localizationpriority: medium
author: dkershaw10
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 93d7fbfca62f4d34b3a2640c5ae6eb7e91c59a1a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59126644"
---
# <a name="settingvalue-resource-type"></a>settingValue 资源类型

命名空间：microsoft.graph

由名称/值对表示的设置。

### <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
|name|String| [groupSettingTemplate](groupsettingtemplate.md) (定义的设置) 。 |
|value|String| 设置的值。 |

### <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingValue"
}-->

```json
{
  "name": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "settingValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

