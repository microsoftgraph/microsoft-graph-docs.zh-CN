---
title: educationAssignmentPointsGrade 资源类型
description: 当工作分配设置为磅薪等级类型时，每个提交将具有此对象与**submission.grade**属性关联。 这将从 educationAssignmentGrade，创建一个子类
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: d96b84380bc7a6d2298117b5dfeaee25d943efb2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982384"
---
# <a name="educationassignmentpointsgrade-resource-type"></a>educationAssignmentPointsGrade 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

当工作分配设置为磅薪等级类型时，每个提交将具有此对象与**submission.grade**属性关联。 这将创建一个子类从[educationAssignmentGrade](educationassignmentgrade.md)，其中将 who 将数据添加到此属性。 **Assignments.grading**属性中存储的最大点。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|points|Single|教师的磅数提供此提交对象。|

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
  "points": "Single"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationAssignmentPointsGrade resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
