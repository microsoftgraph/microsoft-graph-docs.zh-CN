---
title: educationIdentityDomain 资源类型
description: '表示教育用户类型与用户帐户所属域之间的映射。 域资源是标识创建配置的一部分。 '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b25f935ae404a243826a14c310a17ad80c598380
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095385"
---
# <a name="educationidentitydomain-resource-type"></a>educationIdentityDomain 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示教育用户类型与用户帐户所属域之间的映射。 域资源是 [标识创建配置](educationidentitycreationconfiguration.md)的一部分。

## <a name="properties"></a>属性

| 属性  | 类型   | 说明                                                                                        |
| :-------- | :----- | :------------------------------------------------------------------------------------------------- |
| appliesTo | String | 要分配给许可证的用户角色类型。 可取值为：`student`、`teacher`、`faculty`。 |
| 名称      | 字符串 | 代表用户帐户的域。                                                        |

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


