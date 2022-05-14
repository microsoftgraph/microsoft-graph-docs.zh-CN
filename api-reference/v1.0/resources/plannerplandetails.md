---
title: plannerPlanDetails 资源类型
description: '**plannerPlanDetails** 资源表示有关计划的附加信息。 每个 plan 对象都有一个详细信息对象。'
ms.localizationpriority: medium
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 41daa24c42805b76702a9ed77942c9ce1edbcbf7
ms.sourcegitcommit: ca1b33aaecb320b33423aeec7438ce306bffab14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/14/2022
ms.locfileid: "65420549"
---
# <a name="plannerplandetails-resource-type"></a>plannerPlanDetails 资源类型

命名空间：microsoft.graph


**plannerPlanDetails** 资源表示有关计划的附加信息。 每个 [plan](plannerplan.md) 对象都有一个详细信息对象。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 plannerPlanDetails](../api/plannerplandetails-get.md) | [plannerPlanDetails](plannerplandetails.md) |读取 **plannerPlanDetails** 对象的属性和关系。|
|[更新](../api/plannerplandetails-update.md) | [plannerPlanDetails](plannerplandetails.md)    |更新 **plannerPlanDetails** 对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|categoryDescriptions|[plannerCategoryDescriptions](plannercategorydescriptions.md)|一个对象，指定可与计划中的任务关联的 25 个类别的说明。|
|id|String| 只读。 计划详细信息的 ID。 长度为 28 个字符，区分大小写。 [格式验证](planner-identifiers-disclaimer.md)在服务上完成。|
|sharedWith|[plannerUserIds](planneruserids.md)|与此计划共享的用户 ID 集。 如果要利用Microsoft 365组，请使用组 API 管理组成员身份以共享[组](group.md)的计划。 你还可以将组的现有成员添加到此集合中，尽管它们不需要访问组拥有的计划。 |

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

