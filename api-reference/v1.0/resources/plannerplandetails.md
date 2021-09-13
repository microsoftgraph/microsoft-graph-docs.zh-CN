---
title: plannerPlanDetails 资源类型
description: '**plannerPlanDetails** 资源表示有关计划的其他信息。 每个计划对象都有一个 details 对象。'
ms.localizationpriority: medium
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 8631aa508c73a4921cc1e3d6a1805acbbc7defbf
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59129808"
---
# <a name="plannerplandetails-resource-type"></a>plannerPlanDetails 资源类型

命名空间：microsoft.graph


**plannerPlanDetails** 资源表示有关计划的其他信息。 每个 [计划](plannerplan.md) 对象都有一个 details 对象。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 plannerPlanDetails](../api/plannerplandetails-get.md) | [plannerPlanDetails](plannerplandetails.md) |读取 **plannerPlanDetails 对象的属性和** 关系。|
|[更新](../api/plannerplandetails-update.md) | [plannerPlanDetails](plannerplandetails.md)    |更新 **plannerPlanDetails** 对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|categoryDescriptions|[plannerCategoryDescriptions](plannercategorydescriptions.md)|指定可与计划中的任务相关联的六个类别的描述的对象|
|id|String| 只读。 计划详细信息的 ID。 长度为 28 个字符，区分大小写。 [格式验证](planner-identifiers-disclaimer.md)在服务上完成。|
|sharedWith|[plannerUserIds](planneruserids.md)|此计划共享的用户 ID 集。 如果你要利用Microsoft 365组，请使用组 API 管理组成员身份以[共享组计划](group.md)。 您还可以将组的现有成员添加到此集合中，尽管他们无需访问组所拥有的计划。 |

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

