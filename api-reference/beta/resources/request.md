---
title: 请求资源类型
description: 一个抽象实体类型，用于为要创建、更新和删除对象的异步请求工作流建模。
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 6e75c2d632356fceffaf432fc4def204e837c9bc
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2022
ms.locfileid: "65399395"
---
# <a name="request-resource-type"></a>请求资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

一个抽象实体类型，用于为要创建、更新和删除对象的异步请求工作流建模。

继承自 [entity](entity.md)。


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|approvalId|String|请求批准的标识符。|
|completedDateTime|DateTimeOffset|请求完成日期时间。|
|createdBy|[identitySet](identityset.md)|创建此请求的用户。|
|createdDateTime|DateTimeOffset|请求创建日期时间。|
|customData|String|用于定义请求的任何自定义数据的免费文本字段。 未使用。|
|status|String|请求的状态。 不可为 null。 可能的值为：`Canceled`、、`Denied`、`Failed`、`Granted`、`PendingApproval``PendingAdminDecision`、`PendingProvisioning``Revoked``PendingScheduleCreation``Provisioned`、和 。`ScheduleCreated` 不可为空。|
|id|String|请求的标识符。 只读。 不可为 null。 继承自 [entity](entity.md)。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|“审批”|“[审批](../resources/approval.md)”|表示请求链接到的审批对象。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.request",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.request",
  "id": "String (identifier)",
  "approvalId": "String (identifier)",
  "completedDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "customData": "String",
  "status": "String",
}
```

