---
title: 请求资源类型
description: 表示 PIM 或 userConsentRequests 中请求的详细信息。
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 72a52ce4911dc85a5d4f954cdc48e62ad8f1f9c2
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65897951"
---
# <a name="request-resource-type"></a>请求资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 [PIM](privilegedidentitymanagementv3-overview.md) 或 [用户同意请求](userconsentrequest.md) API 中请求的详细信息。

继承自 [entity](../resources/entity.md)。


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|approvalId|字符串| 请求批准的标识符。  |
|completedDateTime|DateTimeOffset| 请求完成日期时间。 |
|createdBy|[identitySet](../resources/identityset.md)|创建请求的主体。|
|createdDateTime|DateTimeOffset|请求创建日期时间。|
|customData|字符串|用于定义请求的任何自定义数据的免费文本字段。 未使用。|
|id|字符串|请求对象的唯一标识符。 继承自 [entity](../resources/entity.md)。|
|status|字符串| 请求的状态。 不可为 null。 可能的值为：`Canceled`、、`Denied`、`Failed`、`Granted`、`PendingApproval``PendingAdminDecision`、`PendingProvisioning``Revoked``PendingScheduleCreation``Provisioned`、和 。`ScheduleCreated` 不可为空。 |

## <a name="relationships"></a>关系
无。

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
  "status": "String",
  "completedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "approvalId": "String",
  "customData": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```