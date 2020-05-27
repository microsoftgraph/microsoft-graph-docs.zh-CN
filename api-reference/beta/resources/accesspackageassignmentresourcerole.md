---
title: accessPackageAssignmentResourceRole 资源类型
description: 访问包分配资源角色指示使用者已通过访问包分配分配的特定于资源的角色。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6ef0827736d16f1dbf3aedfb664467011e75e7b2
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2020
ms.locfileid: "44383775"
---
# <a name="accesspackageassignmentresourcerole-resource-type"></a>accessPackageAssignmentResourceRole 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在[AZURE AD 权限管理](entitlementmanagement-root.md)中，访问包分配资源角色指示已通过访问包分配分配的主题的特定于资源的角色。

## <a name="methods"></a>Methods

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [获取 accessPackageAssignmentResourceRole](../api/accesspackageassignmentresourcerole-get.md) | [accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md)  | 检索 accessPackageAssignmentResourceRole 对象。 |
| [列出 accessPackageAssignmentResourceRoles](../api/accesspackageassignmentresourcerole-list.md) | [accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md)集合 | 检索 accessPackageAssignmentResourceRole 对象的列表。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String| 只读。|
|originId|String|相对于源系统的唯一标识符。 |
|originSystem|String|要在其中创建角色分配或为访问包分配创建的系统，例如 `SharePointOnline` 。|
|status|String|值是 `Fulfilled` 访问包分配已传递到原始系统。|

## <a name="relationships"></a>关系

| 关系 | 类型        | Description |
|:-------------|:------------|:------------|
|accessPackageAssignments|[accessPackageAssignment](accesspackageassignment.md)集合| 此角色分配导致的访问包分配。 只读。 可为 NULL。|
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
  "baseType": "",
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
