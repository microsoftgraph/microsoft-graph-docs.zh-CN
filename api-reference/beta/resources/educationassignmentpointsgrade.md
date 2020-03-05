---
title: educationAssignmentPointsGrade 资源类型
description: 当工作分配设置为 "点" 评分类型时，每个提交都将具有与 "**提交. 年级**" 属性相关联的此对象。 这将从 educationAssignmentGrade 中创建一个子类，
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: c2ef014c3e9e2954dba5fb759fcf3f86b3681b68
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42502506"
---
# <a name="educationassignmentpointsgrade-resource-type"></a>educationAssignmentPointsGrade 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

当工作分配设置为 "点" 评分类型时，每个提交都将具有与 "**提交. 年级**" 属性相关联的此对象。 这将从[educationAssignmentGrade](educationassignmentgrade.md)创建一个子类，该子类将向此属性添加数据。 最大分数存储在**工作分配. 评分**属性中。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|points|单精度|教师向此提交对象提供的积分数。|

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
  "points": "Double"
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
