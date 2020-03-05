---
title: educationIdentityDomain 资源类型
description: '表示教育用户类型与用户帐户所属域之间的映射。 域资源是标识创建配置的一部分。 '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: a21d4d3005be8a776ae8bb9f9e3c1027be48de72
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42501925"
---
# <a name="educationidentitydomain-resource-type"></a>educationIdentityDomain 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示教育用户类型与用户帐户所属域之间的映射。 域资源是[标识创建配置](educationidentitycreationconfiguration.md)的一部分。 

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:-|:-|:-|
| **appliesTo** | string |  要分配给许可证的用户角色类型。 可取值为：`student`、`teacher`、`faculty`。      |
| **名称** | string |  代表用户帐户的域。         |

## <a name="json-representation"></a>JSON 表示形式
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentityDomain"
}-->

```json
{
    "appliesTo": {"@odata.type": "microsoft.graph.educationUserRole"},
    "name": "String"
}
```
