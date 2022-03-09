---
title: approvalStage 资源类型
description: 与 userConsentRequest 或访问包分配请求关联的 approvalStage 对象。
author: psignoret
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 2cd51e18cd3d641018c5f0792754cec129392aa6
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63395851"
---
# <a name="approvalstage-resource-type"></a>approvalStage 资源类型

命名空间：microsoft.graph

指定审批中的决策 [阶段](approval.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 approvalStages](../api/approval-list-stages.md) | [approvalStage](approvalstage.md) 集合 | 列出与权利管理 **中的审批对象** 关联的 **approvalStage** 对象。 |
|[获取 approvalStage](../api/approvalstage-get.md) | [approvalStage](approvalstage.md) | 在权利管理中检索 **approvalStage** 对象的属性。 |
|[更新 approvalStage](../api/approvalstage-update.md) | None | 在权利管理中对 **approvalStage** 对象应用批准或拒绝决定。 |

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|assignedToMe|布尔值|指示是否将阶段分配给呼叫用户进行审阅。 只读。|
|displayName|String|策略创建者提供用于标识审批阶段的标签。 只读。|
|id|String|与审批对象关联的阶段的标识符。 只读。|
|justification|字符串|与审批阶段决策相关的理由。|
|reviewResult|String|此审批记录的结果。 可能的值包括：、`NotReviewed`、`Denied``Approved`。|
|reviewedBy|[identity](identity.md) | 审阅者的标识符。 只读。|
|reviewedDateTime|DateTimeOffset|记录决策的日期和时间。 日期和时间信息采用 ISO 8601 格式，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。|
|状态|String|阶段状态。 可能的值：、`InProgress`、`Completed``Initializing`、`Expired`。 只读。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.approvalStage",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.approvalStage",
  "id": "String (identifier)",
  "displayName": "String",
  "status": "String",
  "assignedToMe": "Boolean",
  "reviewedBy": {
    "@odata.type": "microsoft.graph.identity"
  },
  "reviewedDateTime": "String (timestamp)",
  "reviewResult": "String",
  "justification": "String"
}
```
