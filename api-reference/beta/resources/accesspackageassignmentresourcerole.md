---
title: accessPackageAssignmentResourceRole 资源类型
description: 访问包分配资源角色指示主题已通过访问包分配分配的资源特定角色。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 4473c303a74cbf9e8e0c17d6c9060960590a3405
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433266"
---
# <a name="accesspackageassignmentresourcerole-resource-type"></a>accessPackageAssignmentResourceRole 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 [Azure AD 权利管理](entitlementmanagement-root.md)中，访问包分配资源角色指示主题已通过访问包分配分配的资源特定角色。

## <a name="methods"></a>Methods

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [获取 accessPackageAssignmentResourceRole](../api/accesspackageassignmentresourcerole-get.md) | [accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md)  | 检索 accessPackageAssignmentResourceRole 对象。 |
| [列出 accessPackageAssignmentResourceRoles](../api/accesspackageassignmentresourcerole-list.md) | [accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) 集合 | 检索 accessPackageAssignmentResourceRole 对象的列表。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String| 只读。|
|originId|String|与源系统相对的唯一标识符，对应于 [accessPackageResourceRole](accesspackageresourcerole.md)的 originId 属性。 |
|originSystem|String|要创建角色分配或已创建用于访问包分配的系统，例如 ，或 ， `SharePointOnline` `AadGroup` 对应于 `AadApplication` [accessPackageResourceRole](accesspackageresourcerole.md)的 originSystem 属性。|
|status|String|该值是访问包分配尚未传递到源系统以及访问包分配已传递到源系统 `PendingFulfillment` `Fulfilled` 时。|

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|accessPackageAssignments|[accessPackageAssignment](accesspackageassignment.md) 集合| 导致出现此限制的访问包角色分配。 只读。 可为 NULL。|
|accessPackageResourceRole|[accessPackageResourceRole](accesspackageresourcerole.md)| 只读。 可为 NULL。|
|accessPackageResourceScope|[accessPackageResourceScope](accesspackageresourcescope.md)| 只读。 可为 NULL。|
|accessPackageSubject|[accessPackageSubject](accesspackagesubject.md)| 只读。可为空。|


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageAssignmentResourceRole",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "originId": "String",
  "originSystem": "String",
  "status": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageAssignmentResourceRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


