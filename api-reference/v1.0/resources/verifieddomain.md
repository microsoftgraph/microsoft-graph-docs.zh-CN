---
title: verifiedDomain 资源类型
description: 指定租户的域。 组织实体的 verifiedDomains 属性是 verifiedDomain 对象的集合。
ms.localizationpriority: medium
author: Jumaodhiss
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 0205971eff906b6c4adb33490bd8e7ea6b3e3a5f
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2022
ms.locfileid: "65247243"
---
# <a name="verifieddomain-resource-type"></a>verifiedDomain 资源类型

命名空间：microsoft.graph

指定租户的域。 [组织](organization.md)实体 **的 verifiedDomains** 属性是 **verifiedDomain** 对象的集合。


## <a name="properties"></a>属性
| 属性     | 类型    | 说明                                                                          |
|:-------------|:--------|:-------------------------------------------------------------------------------------|
| capabilities | String  | 例如，`Email`、`OfficeCommunicationsOnline`。                                  |
| isDefault    | Boolean | `true` 如果这是与租户关联的默认域，否则， `false`. |
| isInitial    | Boolean | `true` 如果这是与租户关联的初始域，否则， `false`. |
| name         | String  | 域名;例如， `contoso.onmicrosoft.com`.                             |
| type         | String  | 例如，`Managed`。                                                              |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.verifiedDomain"
}-->

```json
{
  "capabilities": "String",
  "isDefault": true,
  "isInitial": true,
  "name": "String",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "verifiedDomain resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

