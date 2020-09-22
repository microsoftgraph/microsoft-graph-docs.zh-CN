---
title: serviceInformation 资源类型
description: serviceInformation 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 39382b0fb17795bde26b4e54f629b2e4281f81db
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070441"
---
# <a name="serviceinformation-resource-type"></a>serviceInformation 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关用户已从其帐户中选择要引用的云服务的基本描述性数据。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明                                                      |
|:-------------|:------------|:-----------------------------------------------------------------|
|名称          | String      | 云服务的名称 (例如，Twitter、Instagram) 。 |
|webUrl        | String      | 包含要引用的服务的 URL。               |

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


