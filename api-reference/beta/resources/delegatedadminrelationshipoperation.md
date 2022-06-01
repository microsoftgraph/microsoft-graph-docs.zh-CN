---
title: delegatedAdminRelationshipOperation 资源类型
description: 表示与委派的管理员关系相关的长时间运行的操作。
author: adtangir
ms.localizationpriority: medium
ms.prod: customer-relationship-management
doc_type: resourcePageType
ms.openlocfilehash: bf369451c3a2b0d5ab4ca01894a4c7d546f7e630
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/01/2022
ms.locfileid: "65820936"
---
# <a name="delegatedadminrelationshipoperation-resource-type"></a>delegatedAdminRelationshipOperation 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示与委派的管理员关系相关的长时间运行的操作。 长时间运行操作的示例可以是对 [delegatedAdminAccessAssignment 对象的](delegatedAdminAccessAssignment.md) 更新。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 delegatedAdminRelationshipOperations](../api/delegatedadminrelationship-list-operations.md)|[delegatedAdminRelationshipOperation](delegatedadminrelationshipoperation.md) 集合|获取 **delegatedAdminRelationshipOperation** 对象及其属性的列表。|
|[获取 delegatedAdminRelationshipOperation](../api/delegatedadminrelationshipoperation-get.md)|[delegatedAdminRelationshipOperation](delegatedadminrelationshipoperation.md)|读取 **delegatedAdminRelationshipOperation** 对象的属性和关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|以 ISO 8601 格式和 UTC 时间创建长时间运行的操作的时间。 只读。|
|data|String|该操作的数据 (有效负载) 。 只读。|
|id|String|委托管理员长时间运行操作的唯一标识符。 只读。 继承自 [entity](../resources/entity.md)。|
|lastModifiedDateTime|DateTimeOffset|上次修改长时间运行的操作的时间（以 ISO 8601 格式和 UTC 时间）。 只读。|
|operationType|delegatedAdminRelationshipOperationType|长时间运行的操作的类型。 可能的值为： `delegatedAdminAccessAssignmentUpdate`. `unknownFutureValue` 只读。|
|status|longRunningOperationStatus|操作的状态。 只读。 可能的值包括 `notStarted`、`running`、`succeeded`、`failed`、`unknownFutureValue`。 只读。 支持 `$orderBy`。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.delegatedAdminRelationshipOperation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.delegatedAdminRelationshipOperation",
  "id": "String (identifier)",
  "operationType": "String",
  "data": "String",
  "status": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)"
}
```
