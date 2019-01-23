---
title: educationIdentityMatchingOptions 资源类型
description: 提供用于匹配的用户帐户的 source 属性和目标属性之间的映射。 Source 属性应存在的源数据中。 目标属性应为 Azure Active Directory (Azure AD) 中的有效属性。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: c2b092d5589cdccccfe73a7e71afcafa7b555a90
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425790"
---
# <a name="educationidentitymatchingoptions-resource-type"></a>educationIdentityMatchingOptions 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

提供用于匹配的用户帐户的 source 属性和目标属性之间的映射。 Source 属性应存在的源数据中。 目标属性应为 Azure Active Directory (Azure AD) 中的有效属性。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:-|:-|:-|
| **appliesTo** | string |  要分配许可证的用户角色类型。 可取值为：`student`、`teacher`。      |
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
