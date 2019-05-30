---
title: educationClass 资源类型
description: '表示学校的课程。 **educationClass** 资源对应于 Office 365 组并共享同一个 ID。 学生是课程的正式成员，教师为所有者，且具有相应权限。 若要使 Office 体验正常进行，教师必须同时为教师和成员集合的成员。  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: dfce83c99ec886a01c2c52c3bae58c91b12fa0b0
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536167"
---
# <a name="educationclass-resource-type"></a>educationClass 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示学校的课程。 **educationClass** 资源对应于 Office 365 组并共享同一个 ID。 学生是课程的正式成员，教师为所有者，且具有相应权限。 若要使 Office 体验正常进行，教师必须同时为教师和成员集合的成员。  


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[Get educationClass](../api/educationclass-get.md) | [educationClass](educationclass.md) |读取 **educationClass** 对象的属性和关系。|
|[Add member](../api/educationclass-post-members.md) |[educationUser](educationuser.md)| 通过发布到 members 导航属性，为课程添加一个新的 **educationUser**。|
|[List members](../api/educationclass-list-members.md) |[educationUser](educationuser.md) 集合| 获取 **educationUser** 对象集合。|
|[Remove student](../api/educationclass-delete-members.md) |[educationUser](educationuser.md)| 通过成员导航属性从课程删除 **educationUser**。|
|[List schools](../api/educationclass-list-schools.md) |[educationSchool](educationschool.md) 集合| 获取 **educationSchool** 对象集合。|
|[Add teacher](../api/educationclass-post-teachers.md) |[educationUser](educationuser.md)| 通过发布到 teachers 导航属性，为课程添加一个新的 **educationUser**。|
|[List teachers](../api/educationclass-list-teachers.md) |[educationUser](educationuser.md) 集合| 获取课程的教师列表。|
|[Remove teacher](../api/educationclass-delete-teachers.md) |[educationUser](educationuser.md)| 通过教师导航属性从课程删除 **educationUser**。|
|[创建 educationAssignment](../api/educationclass-post-assignments.md) |[educationAssignment](../resources/educationassignment.md)| 通过发布到工作分配集合创建新的**educationAssignment** 。|
|[列出作业](../api/educationclass-list-assignments.md) |[educationAssignment](../resources/educationassignment.md)集合| 获取**educationAssignment**对象集合。|
|[Get group](../api/educationclass-get-group.md) |[组](group.md)| 获得与此 **educationClass** 对应的 Office 365 **group**。|
|[创建 educationCategory](../api/educationclass-post-category.md) | [educationCategory](educationcategory.md) | 为此类创建新的**educationCategory** 。|
|[List categories](../api/educationclass-list-categories.md) | [educationCategory](educationcategory.md)集合 | 获取属于此类的**educationCategory**对象的列表。|
|[Update](../api/educationclass-update.md) | [educationClass](educationclass.md)    |更新 **educationClass** 对象。 |
|[删除](../api/educationclass-delete.md) | 无 |删除 **educationClass** 对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id| 字符串| 课程的唯一标识符。|
|说明|String| 课程说明。|
|displayName|String| 课程名称。|
|mailNickname|字符串| 向所有成员发送电子邮件的邮件名称（如果已启用）。 |
|createdBy|[identitySet](identityset.md)| 创建了课程的实体 |
|classCode|String| 学校用于标识课程的课程代码。|
|externalId|String| 来自同步系统的课程 ID。 |
|externalName|String|同步系统中的课程名称。|
|externalSource|string| 此课程的创建方式。 可取值为：`sis`、`manual`、`unknownFutureValue`。|
|term|[educationTerm](educationterm.md)|此课程的学期。|


## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|成员|[educationUser](../resources/educationuser.md) 集合| 课程中的所有用户。 可为 Null。|
|schools|[educationSchool](../resources/educationschool.md) 集合| 与此课程相关的所有学校。 可为 Null。|
|teachers|[educationUser](../resources/educationuser.md) 集合|  课程中的所有教师。 可为 NULL。|
|assignments|[educationAssignment](../resources/educationassignment.md)集合| 与此类关联的所有工作分配。 可为 Null。|
|categories|[educationCategory](../resources/educationassignment.md)集合| 与此类关联的所有类别。 可为 Null。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationClass"
}-->

```json
{
  "id": "String",
  "description": "String",
  "classCode": "String",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "displayName": "String",
  "externalId": "String",
  "externalName": "String",
  "externalSource": "string",
  "mailNickname": "String",
  "term": {"@odata.type": "microsoft.graph.educationTerm"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationClass resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
