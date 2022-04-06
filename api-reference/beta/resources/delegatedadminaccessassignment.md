---
title: delegatedAdminAccessAssignment 资源类型
description: 表示向 Microsoft 合作伙伴的访问容器分配管理角色。
author: adtangir
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: eec8597ffa629b919a7f9b7a9f9d22fbdcde2217
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589616"
---
# <a name="delegatedadminaccessassignment-resource-type"></a>delegatedAdminAccessAssignment 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示使用委派管理向 Microsoft 合作伙伴分配管理角色。 管理角色通过访问容器（如安全组角色） (分配给 Microsoft) 。 一旦处于活动状态，访问容器的成员将有权访问访问详细信息中指定的角色。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[创建 delegatedAdminAccessAssignment](../api/delegatedadminrelationship-post-accessassignments.md)|[delegatedAdminAccessAssignment](delegatedadminaccessassignment.md)|创建新的 **delegatedAdminAccessAssignment** 对象。|
|[列出 delegatedAdminAccessAssignments](../api/delegatedadminrelationship-list-accessassignments.md)|[delegatedAdminAccessAssignment](delegatedadminaccessassignment.md) 集合|获取 **delegatedAdminAccessAssignment** 对象及其属性的列表。|
|[获取 delegatedAdminAccessAssignment](../api/delegatedadminaccessassignment-get.md)|[delegatedAdminAccessAssignment](delegatedadminaccessassignment.md)|读取 **delegatedAdminAccessAssignment** 对象的属性和关系。|
|[更新 delegatedAdminAccessAssignment](../api/delegatedadminaccessassignment-update.md)|[delegatedAdminAccessAssignment](delegatedadminaccessassignment.md)|更新 **delegatedAdminAccessAssignment 对象** 的属性。|
|[删除 delegatedAdminAccessAssignment](../api/delegatedadminaccessassignment-delete.md)|无|删除 **delegatedAdminAccessAssignment** 对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|accessContainer|[delegatedAdminAccessContainer](../resources/delegatedadminaccesscontainer.md)|向成员分配访问权限的访问容器。 例如，安全组。|
|accessDetails|[delegatedAdminAccessDetails](../resources/delegatedadminaccessdetails.md)|包含合作伙伴在客户租户中分配的管理角色标识符的访问详细信息。|
|createdDateTime|DateTimeOffset|创建访问分配时采用 ISO 8601 格式的日期和时间，采用 UTC 时间。 只读。|
|id|String|访问分配的唯一标识符。 只读。 继承自 [entity](../resources/entity.md)。|
|lastModifiedDateTime|DateTimeOffset|上次修改此访问分配时，ISO 8601 和 UTC 时间中的日期和时间。 只读。|
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

