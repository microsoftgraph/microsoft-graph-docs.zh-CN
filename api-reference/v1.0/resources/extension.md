---
title: 扩展资源类型
description: 用以支持 OData v4 开放类型 openTypeExtension 的抽象类型。
ms.openlocfilehash: 1b3d735e0997ca128b539bff9a05c9c7c56799df
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007867"
---
# <a name="extension-resource-type"></a>扩展资源类型

用以支持 OData v4 开放类型 [openTypeExtension](opentypeextension.md) 的抽象类型。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "abstract": "true",
  "baseType": "microsoft.graph.entity",
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.extension"
}-->

```json
{
  "id": "string (identifier)"
}

```
## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|String| 只读。|

## <a name="relationships"></a>Relationships
无


## <a name="methods"></a>方法

请参阅派生类型 [openTypeExtension](opentypeextension.md) 的方法以了解实际支持的方法。


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "extension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->