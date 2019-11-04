---
title: accessPackageAssignmentResourceRole 资源类型
description: 访问包分配资源角色指示使用者已通过访问包分配分配的特定于资源的角色。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1dbf73623ddd51cc1172e5610e84cc7861657489
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939192"
---
# <a name="accesspackageassignmentresourcerole-resource-type"></a>accessPackageAssignmentResourceRole 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在[AZURE AD 权限管理](entitlementmanagement-root.md)中，访问包分配资源角色指示已通过访问包分配分配的主题的特定于资源的角色。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 accessPackageAssignmentResourceRoles](../api/accesspackageassignmentresourcerole-list.md) | [accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md)集合 | 检索 accessPackageAssignmentResourceRole 对象的列表。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|字符串| 只读。|
|originId|字符串|相对于源系统的唯一标识符。 |
|originSystem|字符串|要为访问包分配创建角色分配的系统。|
|状态|字符串|值是`Fulfilled`访问包分配已传递到原始系统。|

## <a name="relationships"></a>关系

| 关系 | 类型        | 描述 |
|:-------------|:------------|:------------|
|accessPackageAssignments|[accessPackageAssignment](accesspackageassignment.md)集合| 此角色分配导致的访问包分配。 只读。 可为 Null。|
|accessPackageResourceRole|[accessPackageResourceRole](accesspackageresourcerole.md)| 只读。 可为 Null。|
|accessPackageResourceScope|[accessPackageResourceScope](accesspackageresourcescope.md)| 只读。 可为 Null。|
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
