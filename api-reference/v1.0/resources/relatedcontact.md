---
title: relatedContact 资源类型
description: 联系人与提供的监护人、 工具、 医生，等信息 educationUser 相关的记录。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 7e3829de2ffeb073d8360976ce70d13985fcae39
ms.sourcegitcommit: d6209114cbbe8072e3ecf7eba23819ae5ace7db5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/01/2019
ms.locfileid: "29694487"
---
# <a name="realtedcontact-resource-type"></a>realtedContact 资源类型

联系人与提供的监护人、 工具、 医生，等信息[educationUser](../resources/educationuser.md)相关的记录。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|字符串|在 Azure Active Directory 联系人的标识。|
|displayName|String|联系人的姓名。 必需。|
|emailAddress|String|该联系人的主电子邮件地址。|
|mobilePhone|String|联系人的移动电话号码。|
|关系|`contactRelationship`|向用户的关系。 可能的值为`parent`， `relative`， `aide`， `doctor`， `guardian`， `child`， `other`， `unknownFutureValue`。|
|accessConsent|布尔|指示是否用户具有已同意访问学生数据。|

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
