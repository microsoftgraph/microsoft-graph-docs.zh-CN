---
title: educationAssignmentResource 资源类型
description: 一个包装对象，用于存储与工作分配关联的资源。 包装器将添加 **distributeForStudentWork** 属性并指示此资源将
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: a4f4e96c4b08eed4584d6357a8c903c080b2d16d
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52750369"
---
# <a name="educationassignmentresource-resource-type"></a>educationAssignmentResource 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

一个包装对象，用于存储与工作分配关联的资源。 包装器将 **添加 distributeForStudentWork** 属性，并指示此资源将复制到学生提交。  如果未复制对象，则每个学生将在作业中看到指向资源的链接。 学生将无法更新此资源。 这是教师向学生发的讲义，没有要打开的讲义。 如果分配了资源，则每个学生都将在提交的资源列表中收到此资源的副本。 每个学生将能够修改其副本并提交它进行评分。


## <a name="methods"></a>Methods

| 方法           | 返回类型    |Description|
|:---------------|:--------|:----------|
|[获取 educationAssignmentResource](../api/educationassignmentresource-get.md) | [educationAssignmentResource](educationassignmentresource.md) |读取 **educationAssignmentResource 对象的属性和** 关系。|
|[删除](../api/educationassignmentresource-delete.md) | 无 |删除 **educationAssignmentResource** 对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |Description|
|:---------------|:--------|:----------|
|distributeForStudentWork|Boolean|指示是否应该将此资源复制到每个学生提交以进行修改和提交。|
|id|String| 此资源的 ID。 只读。|
|resource|[educationResource](educationresource.md)|与此工作分配关联的 Resource 对象。|

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


