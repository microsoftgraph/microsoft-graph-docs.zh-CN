---
title: educationRubric 资源类型
description: 可附加到工作分配的评分标准。
ms.localizationpriority: medium
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: bf5565aa6862b66f59f5b75a4c9b8ae177049d34
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59126833"
---
# <a name="educationrubric-resource-type"></a>educationRubric 资源类型

命名空间：microsoft.graph

可附加到工作分配的评分标准。 一个分卡与 **educationUser** (教师) ，并附加到一个或多个 **education分配** 资源。 

有关详细信息 [，请参阅教育](/graph/education-rubric-overview) 程度概述。

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
|createdDateTime|DateTimeOffset|时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`2014-01-01T00:00:00Z`|
|说明|[itemBody](itembody.md)|此分卡的说明。|
|displayName|String|此分号的名称。|
|一个|[educationAssignmentGradeType](educationassignmentgradetype.md)|此评分标准评分类型 -- 无评分标准为 [null，educationAssignmentPointsGradeType](educationassignmentpointsgradetype.md) 为评分标准。|
|lastModifiedBy|[identitySet](identityset.md)|最后一个修改资源的用户。|
|lastModifiedDateTime|DateTimeOffset|上次修改资源的时间。  时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|levels|[rubricLevel](rubriclevel.md) 集合|此标准中的级别集合。|
|一些|[rubricQuality](rubricquality.md) 集合|此分项由质量集合决定。|

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
