---
title: accessPackageAssignmentResourceRole 资源类型
description: 访问包分配资源角色指示主题通过访问包分配分配的资源特定角色。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2b4893d40db8b5ac70a2ac3093d8dfbdf55c3175
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155596"
---
# <a name="accesspackageassignmentresourcerole-resource-type"></a>accessPackageAssignmentResourceRole 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 [Azure AD 权利管理](entitlementmanagement-root.md)中，访问包分配资源角色指示主题通过访问包分配分配的资源特定角色。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [获取 accessPackageAssignmentResourceRole](../api/accesspackageassignmentresourcerole-get.md) | [accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md)  | 检索 accessPackageAssignmentResourceRole 对象。 |
| [列出 accessPackageAssignmentResourceRoles](../api/accesspackageassignmentresourcerole-list.md) | [accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) 集合 | 检索 accessPackageAssignmentResourceRole 对象的列表。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String| 只读。|
|originId|String|相对于源系统的唯一标识符，对应于 [accessPackageResourceRole](accesspackageresourcerole.md)的 originId 属性。 |
|originSystem|String|要创建或角色分配访问包分配（例如，或）与 `SharePointOnline` `AadGroup` `AadApplication` [accessPackageResourceRole](accesspackageresourcerole.md)的 originSystem 属性相对应的系统。|
|status|String|该值是访问包分配尚未传递到源系统，以及访问包分配已传递到源 `PendingFulfillment` `Fulfilled` 系统时。|

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|accessPackageAssignments|[accessPackageAssignment](accesspackageassignment.md) 集合| 访问包分配导致此角色分配。 只读。 可为 NULL。|
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


