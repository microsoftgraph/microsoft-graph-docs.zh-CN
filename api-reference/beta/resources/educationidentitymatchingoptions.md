---
title: educationIdentityMatchingOptions 资源类型
description: 提供源属性和目标属性之间用于匹配用户帐户的映射。 Source 属性应存在于源数据中。 目标属性应为 Azure Active Directory (Azure AD) 中的有效属性。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 37ebb55fdd5457841ca0083c18518babca7565c4
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/07/2019
ms.locfileid: "34750148"
---
# <a name="educationidentitymatchingoptions-resource-type"></a>educationIdentityMatchingOptions 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

提供源属性和目标属性之间用于匹配用户帐户的映射。 Source 属性应存在于源数据中。 目标属性应为 Azure Active Directory (Azure AD) 中的有效属性。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:-|:-|:-|
| **appliesTo** | string |  要分配给许可证的用户角色类型。 可取值为：`student`、`teacher`、`faculty`。      |
| **sourcePropertyName** | string |  Source 属性的名称, 该名称应为源数据中的字段名称。 此属性区分大小写。        |
| **targetPropertyName** | string |  目标属性的名称, 该名称应为 Azure AD 中的有效属性。 此属性区分大小写。     |
| **targetDomain** | string |  要与要在目标中匹配的 source 属性后缀的域。 如果提供为 null, 则 source 属性将用于与目标属性匹配。        |

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
