---
title: educationIdentityDomain 资源类型
description: '表示教育用户类型与用户帐户所属域之间的映射。 域资源是标识创建配置的一部分。 '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 5f4e23a9111d2515234d1aa665f4847d732dc563
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/28/2020
ms.locfileid: "45435038"
---
# <a name="educationidentitydomain-resource-type"></a>educationIdentityDomain 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示教育用户类型与用户帐户所属域之间的映射。 域资源是[标识创建配置](educationidentitycreationconfiguration.md)的一部分。

## <a name="properties"></a>属性

| 属性  | 类型   | 说明                                                                                        |
| :-------- | :----- | :------------------------------------------------------------------------------------------------- |
| appliesTo | String | 要分配给许可证的用户角色类型。 可取值为：`student`、`teacher`、`faculty`。 |
| name      | 字符串 | 代表用户帐户的域。                                                        |

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentityDomain"
}-->

```json
{
  "appliesTo": { "@odata.type": "microsoft.graph.educationUserRole" },
  "name": "String"
}
```
