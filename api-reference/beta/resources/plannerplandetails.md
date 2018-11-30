---
title: plannerPlanDetails 资源类型
description: '**plannerPlanDetails** 资源表示计划的其他相关信息。每个计划对象均有一个详细信息对象。'
ms.openlocfilehash: 1cce5727666bca705da67fccd1a3edf370c68127
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048088"
---
# <a name="plannerplandetails-resource-type"></a>plannerPlanDetails 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

**plannerPlanDetails** 资源表示计划的其他相关信息。每个[计划](plannerplan.md)对象均有一个详细信息对象。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[Get plannerPlanDetails](../api/plannerplandetails-get.md) | [plannerPlanDetails](plannerplandetails.md) |读取的属性和**plannerPlanDetails**对象的关系。|
|[Update](../api/plannerplandetails-update.md) | [plannerPlanDetails](plannerplandetails.md)    |更新**plannerPlanDetails**对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|categoryDescriptions|[plannerCategoryDescriptions](plannercategorydescriptions.md)|指定可与计划中的任务相关联的六个类别的描述的对象|
|id|String| 只读。 计划详细信息的 ID。 它是 28 字符长度和区分大小写。 服务上执行[格式验证](tasks-identifiers-disclaimer.md)。|
|sharedWith|[plannerUserIds](planneruserids.md)|用户与共享此计划的 Id 集。 如果您使用的 Office 365 组，可以使用组 API 管理组成员身份共享的[组的](group.md)计划。 尽管不作要求以便访问计划组拥有的顺序，还可以向此集合中，添加现有组的成员。 |
|contextDetails|[plannerPlanContextDetailsCollection](plannerplancontextdetailscollection.md)|只读。 定义对[plannerPlan](plannerplan.md)容器的[plannerPlanContext](plannerplancontext.md)条目关联的其他信息的集合。 |

## <a name="relationships"></a>Relationships
无。


## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanDetails"
}-->

```json
{
  "categoryDescriptions": {"@odata.type": "microsoft.graph.plannerCategoryDescriptions"},
  "contextDetails": {"@odata.type": "microsoft.graph.plannerPlanContextDetailsCollection"},
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
