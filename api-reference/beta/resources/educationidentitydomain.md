---
title: educationIdentityDomain 资源类型
description: '表示教育用户类型与用户帐户所属域之间的映射。 域资源是标识创建配置的一部分。 '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 5cf7444c51b34ae4a8eacf9c99fdfd085dbec896
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334262"
---
# <a name="educationidentitydomain-resource-type"></a>educationIdentityDomain 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示教育用户类型与用户帐户所属域之间的映射。 域资源是[标识创建配置](educationidentitycreationconfiguration.md)的一部分。 

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:-|:-|:-|
| **appliesTo** | string |  要分配给许可证的用户角色类型。 可取值为：`student`、`teacher`。      |
| **name** | string |  代表用户帐户的域。         |

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
