---
title: delegatedAdminRelationshipRequest 资源类型
description: 表示特定于合作伙伴与客户之间委派的管理员关系的请求。
author: adtangir
ms.localizationpriority: medium
ms.prod: customer-relationship-management
doc_type: resourcePageType
ms.openlocfilehash: 5aaaabed54e6f5a4f0ba21cbdf64fb7d9deb0e8f
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/01/2022
ms.locfileid: "65821181"
---
# <a name="delegatedadminrelationshiprequest-resource-type"></a>delegatedAdminRelationshipRequest 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示特定于合作伙伴与客户之间委派的管理员关系的请求。 它允许 Microsoft 合作伙伴管理员对关系执行操作，例如锁定关系以进行审批或终止关系。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[创建 delegatedAdminRelationshipRequest](../api/delegatedadminrelationship-post-requests.md)|[delegatedAdminRelationshipRequest](delegatedadminrelationshiprequest.md)|创建新的 **delegatedAdminRelationshipRequest** 对象。|
|[列出 delegatedAdminRelationshipRequests](../api/delegatedadminrelationship-list-requests.md)|[delegatedAdminRelationshipRequest](delegatedadminrelationshiprequest.md) 集合|获取 **delegatedAdminRelationshipRequest** 对象及其属性的列表。|
|[获取 delegatedAdminRelationshipRequest](../api/delegatedadminrelationshiprequest-get.md)|[delegatedAdminRelationshipRequest](delegatedadminrelationshiprequest.md)|读取 **delegatedAdminRelationshipRequest** 对象的属性和关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|action|delegatedAdminRelationshipRequestAction|要对委派的管理关系执行的操作。|
|createdDateTime|DateTimeOffset|以 ISO 8601 格式和 UTC 时间创建关系请求的日期和时间。 只读。 |
|id|String|关系请求的唯一标识符。 只读。 继承自 [entity](../resources/entity.md)。|
|lastModifiedDateTime|DateTimeOffset|ISO 8601 格式的日期和时间以及上次修改此关系请求时的 UTC 时间。 只读。|
|status|delegatedAdminRelationshipRequestStatus|请求的状态。 只读。 可能的值包括 `created`、`pending`、`succeeded`、`failed`、`unknownFutureValue`。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.delegatedAdminRelationshipRequest",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.delegatedAdminRelationshipRequest",
  "id": "String (identifier)",
  "action": "String",
  "status": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)"
}
```

