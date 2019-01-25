---
title: educationIdentityMatchingOptions 资源类型
description: 提供用于匹配的用户帐户的 source 属性和目标属性之间的映射。 Source 属性应存在的源数据中。 目标属性应为 Azure Active Directory (Azure AD) 中的有效属性。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 723a74cff1d5a660272d3456e9f54de8a54e21bc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513702"
---
# <a name="educationidentitymatchingoptions-resource-type"></a>educationIdentityMatchingOptions 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

提供用于匹配的用户帐户的 source 属性和目标属性之间的映射。 Source 属性应存在的源数据中。 目标属性应为 Azure Active Directory (Azure AD) 中的有效属性。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:-|:-|:-|
| appliesTo | string |  要分配许可证的用户角色类型。 可取值为：`student`、`teacher`。      |
| **sourcePropertyName** | string |  Source 属性，应该是源数据中的字段名称的名称。 此属性是区分大小写。        |
| **targetPropertyName** | string |  目标属性，应为 Azure AD 中的有效属性名称。 此属性是区分大小写。     |
| **targetDomain** | string |  使用 source 属性以匹配目标后缀域。 如果提供为 null，source 属性将用于与目标属性相匹配。        |

## <a name="json-representation"></a>JSON 表示形式
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentityMatchingOptions"
}-->

```json
{
    "appliesTo": {"@odata.type": "microsoft.graph.educationUserRole"},
    "sourcePropertyName": "String",
    "targetPropertyName": "String",
    "targetDomain": "String"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationidentitymatchingoptions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
