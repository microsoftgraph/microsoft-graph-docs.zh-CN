---
title: educationSchool 资源类型
description: '学校。 **educationSchool**资源当前与 administrativeUnit 资源相对应并共享相同的 ID。  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 917395324e6ae519af468a4bb4b31056796e1498
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542920"
---
# <a name="educationschool-resource-type"></a>educationSchool 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

学校。 **educationSchool**资源当前与[administrativeUnit](administrativeunit.md)资源相对应并共享相同的 ID。  

此资源是[educationOrganization](educationorganization.md)的子类型。




## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[Get](../api/educationschool-get.md) | [educationSchool](educationschool.md) |读取 **educationSchool** 对象的属性和关系。|
|[Add class](../api/educationschool-post-classes.md) |[educationClass](educationclass.md)| 通过发布到课程导航属性，为学校添加一个新的 **educationClass**。|
|[List classes](../api/educationschool-list-classes.md) |[educationClass](educationclass.md) 集合| 获取 **educationClass** 对象集合。|
|[Remove class](../api/educationschool-delete-classes.md) |[educationClass](educationclass.md)| 通过课程导航属性从学校删除 **educationClass**。|
|[Add user](../api/educationschool-post-users.md) |[educationUser](educationuser.md)| 通过发布到 **users** 导航属性，为学校添加一个新的 **educationUser**。|
|[List users](../api/educationschool-list-users.md) |[educationUser](educationuser.md) 集合| 获取 **educationUser** 对象集合。|
|[Remove user](../api/educationschool-delete-users.md) |[educationUser](educationuser.md)| 通过 **users** 导航属性从学校删除 **educationUser**。|
|[获取 administrativeUnit](../api/educationschool-get-administrativeunit.md) |[administrativeUnit](administrativeunit.md)| 获取与此**educationSchool**相对应的**administrativeUnit** 。|
|[Update](../api/educationschool-update.md) | [educationSchool](educationschool.md) |更新 **educationSchool** 对象。 |
|[删除](../api/educationschool-delete.md) | 无 |删除 **educationSchool** 对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|String|该学校的 GUID。|
|displayName| String| 学校的显示名称。| 
|description| String | 学校描述。| 
|status| string| 只读。 可取值为：`inactive`、`active`、`expired`、`deleteable`。|
|externalSource| string| 只读。  可取值为：`sis`、`manual`、`unknownFutureValue`。|
|principalEmail| String| 主体的电子邮件地址。|
|principalName| String | 主体名称。|
|externalPrincipalId| String | 同步系统中主体的 ID。 |
|highestGrade|String| 教授的最高年级。 |
|lowestGrade|String| 教授的最低年级。 |
|schoolNumber|String| 学校编号。|
|externalId|String| 同步系统中学校的 ID。 |
|phone|String| 学校电话号码。 |
|fax|String| 学校传真号码。 |
|address|[physicalAddress](physicaladdress.md)| 学校地址。|
|createdBy|[identitySet](identityset.md)|创建了学校的实体。|


## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|classes|[educationClass](educationclass.md) 集合| 在学校教授的课程。 可为 NULL。|
|users|[educationUser](educationuser.md) 集合| 学校中的用户。 可为 Null。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSchool"
}-->

```json
{
  "id": "String",
  "displayName": "String",
  "description": "String",
  "status": "String",
  "externalSource": "String",
  "principalEmail": "String",
  "principalName": "String",
  "externalPrincipalId": "String",
  "highestGrade": "String",
  "lowestGrade": "String",
  "schoolNumber": "String",
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "externalId": "String",
  "fax": "String",
  "phone": "String",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationSchool resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationschool.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
