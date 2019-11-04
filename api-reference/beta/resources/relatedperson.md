---
title: relatedPerson 资源类型
description: relatedPerson 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 6be6300bc901305fb87b04e2482f145b9187f9fb
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939234"
---
# <a name="relatedperson-resource-type"></a>relatedPerson 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关与用户的[配置文件](profile.md)中给定实体内的信息相关的人员的信息。

## <a name="properties"></a>属性

| 属性        | 类型        | 说明                                               |
|:----------------|:------------|:----------------------------------------------------------|
|displayName      |String       | 人员的姓名。                                        |
|关系     |字符串       | 可取值为：`manager`、`colleague`、`directReport`、`dotLineReport`、`assistant`、`dotLineManager`、`alternateContact`、`friend`、`spouse`、`sibling`、`child`、`parent`、`sponsor`、`emergencyContact`、`other`、`unknownFutureValue`。|
|userPrincipalName|字符串       | 组织内的人员的电子邮件地址或引用。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.relatedPerson",
  "baseType": null
}-->

```json
{
  "displayName": "String",
  "relationship": "String",
  "userPrincipalName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "relatedPerson resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
