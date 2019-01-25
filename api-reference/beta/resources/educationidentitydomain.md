---
title: educationIdentityDomain 资源类型
description: '代表教育用户类型和用户的帐户所属的域之间的映射。 域资源是标识创建配置的一部分。 '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 0c6004d18897b8f8284c06a3b09830072148df87
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528177"
---
# <a name="educationidentitydomain-resource-type"></a>educationIdentityDomain 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表教育用户类型和用户的帐户所属的域之间的映射。 域资源是[标识创建配置](educationidentitycreationconfiguration.md)的一部分。 

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:-|:-|:-|
| appliesTo | string |  要分配许可证的用户角色类型。 可取值为：`student`、`teacher`。      |
| **name** | string |  表示的用户帐户的域。         |

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationidentitydomain.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
