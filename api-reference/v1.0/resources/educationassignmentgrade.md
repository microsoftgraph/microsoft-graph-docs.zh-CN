---
title: educationAssignmentGrade 资源类型
description: 表示提交上的 Grade 对象。
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: a165203242f13805cab7dbf159519deaf42e9cb146358a4406362ae2a8ba9507
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54230758"
---
# <a name="educationassignmentgrade-resource-type"></a>educationAssignmentGrade 资源类型

命名空间：microsoft.graph

表示 **提交上的 Grade** 对象。 

这是永远不会实例化抽象类型;但是，所有评分类型 (点、通过/失败等) 是此资源类型的子类。 此对象还跟踪进行评分的人。 this is used in the **submission.grade** property.


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|gradedBy|[identitySet](identityset.md)| 评分的用户。 |
|gradedDateTime|DateTimeOffset| 此提交对象应用成绩的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentGrade"
}-->

```json
{
  "gradedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "gradedDateTime": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentGrade resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


