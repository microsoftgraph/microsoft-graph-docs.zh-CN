---
title: educationMakeCodeResource 资源类型
description: 一个 MakeCode 资源
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: e983f217af71b6e27f750599ee2f8db295da5fec
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173368"
---
# <a name="educationmakecoderesource-resource-type"></a>educationMakeCodeResource 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

一个代表[MakeCode](https://www.microsoft.com/en-us/makecode)项目的资源。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|mkcd|String|MakeCode 项目的 ID|
|url|String|MakeCode 资源类型的主机 (例如, arcade、microbit)|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationMakeCodeResource",
  "baseType": "microsoft.graph.educationResource"
}-->

```json
{
  "mkcd": "String",
  "url": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationMakeCodeResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->