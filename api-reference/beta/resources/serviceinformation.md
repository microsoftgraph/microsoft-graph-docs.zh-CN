---
title: serviceInformation 资源类型
description: serviceInformation 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: ba13967a2b4373c1a3599baf2fcc856967fbb00c
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939829"
---
# <a name="serviceinformation-resource-type"></a>serviceInformation 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关用户已从其帐户中选择要引用的云服务的基本描述性数据。

## <a name="properties"></a>属性

| 属性     | 类型        | 描述                                            |
|:-------------|:------------|:-------------------------------------------------------|
|name          | 字符串      | 云服务的名称（例如，Twitter、Instagram）。 |
|webUrl        | String      | 包含要引用的服务的 URL。     |

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
