---
title: acl 资源类型
description: 由 Microsoft Search externalConnection 编制索引的项的访问控制项。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 6d390ac0fee3063bd8f0d292d14e04b2616c1d00
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193531"
---
# <a name="acl-resource-type"></a>acl 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

由 Microsoft Search [externalConnection](externalconnection.md)编制索引的项的访问控制项。

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a>属性

| 属性       | 类型   | 描述                                        |
|:---------------|:-------|:---------------------------------------------------|
| accessType     | 字符串 | 授予对标识的访问权限。 可取值为：`grant`、`deny`。 |
| identitySource | 字符串 | 标识源。 可能的值为 `azureActiveDirectory` 或 `external` 。           |
| type           | 字符串 | 标识的类型。 可能的值为： `user` 、 `group` 、、 `everyone` `everyoneExceptGuests` 如果 identitySource 是， `azureActiveDirectory` 并且只有 `group` identitySource 是 `external` 。 |
| value          | String | 标识的唯一标识符。 对于 Azure Active Directory 标识， `value` 将设置为用户、组或租户的类型为 user、group 和 everyone 的对象标识符 (和 everyoneExceptGuests) 分别。 如果将外部组 `value` 设置为 [EXTERNALGROUP](externalgroup.md)的 ID。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.acl",
  "baseType": null
}-->

```json
{
  "accessType": "String",
  "identitySource": "String",
  "type": "String",
  "value": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "acl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
