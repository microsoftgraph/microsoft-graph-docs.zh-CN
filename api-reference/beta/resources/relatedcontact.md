---
title: relatedContact 资源类型
description: 与为监护人、工具、医生等提供信息的 educationUser 相关的联系人记录。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 66c4329b6c81d3bad38583ccf963bb4c6bb08f50
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48042406"
---
# <a name="relatedcontact-resource-type"></a>relatedContact 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

与为监护人、工具、医生等提供信息的 [educationUser](../resources/educationuser.md) 相关的联系人记录。

## <a name="properties"></a>属性

| 属性      | 类型                  | 说明                                                                                                         |
| :------------ | :-------------------- | :------------------------------------------------------------------------------------------------------------------ |
| id            | String                | Azure Active Directory 中的联系人的标识。                                                              |
| displayName   | String                | 联系人的名称。 必需。                                                                                      |
| emailAddress  | String                | 联系人的主电子邮件地址。                                                                               |
| mobilePhone   | String                | 联系人的移动电话号码。                                                                                 |
| 关系  | `contactRelationship` | 与用户的关系。 可能的值为、、、、、 `parent` `relative` `aide` `doctor` `guardian` `child` 、 `other` 。 |
| accessConsent | Boolean               | 指示用户是否同意访问学生数据。                                               |

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


