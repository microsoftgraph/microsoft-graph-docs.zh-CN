---
title: provisionedIdentity 资源类型
description: 描述与设置对象摘要事件关联的标识。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fb535bbba827f93b597c5e41efb128f2ad610ef2
ms.sourcegitcommit: e0de4e41773e361752870411d1b1a74270738127
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/28/2019
ms.locfileid: "35349339"
---
# <a name="provisionedidentity-resource-type"></a>provisionedIdentity 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

描述与设置对象摘要事件关联的标识。 

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|详细信息|[detailsInfo](detailsinfo.md)|标识的详细信息。|
|displayName|String|标识的显示名称。 |
|id|String|唯一标识标识。|
|identityType|String|已设置的标识类型, 如 "user" 或 "group"。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisionedIdentity",
  "baseType": null
}-->

```json
{
  "details": {"@odata.type": "microsoft.graph.detailsInfo"},
  "displayName": "String",
  "id": "String",
  "identityType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisionedIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
