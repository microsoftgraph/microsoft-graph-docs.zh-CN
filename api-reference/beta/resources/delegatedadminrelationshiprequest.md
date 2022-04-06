---
title: delegatedAdminRelationshipRequest 资源类型
description: 表示特定于合作伙伴和客户之间的委派管理员关系的请求。
author: adtangir
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 7381f4acf3ec04f4bdf4ef8f3a8bdf3744efa81d
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589594"
---
# <a name="delegatedadminrelationshiprequest-resource-type"></a>delegatedAdminRelationshipRequest 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示特定于合作伙伴和客户之间的委派管理员关系的请求。 它允许 Microsoft 合作伙伴管理员对关系采取操作，例如锁定关系进行审批或终止关系。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[创建 delegatedAdminRelationshipRequest](../api/delegatedadminrelationship-post-requests.md)|[delegatedAdminRelationshipRequest](delegatedadminrelationshiprequest.md)|创建新的 **delegatedAdminRelationshipRequest** 对象。|
|[列出 delegatedAdminRelationshipRequests](../api/delegatedadminrelationship-list-requests.md)|[delegatedAdminRelationshipRequest](delegatedadminrelationshiprequest.md) 集合|获取 **delegatedAdminRelationshipRequest** 对象及其属性的列表。|
|[获取 delegatedAdminRelationshipRequest](../api/delegatedadminrelationshiprequest-get.md)|[delegatedAdminRelationshipRequest](delegatedadminrelationshiprequest.md)|读取 **delegatedAdminRelationshipRequest** 对象的属性和关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|action|delegatedAdminRelationshipRequestAction|对委派管理员关系执行的操作。|
|createdDateTime|DateTimeOffset|创建关系请求时采用 ISO 8601 格式的日期和时间，采用 UTC 时间。 只读。 |
|id|String|关系请求的唯一标识符。 只读。 继承自 [entity](../resources/entity.md)。|
|lastModifiedDateTime|DateTimeOffset|ISO 8601 格式的日期和时间以及上次修改此关系请求的 UTC 时间。 只读。|
|状态|delegatedAdminRelationshipRequestStatus|请求的状态。 只读。 可能的值包括 `created`、`pending`、`complete`、`failed`、`unknownFutureValue`。|

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

