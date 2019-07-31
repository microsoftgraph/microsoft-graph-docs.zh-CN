---
title: educationAssignmentResource 资源类型
description: 一个包装对象, 该对象存储与工作分配相关联的资源。 该包装添加了**distributeForStudentWork**属性, 并指示该资源将
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 60181a2289b272809cff025abeee83c594ae833e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006428"
---
# <a name="educationassignmentresource-resource-type"></a>educationAssignmentResource 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

一个包装对象, 该对象存储与工作分配相关联的资源。 该包装将添加**distributeForStudentWork**属性, 并指示该资源将被复制到学生提交。  如果不复制该对象, 则每个学生都将看到该工作分配的资源的链接。 学生将不能更新此资源。 这是教师向学生提供的讲义, 无需将其打开。 如果分配资源, 每个学生都会在其提交的资源列表中收到此资源的副本。 每个学生都可以修改其副本并将其提交到评分。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 educationAssignmentResource](../api/educationassignmentresource-get.md) | [educationAssignmentResource](educationassignmentresource.md) |读取**educationAssignmentResource**对象的属性和关系。|
|[更新](../api/educationassignmentresource-update.md) | [educationAssignmentResource](educationassignmentresource.md) |更新**educationAssignmentResource**对象。 |
|[删除](../api/educationassignmentresource-delete.md) | 无 |删除**educationAssignmentResource**对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|distributeForStudentWork|Boolean|指示是否应将此资源复制到每个提交的学生进行修改和提交。|
|id|String| 此资源的 ID。 只读。|
|resource|[educationResource](educationresource.md)|与此工作分配相关联的资源对象。|

## <a name="relationships"></a>关系
无。


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentResource"
}-->

```json
{
  "distributeForStudentWork": true,
  "id": "String (identifier)",
  "resource": {"@odata.type": "microsoft.graph.educationResource"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
