---
title: educationMakeCodeResource 资源类型
description: 一个 MakeCode 资源
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 5ffab7e11675996e79aed746cfe4624b28e37aab
ms.sourcegitcommit: f23cc661a0e30d01a6b59cfdae90768c55b80ae2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/08/2019
ms.locfileid: "37418284"
---
# <a name="educationmakecoderesource-resource-type"></a>educationMakeCodeResource 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

一个代表[MakeCode](https://www.microsoft.com/en-us/makecode)项目的资源。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|projectId|String|MakeCode 项目的 ID|
|hostWebUrl|String|MakeCode 资源类型的主机（例如，arcade、microbit）|

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
  "projectId": "String",
  "hostWebUrl": "String"
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