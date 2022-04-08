---
title: delegatedAdminAccessAssignment 资源类型
description: 表示将管理角色分配给 Microsoft 合作伙伴的访问容器。
author: adtangir
ms.localizationpriority: medium
ms.prod: customer-relationship-management
doc_type: resourcePageType
ms.openlocfilehash: a9d831325d211233062d93ce1ccda1128d9dfb4b
ms.sourcegitcommit: 5a43129dbf705f2d1a6afcff36af9f41ecee026d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2022
ms.locfileid: "64704336"
---
# <a name="delegatedadminaccessassignment-resource-type"></a>delegatedAdminAccessAssignment 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示使用委派管理将管理角色分配给 Microsoft 合作伙伴。 管理角色通过访问容器（如安全组) ）分配给 Microsoft 合作伙伴 (。 激活后，访问容器的成员将访问访问详细信息中指定的角色。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[创建 delegatedAdminAccessAssignment](../api/delegatedadminrelationship-post-accessassignments.md)|[delegatedAdminAccessAssignment](delegatedadminaccessassignment.md)|创建新的 **delegatedAdminAccessAssignment** 对象。|
|[列出 delegatedAdminAccessAssignments](../api/delegatedadminrelationship-list-accessassignments.md)|[delegatedAdminAccessAssignment](delegatedadminaccessassignment.md) 集合|获取 **delegatedAdminAccessAssignment** 对象及其属性的列表。|
|[获取 delegatedAdminAccessAssignment](../api/delegatedadminaccessassignment-get.md)|[delegatedAdminAccessAssignment](delegatedadminaccessassignment.md)|读取 **delegatedAdminAccessAssignment 对象的** 属性和关系。|
|[更新 delegatedAdminAccessAssignment](../api/delegatedadminaccessassignment-update.md)|[delegatedAdminAccessAssignment](delegatedadminaccessassignment.md)|更新 **delegatedAdminAccessAssignment** 对象的属性。|
|[删除 delegatedAdminAccessAssignment](../api/delegatedadminaccessassignment-delete.md)|无|删除 **delegatedAdminAccessAssignment** 对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|accessContainer|[delegatedAdminAccessContainer](../resources/delegatedadminaccesscontainer.md)|分配成员访问权限的访问容器。 例如，安全组。|
|accessDetails|[delegatedAdminAccessDetails](../resources/delegatedadminaccessdetails.md)|访问详细信息，其中包含合作伙伴在客户租户中分配的管理角色的标识符。|
|createdDateTime|DateTimeOffset|以 ISO 8601 格式和 UTC 时间创建访问分配的日期和时间。 只读。|
|id|String|访问分配的唯一标识符。 只读。 继承自 [entity](../resources/entity.md)。|
|lastModifiedDateTime|DateTimeOffset|ISO 8601 中的日期和时间，以及上次修改此访问分配时的 UTC 时间。 只读。|
|状态|delegatedAdminAccessAssignmentStatus|访问分配的状态。 只读。 可能的值包括 `pending`、`active`、`deleting`、`deleted`、`error`、`unknownFutureValue`。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.delegatedAdminAccessAssignment",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.delegatedAdminAccessAssignment",
  "id": "String (identifier)",
  "status": "String",
  "accessContainer": {
    "@odata.type": "microsoft.graph.delegatedAdminAccessContainer"
  },
  "accessDetails": {
    "@odata.type": "microsoft.graph.delegatedAdminAccessDetails"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)"
}
```

