---
title: acl 资源类型
description: 由 externalConnection 索引的项的访问控制Microsoft 搜索项。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 339b5ab51fd604cae2dd42e2ec853ede8d27ef5b
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467648"
---
# <a name="acl-resource-type"></a>acl 资源类型

命名空间：microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

由[externalConnection](externalconnectors-externalconnection.md)索引的项的访问控制Microsoft 搜索项。

## <a name="properties"></a>属性

| 属性       | 类型   | 说明                                        |
|:---------------|:-------|:---------------------------------------------------|
| accessType     | String | 授予标识的访问权限。 可取值为：`grant`、`deny`。 |
| identitySource | String | 标识的来源。 可能的值为 `azureActiveDirectory` 或 `external`。           |
| type           | String | 标识的类型。 可能的值为 `user` `group` `everyone` `everyoneExceptGuests` ：、，如果 identitySource 为 且 `azureActiveDirectory` 只是 `group` identitySource 为 `external` 。 |
| value          | String | 标识的唯一标识。 如果Azure Active Directory，则分别设置为类型为 user、group 和 everyone (和 everyoneExceptGuests 的用户、组或租户) `value` 标识符。 对于外部组 `value` ，设置为 [externalGroup](externalconnectors-externalgroup.md)的 ID。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalConnectors.acl",
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
