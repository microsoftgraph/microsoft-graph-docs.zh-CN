---
title: relatedContact 资源类型
description: 与为监护人、工具、医生等提供信息的 educationUser 相关的联系人记录。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ce1ff84abb6704255267b521c67e5fc7b231b7df
ms.sourcegitcommit: e4b0211db9b20dfea8be964003661cd99fe064d1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/10/2019
ms.locfileid: "37439932"
---
# <a name="relatedcontact-resource-type"></a>relatedContact 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

与为监护人、工具、医生等提供信息的[educationUser](../resources/educationuser.md)相关的联系人记录。

## <a name="properties"></a>属性

| 属性      | 类型                  | 说明                                                                                                         |
| :------------ | :-------------------- | :------------------------------------------------------------------------------------------------------------------ |
| id            | 字符串                | Azure Active Directory 中的联系人的标识。                                                              |
| displayName   | 字符串                | 联系人的名称。 必需。                                                                                      |
| emailAddress  | String                | 联系人的主电子邮件地址。                                                                               |
| mobilePhone   | String                | 联系人的移动电话号码。                                                                                 |
| 关系  | `contactRelationship` | 与用户的关系。 可能的值`parent`为`relative`、 `aide` `doctor` `guardian`、、、 `child`、 `other`、。 |
| accessConsent | 布尔               | 指示用户是否同意访问学生数据。                                               |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.relatedContact"
}-->

```json
{
  "id": "String",
  "displayName": "String",
  "emailAddress": "String",
  "mobilePhone": "String",
  "relationship": "contactRelationship",
  "accessConsent": true
}
```

<!-- uuid: 720F9AB6-6E7A-4A66-8B0A-37A556FF99C5
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "relatedContact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
