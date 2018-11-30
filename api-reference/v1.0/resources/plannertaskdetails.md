---
title: plannerTaskDetails 资源类型
description: '**plannerTaskDetails** 资源表示任务的其他相关信息。每个任务对象均有一个详细信息对象。'
ms.openlocfilehash: 74ba1c5b7c607f30253463e6cfc256fd3119bf45
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011430"
---
# <a name="plannertaskdetails-resource-type"></a>plannerTaskDetails 资源类型

**plannerTaskDetails** 资源表示任务的其他相关信息。每个[任务](plannertask.md)对象均有一个详细信息对象。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[Get plannerTaskDetails](../api/plannertaskdetails-get.md) | [plannerTaskDetails](plannertaskdetails.md) |读取 **plannerTaskDetails** 对象的属性和关系。|
|[Update](../api/plannertaskdetails-update.md) | [plannerTaskDetails](plannertaskdetails.md)    |更新 **plannerTaskDetails** 对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|checklist|[plannerChecklistItems](plannerchecklistitems.md)|任务上的检查表项目集合。|
|说明|String|任务描述|
|id|String| 只读。 任务详细信息的 ID。 它是 28 字符长度和区分大小写。 服务上执行[格式验证](planner-identifiers-disclaimer.md)。|
|previewType|string|这将设置显示任务的预览的类型。 可能的值为： `automatic`， `noPreview`， `checklist`， `description`， `reference`。 当设置为`automatic`显示的预览选择应用程序查看任务。|
|references|[plannerExternalReferences](plannerexternalreferences.md)|任务上的引用集合。|

## <a name="relationships"></a>关系
无


## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerTaskDetails"
}-->

```json
{
  "checklist": {"@odata.type": "microsoft.graph.plannerChecklistItems"},
  "description": "String",
  "id": "String (identifier)",
  "previewType": "string",
  "references": {"@odata.type": "microsoft.graph.plannerExternalReferences"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerTaskDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
