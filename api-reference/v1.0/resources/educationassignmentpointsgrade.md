---
title: educationAssignmentPointsGrade 资源类型
description: 当分配设置为分数等级类型时，每个提交都将具有与 **submission.grade** 属性关联的此对象。
ms.localizationpriority: medium
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 8019915e246a1b219357887ead1ee9ec8e7627d6
ms.sourcegitcommit: c21fefa5c3c62df14147e7918cb43327f7d72e69
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/06/2022
ms.locfileid: "64684667"
---
# <a name="educationassignmentpointsgrade-resource-type"></a>educationAssignmentPointsGrade 资源类型

命名空间：microsoft.graph

当分配设置为分数等级类型时，每个提交都将具有与 **submission.grade** 属性关联的此对象。 这会从 [educationAssignmentGrade](educationassignmentgrade.md) 创建一个子类，该子类会将谁的数据添加到此属性。 最大点存储在 **assignments.grading 属性中** 。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|points|单精度|教师给此提交对象的分数数。|
|gradedBy|[identitySet](identityset.md)| 执行评分的用户。 |
|gradedDateTime|DateTimeOffset| 将成绩应用于此提交对象的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentPointsGrade"
}-->

```json
{
  "points": "Double",
  "gradedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "gradedDateTime": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentPointsGrade resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


