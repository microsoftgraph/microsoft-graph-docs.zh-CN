---
title: operationApprovalRequestEntityStatus 资源类型
description: OperationApprovalRequestEntityStatus 对象
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cef153334cdd30044a75ed1cc0e322f6e94ecb64
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/19/2021
ms.locfileid: "60487887"
---
# <a name="operationapprovalrequestentitystatus-resource-type"></a>operationApprovalRequestEntityStatus 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

OperationApprovalRequestEntityStatus 对象

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|requestId|String|此实体的 OperationApprovalRequest 的 ID。 此属性是只读的。|
|requestExpirationDateTime|DateTimeOffset|不再允许对请求执行操作的日期/时间。 此属性是只读的。|
|requestStatus|[operationApprovalRequestStatus](../resources/intune-rbac-operationapprovalrequeststatus.md)|当前审批请求状态。 此属性是只读的。 可取值为：`unknown`、`needsApproval`、`approved`、`rejected`、`cancelled`、`completed` 或 `expired`。|
|entityLocked|Boolean|实体在更改方面的状态，是允许进一步的请求还是锁定实体。 此属性是只读的。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.operationApprovalRequestEntityStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.operationApprovalRequestEntityStatus",
  "requestId": "String",
  "requestExpirationDateTime": "String (timestamp)",
  "requestStatus": "String",
  "entityLocked": true
}
```



