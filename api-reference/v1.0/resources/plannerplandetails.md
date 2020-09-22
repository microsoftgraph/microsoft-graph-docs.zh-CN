---
title: plannerPlanDetails 资源类型
description: '**PlannerPlanDetails**资源表示有关计划的其他信息。 每个 plan 对象都有一个详细信息对象。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 727da0983ddcaffb158be14a578a5a81eacecab3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037386"
---
# <a name="plannerplandetails-resource-type"></a>plannerPlanDetails 资源类型

命名空间：microsoft.graph


**PlannerPlanDetails**资源表示有关计划的其他信息。 每个 [plan](plannerplan.md) 对象都有一个详细信息对象。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 plannerPlanDetails](../api/plannerplandetails-get.md) | [plannerPlanDetails](plannerplandetails.md) |读取 **plannerPlanDetails** 对象的属性和关系。|
|[更新](../api/plannerplandetails-update.md) | [plannerPlanDetails](plannerplandetails.md)    |更新 **plannerPlanDetails** 对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|categoryDescriptions|[plannerCategoryDescriptions](plannercategorydescriptions.md)|指定可与计划中的任务相关联的六个类别的描述的对象|
|id|String| 只读。 计划详细信息的 ID。 长度为 28 个字符，区分大小写。 [格式验证](planner-identifiers-disclaimer.md)在服务上完成。|
|sharedWith|[plannerUserIds](planneruserids.md)|与之共享此计划的用户 id 集。 如果您利用的是 Microsoft 365 组，请使用组 API 来管理组成员身份，以共享 [组的](group.md) 计划。 您还可以将组的现有成员添加到此集合中，但它们不需要他们访问该组拥有的计划。 |

## <a name="relationships"></a>关系
无


## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerPlanDetails"
}-->

```json
{
  "categoryDescriptions": {"@odata.type": "microsoft.graph.plannerCategoryDescriptions"},
  "id": "String (identifier)",
  "sharedWith": {"@odata.type": "microsoft.graph.plannerUserIds"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlanDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

