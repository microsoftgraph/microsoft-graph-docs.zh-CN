---
title: educationRubric 资源类型
description: 可附加到工作分配的评分标准
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 37e1d4a6267f1f1292a72cc7f34b8135483091ec
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161934"
---
# <a name="educationrubric-resource-type"></a>educationRubric 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

可附加到工作分配的评分标准。 一个分值与一个 **educationUser** (教师) ，并附加到一个或多个 **educationAssignment** 资源。 

有关详细信息 [，请参阅教育程度](/graph/education-rubric-overview) 概述。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [创建 educationRubric](../api/educationuser-post-rubrics.md) | [educationRubric](educationrubric.md) | 创建新的 educationRubric 对象。 |
| [获取 educationRubric](../api/educationrubric-get.md) | [educationRubric](educationrubric.md) | 读取 educationRubric 对象的属性和关系。 |
| [更新 educationRubric](../api/educationrubric-update.md) | [educationRubric](educationrubric.md) | 更新 educationRubric 对象。 |
| [删除 educationRubric](../api/educationrubric-delete.md) | 无 | 删除 educationRubric 对象。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|createdBy|[identitySet](identityset.md)|创建此资源的用户。|
|createdDateTime|DateTimeOffset|时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`|
|说明|[itemBody](itembody.md)|此分卡的说明。|
|displayName|String|此度数的名称。|
|分|[educationAssignmentGradeType](educationassignmentgradetype.md)|此评分标准评分类型 - 无点评分标准为 [null，educationAssignmentPointsGradeType](educationassignmentpointsgradetype.md) 为评分标准。|
|lastModifiedBy|[identitySet](identityset.md)|最后一个修改资源的用户。|
|lastModifiedDateTime|DateTimeOffset|上次修改资源的时间。  时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|levels|[rubricLevel](rubriclevel.md) 集合|此标准所包括的级别的集合。|
|质量|[rubricQuality](rubricquality.md) 集合|这个质量集合是这个质量的一部分。|

## <a name="relationships"></a>关系

无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationRubric",
  "keyProperty": "id"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "description": {"@odata.type": "microsoft.graph.itemBody"},
  "displayName": "String",
  "grading": {"@odata.type": "microsoft.graph.educationAssignmentGradeType"},
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "levels": [{"@odata.type": "microsoft.graph.rubricLevel"}],
  "qualities": [{"@odata.type": "microsoft.graph.rubricQuality"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationRubric resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->