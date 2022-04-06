---
title: delegatedAdminRelationshipOperation 资源类型
description: 表示与委派管理员关系相关的长时间运行的操作。
author: adtangir
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 50aaad489ba955c4d7ba2a9c0992e63b445732b5
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589595"
---
# <a name="delegatedadminrelationshipoperation-resource-type"></a>delegatedAdminRelationshipOperation 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示与委派管理员关系相关的长时间运行的操作。 长时间运行的操作的示例可以是 [delegatedAdminAccessAssignment 对象的](delegatedAdminAccessAssignment.md) 更新。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 delegatedAdminRelationshipOperations](../api/delegatedadminrelationship-list-operations.md)|[delegatedAdminRelationshipOperation](delegatedadminrelationshipoperation.md) 集合|获取 **delegatedAdminRelationshipOperation 对象** 及其属性的列表。|
|[获取 delegatedAdminRelationshipOperation](../api/delegatedadminrelationshipoperation-get.md)|[delegatedAdminRelationshipOperation](delegatedadminrelationshipoperation.md)|读取 **delegatedAdminRelationshipOperation 对象的属性和** 关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|创建长时间运行的操作时采用 ISO 8601 格式和 UTC 时间的时间。 只读。|
|data|String|数据 (操作) 有效负载。 只读。|
|id|String|委派管理员长时间运行操作的唯一标识符。 只读。 继承自 [entity](../resources/entity.md)。|
|lastModifiedDateTime|DateTimeOffset|以 ISO 8601 格式和 UTC 时间表示的上次修改长时间运行操作的时间。 只读。|
|operationType|delegatedAdminRelationshipOperationType|长时间运行的操作的类型。 可能的值是：、`delegatedAdminAccessAssignmentUpdate``unknownFutureValue`。 只读。|
|状态|delegatedAdminRelationshipOperationStatus|操作的状态。 只读。 可能的值包括 `notStarted`、`running`、`complete`、`failed`、`unknownFutureValue`。 只读。 支持 `$orderBy`。|

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
