---
title: delegatedAdminRelationship 资源类型
description: 表示 Microsoft 合作伙伴在客户租户中拥有的委派管理权限的详细信息。
author: adtangir
ms.localizationpriority: medium
ms.prod: customer-relationship-management
doc_type: resourcePageType
ms.openlocfilehash: 430c1acb78d05681cd88d76fbeb5ba0e43aeef53
ms.sourcegitcommit: 5a43129dbf705f2d1a6afcff36af9f41ecee026d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2022
ms.locfileid: "64704429"
---
# <a name="delegatedadminrelationship-resource-type"></a>delegatedAdminRelationship 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示合作伙伴和客户之间的委派管理员关系。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[创建 delegatedAdminRelationship](../api/tenantrelationship-post-delegatedadminrelationships.md)|[delegatedAdminRelationship](delegatedadminrelationship.md)|创建新的 **delegatedAdminRelationship** 对象。|
|[列出 delegatedAdminRelationships](../api/tenantrelationship-list-delegatedadminrelationships.md)|[delegatedAdminRelationship](delegatedadminrelationship.md) 集合|获取 **delegatedAdminRelationship** 对象及其属性的列表。|
|[获取 delegatedAdminRelationship](../api/delegatedadminrelationship-get.md)|[delegatedAdminRelationship](delegatedadminrelationship.md)|读取 **delegatedAdminRelationship** 对象的属性和关系。|
|[更新 delegatedAdminRelationship](../api/delegatedadminrelationship-update.md)|[delegatedAdminRelationship](delegatedadminrelationship.md)|更新 **delegatedAdminRelationship 对象的** 属性。|
|[删除 delegatedAdminRelationship](../api/delegatedadminrelationship-delete.md)|无|删除 **delegatedAdminRelationship** 对象。|


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|accessDetails|[delegatedAdminAccessDetails](../resources/delegatedadminaccessdetails.md)|访问详细信息，其中包含合作伙伴管理员在客户租户中请求的管理角色的标识符。|
|activatedDateTime|DateTimeOffset|ISO 8601 格式的日期和时间，以及关系处于活动状态时的 UTC 时间。 只读。|
|createdDateTime|DateTimeOffset|以 ISO 8601 格式和 UTC 时间创建关系的日期和时间。 只读。|
|客户|[delegatedAdminRelationshipCustomerParticipant](../resources/delegatedadminrelationshipcustomerparticipant.md)|关系客户的显示名称和唯一标识符。 这是由创建关系时的合作伙伴配置的，或者由系统在客户批准关系后配置的。 客户无法更改。|
|displayName|String|用于简化标识的关系的显示名称。 在合作伙伴 *的所有* 委派管理员关系中必须是唯一的。 仅当关系 `created` 处于状态且客户无法更改时，合作伙伴才会设置此设置。|
|duration|期限|以 ISO 8601 格式的关系持续时间。 必须是介于和`P2Y`非独占之间的`P1D`值。 仅当关系 `created` 处于状态且客户无法更改时，合作伙伴才会设置此设置。|
|endDateTime|DateTimeOffset|ISO 8601 格式的日期和时间，以及关系 **状态** 更改为或 `terminated` 更改为 UTC 时间的日期和 `expired`时间。 计算为 `endDateTime = activatedDateTime + duration`. 只读。|
|id|字符串|关系的唯一标识符。 只读。 继承自 [entity](../resources/entity.md)。|
|lastModifiedDateTime|DateTimeOffset|ISO 8601 格式的日期和时间，以及上次修改关系时的 UTC 时间。 只读。|
|状态|delegatedAdminRelationshipStatus|关系的状态。 只读。 可能的值是：`activating`、、`active`、`approvalPending`、`approved`、`expired``created`、`expiring`、`terminated``terminating`、`terminationRequested`。 `unknownFutureValue` 支持 `$orderBy`。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|accessAssignments|[delegatedAdminAccessAssignment](../resources/delegatedadminaccessassignment.md) 集合|与委派的管理员关系关联的访问分配。|
|operations|[delegatedAdminRelationshipOperation](../resources/delegatedadminrelationshipoperation.md) 集合|与委派的管理关系关联的长时间运行的操作。|
|请求|[delegatedAdminRelationshipRequest](../resources/delegatedadminrelationshiprequest.md) 集合|与委派的管理关系关联的请求。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.delegatedAdminRelationship",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.delegatedAdminRelationship",
  "id": "String (identifier)",
  "displayName": "String",
  "duration": "String",
  "customer": {
    "@odata.type": "microsoft.graph.delegatedAdminRelationshipCustomerParticipant"
  },
  "accessDetails": {
    "@odata.type": "microsoft.graph.delegatedAdminAccessDetails"
  },
  "status": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "activatedDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)"
}
```

