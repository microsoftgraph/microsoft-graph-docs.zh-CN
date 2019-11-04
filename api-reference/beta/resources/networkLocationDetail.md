---
title: networkLocationDetail 资源类型
description: 提供用户登录时所采用的网络的名称和类型。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8cbf60f7e7e370c5813623643f9d14cb324950cc
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939507"
---
# <a name="networklocationdetail-resource-type"></a>networkLocationDetail 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

提供用户登录时所采用的网络的名称和类型。

## <a name="properties"></a>属性

| 属性     | 类型        | 描述 |
|:-------------|:------------|:------------|
|networkNames|String collection|提供登录时使用的网络的名称。|
|网络|网络| 提供登录时使用的网络类型。 可取值为：`intranet`、`extranet`、`namedNetwork`、`trusted`、`unknownFutureValue`。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.networkLocationDetail",
  "baseType": null
}-->

```json
{
  "networkNames": ["String"],
  "networkType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "networkLocationDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->