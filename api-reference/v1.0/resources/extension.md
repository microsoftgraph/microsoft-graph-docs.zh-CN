---
title: 扩展资源类型
description: 用以支持 OData v4 开放类型 openTypeExtension 的抽象类型。
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 547570b70948590e72060432618005f02b8a167ba772cb39cd5290ea4134cdf8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54141712"
---
# <a name="extension-resource-type"></a>扩展资源类型

命名空间：microsoft.graph

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

## <a name="relationships"></a>关系
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

