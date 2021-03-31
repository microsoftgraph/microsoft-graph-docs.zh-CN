---
title: approvalStage 资源类型
description: 与 userConsentRequest 关联的 approvalStage 对象。
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d6212553d9364c4352bf1d6796156a4020854bf1
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469527"
---
# <a name="approvalstage-resource-type"></a>approvalStage 资源类型

命名空间：microsoft.graph

指定审批中的决策阶段。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|assignedToMe|Boolean|指示是否将阶段分配给呼叫用户进行审阅。 只读。|
|displayName|String|策略创建者提供用于标识审批阶段的标签。 只读。|
|id|String|与审批对象关联的阶段的标识符。 只读。|
|justification|String|与审批阶段决策相关的理由。|
|reviewResult|String|此审批记录的结果。 可能的值包括 `NotReviewed` `Approved` `Denied` ：、、。|
|reviewedBy|[userIdentity](useridentity.md) | 审阅者的标识符。 只读。|
|reviewedDateTime|DateTimeOffset|记录决策的日期和时间。 日期和时间信息采用 ISO 8601 格式，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。|
|状态|String|阶段状态。 可能的值 `InProgress` `Initializing` `Completed` ：、、、。 `Expired` 只读。|

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
