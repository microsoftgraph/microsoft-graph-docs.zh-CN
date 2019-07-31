---
title: educationAssignmentGrade 资源类型
description: " 但是, 所有类型的评分 (点、pass/fail 等) 都是此类的子类"
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 4de74fc9cbdf505bd57cfad3ab8dbf5a12e4e58a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006470"
---
# <a name="educationassignmentgrade-resource-type"></a>educationAssignmentGrade 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表提交中的**年级**对象。 这是一个永远不会实例化的抽象类型;但是, 所有类型的评分 (点、pass/fail 等) 都是此资源类型的子类。 此对象还跟踪正在进行评分的团队。 这在**提交. 年级**属性中使用。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|gradedBy|[identitySet](identityset.md)| 执行评分的用户。 |
|gradedDateTime|DateTimeOffset| 将评分应用于此提交对象的时间点。 时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|

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
