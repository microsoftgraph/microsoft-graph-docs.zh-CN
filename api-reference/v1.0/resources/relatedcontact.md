---
title: relatedContact 资源类型
description: 表示与 educationUser 相关的联系人记录，该记录为监护人、帮助者、家长等提供相关信息。
author: marcla
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b5d833afe05480a1ae4e490220ad16755f268c7a
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589434"
---
# <a name="relatedcontact-resource-type"></a>relatedContact 资源类型

命名空间：microsoft.graph

表示与 [educationUser](../resources/educationuser.md) 相关的联系人记录，该记录为监护人、帮助者、家长等提供相关信息。

## <a name="properties"></a>属性

| 属性      | 类型                  | 说明                                                                                                                               |
| :------------ | :-------------------- | :---------------------------------------------------------------------------------------------------------------------------------------- |
| accessConsent | Boolean               | 指示用户是否已同意访问学生数据。                                                                     |
| displayName   | String                | 联系人的姓名。 必需项。                                                                                                            |
| emailAddress  | String                | 联系人的主电子邮件地址。 必需项。                                                                                           |
| mobilePhone   | String                | 联系人的移动电话号码。                                                                                                       |
| 关系  | contactRelationship | 与用户的关系。 可取值为：`parent`、`relative`、`aide`、`doctor`、`guardian`、`child`、`other`、`unknownFutureValue`。|

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
  "accessConsent": true,
  "displayName": "String",
  "emailAddress": "String",
  "mobilePhone": "String",
  "relationship": "String"
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
