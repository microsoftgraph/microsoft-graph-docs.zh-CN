---
title: acl 资源类型
description: 由 Microsoft Search externalConnection 编制索引的项的访问控制项。
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 5a26004cf20a5f8c5c032eeade8f657fdf8bd93c
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703938"
---
# <a name="acl-resource-type"></a>acl 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

由 Microsoft Search [externalConnection](externalconnection.md)编制索引的项的访问控制项。

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a>属性

| 属性       | 类型   | 说明                                        |
|:---------------|:-------|:---------------------------------------------------|
| accessType     | String | 授予对标识的访问权限。 可取值为：`grant`、`deny`。 |
| identitySource | String | 必须设置为 `Azure Active Directory`。           |
| type           | String | 标识的类型。 可取值为：`user`、`group`、`everyone`、`everyoneExceptGuests`。 |
| value          | String | Azure Active Directory 标识符。 如果`type`为`user`或`group`， `value`则将设置为用户或组的对象标识符。 如果`type`为`everyone`或`everyoneExceptGuests`， `value`则将设置为 Azure Active Directory 租户的租户标识符。 |

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
