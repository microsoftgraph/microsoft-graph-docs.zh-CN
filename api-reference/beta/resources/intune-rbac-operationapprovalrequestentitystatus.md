---
title: operationApprovalRequestEntityStatus 资源类型
description: OperationApprovalRequestEntityStatus 对象
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ffc877ddf0a724b1471c55e2b9edb0455e4da0fb
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209126"
---
# <a name="operationapprovalrequestentitystatus-resource-type"></a>operationApprovalRequestEntityStatus 资源类型

命名空间：microsoft.graph

> **重要：**/beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

OperationApprovalRequestEntityStatus 对象

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|requestId|String|此实体的 OperationApprovalRequest 的 ID。 此属性是只读的。|
|requestExpirationDateTime|DateTimeOffset|不再允许对请求执行操作的 DateTime。 此属性是只读的。|
|requestStatus|[operationApprovalRequestStatus](../resources/intune-rbac-operationapprovalrequeststatus.md)|当前审批请求状态。 此属性是只读的。 可取值为：`unknown`、`needsApproval`、`approved`、`rejected`、`cancelled`、`completed`、`expired`、`unknownFutureValue`。|
|entityLocked|Boolean|实体在更改方面的状态，无论是允许进一步请求还是锁定实体。 此属性是只读的。|

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




