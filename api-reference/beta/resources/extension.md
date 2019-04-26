---
title: 扩展资源类型
description: 用以支持 OData v4 开放类型 openTypeExtension 的抽象类型。
localization_priority: Normal
ms.openlocfilehash: 33238d0addc1b3cc7797fc2a600b7b6195a8d9ea
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333919"
---
# <a name="extension-resource-type"></a>扩展资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用以支持 OData v4 开放类型 [openTypeExtension](opentypeextension.md) 的抽象类型。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
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

## <a name="relationships"></a>关系
无


## <a name="methods"></a>方法

请参阅派生类型 [openTypeExtension](opentypeextension.md) 的方法以了解实际支持的方法。


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "extension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
