---
title: delegatedAdminRelationship 资源类型
description: 表示 Microsoft 合作伙伴在客户租户中具有的委派管理权限的详细信息。
author: adtangir
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: f0bb9038773c965e54ce0695ff443b931df02cfd
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589596"
---
# <a name="delegatedadminrelationship-resource-type"></a>delegatedAdminRelationship 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示合作伙伴和客户之间的委派管理员关系。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[创建 delegatedAdminRelationship](../api/tenantrelationship-post-delegatedadminrelationships.md)|[delegatedAdminRelationship](delegatedadminrelationship.md)|创建新的 **delegatedAdminRelationship** 对象。|
|[列出 delegatedAdminRelationships](../api/tenantrelationship-list-delegatedadminrelationships.md)|[delegatedAdminRelationship](delegatedadminrelationship.md) 集合|获取 **delegatedAdminRelationship** 对象及其属性的列表。|
|[获取 delegatedAdminRelationship](../api/delegatedadminrelationship-get.md)|[delegatedAdminRelationship](delegatedadminrelationship.md)|读取 **delegatedAdminRelationship 对象的属性和** 关系。|
|[更新 delegatedAdminRelationship](../api/delegatedadminrelationship-update.md)|[delegatedAdminRelationship](delegatedadminrelationship.md)|更新 **delegatedAdminRelationship 对象** 的属性。|
|[删除 delegatedAdminRelationship](../api/delegatedadminrelationship-delete.md)|无|删除 **delegatedAdminRelationship** 对象。|


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|accessDetails|[delegatedAdminAccessDetails](../resources/delegatedadminaccessdetails.md)|包含合作伙伴管理员在客户租户中请求的管理角色标识符的访问详细信息。|
|activatedDateTime|DateTimeOffset|关系处于活动状态时采用 ISO 8601 格式的日期和时间，采用 UTC 时间。 只读。|
|createdDateTime|DateTimeOffset|创建关系时采用 ISO 8601 格式和 UTC 时间表示的日期和时间。 只读。|
|customer|[delegatedAdminRelationshipCustomerParticipant](../resources/delegatedadminrelationshipcustomerparticipant.md)|关系显示名称的客户的标识符和唯一标识符。 这由合作伙伴在建立关系时配置，或在客户批准关系后由系统配置。 客户无法更改。|
|displayName|String|用于显示名称识别的关系的标识。 在 *合作伙伴的所有委派* 管理员关系中必须是唯一的。 这仅在关系状态为 `created` 且客户无法更改时由合作伙伴设置。|
|duration|期限|关系采用 ISO 8601 格式的持续时间。 必须是介于 和 （包含 `P1D` 两者） `P2Y` 之间的值。 这仅在关系状态为 `created` 且客户无法更改时由合作伙伴设置。|
|endDateTime|DateTimeOffset|关系状态更改为 或 时采用 ISO 8601 格式的日期和时间，采用 UTC  `terminated` 时间。`expired` 计算公式为 `endDateTime = activatedDateTime + duration`。 只读。|
|id|String|关系的唯一标识符。 只读。 继承自 [entity](../resources/entity.md)。|
|lastModifiedDateTime|DateTimeOffset|ISO 8601 格式的日期和时间以及上次修改关系的 UTC 时间。 只读。|
|状态|delegatedAdminRelationshipStatus|关系的状态。 只读。 可能的值包括：、`activating``approvalPending``active`、`approved`、`created`、、`expired`、、`expiring``terminationRequested``terminated``terminating``unknownFutureValue`、。 支持 `$orderBy`。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|accessAssignments|[delegatedAdminAccessAssignment](../resources/delegatedadminaccessassignment.md) 集合|与委派管理员关系关联的访问分配。|
|operations|[delegatedAdminRelationshipOperation](../resources/delegatedadminrelationshipoperation.md) 集合|与委派管理员关系相关联的长时间运行的操作。|
|requests|[delegatedAdminRelationshipRequest](../resources/delegatedadminrelationshiprequest.md) 集合|与委派管理员关系关联的请求。|

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

