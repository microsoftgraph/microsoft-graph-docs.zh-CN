---
title: relatedContact 资源类型
description: 与教育用户相关的联系人记录为监护人、助手、儿童等提供相关信息。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 3a99702811601278c1d3bbe4413fec495b8ba2d6bd13b23dafd90b3ff86f7c19
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54237528"
---
# <a name="relatedcontact-resource-type"></a>relatedContact 资源类型

命名空间：microsoft.graph

与教育用户相关的联系人 [记录为](../resources/educationuser.md) 监护人、助手、儿童等提供相关信息。

## <a name="properties"></a>属性

| 属性      | 类型                  | 说明                                                                                                                               |
| :------------ | :-------------------- | :---------------------------------------------------------------------------------------------------------------------------------------- |
| id            | String                | 联系人在内部Azure Active Directory。                                                                                    |
| displayName   | String                | 联系人的姓名。 必填。                                                                                                            |
| emailAddress  | String                | 联系人的主电子邮件地址。                                                                                                     |
| mobilePhone   | String                | 联系人的移动电话号码。                                                                                                       |
| 关系  | `contactRelationship` | 与用户的关系。 可能的值是 `parent` `relative` `aide` 、、、、、、、、 `doctor` `guardian` `child` `other` `unknownFutureValue` 。 |
| accessConsent | Boolean               | 指示用户是否已同意访问学生数据。                                                                     |

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

