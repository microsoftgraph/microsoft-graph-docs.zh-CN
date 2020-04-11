---
title: serviceInformation 资源类型
description: serviceInformation 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: daca733578e5415fc777bc01a8ef1272cfdcc681
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2020
ms.locfileid: "43228878"
---
# <a name="serviceinformation-resource-type"></a>serviceInformation 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关用户已从其帐户中选择要引用的云服务的基本描述性数据。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明                                                      |
|:-------------|:------------|:-----------------------------------------------------------------|
|name          | 字符串      | 云服务的名称（例如，Twitter、Instagram）。 |
|WebUrl        | String      | 包含要引用的服务的 URL。               |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.serviceInformation",
  "baseType": null
}-->

```json
{
  "name": "String",
  "webUrl": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "serviceInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
