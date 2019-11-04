---
title: accessPackage 资源类型
description: 访问包定义了资源角色的集合，以及一个或多个用户如何获取对这些资源的访问权限的策略。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e4d7565cdb16eb2a6a0abb7a33344c70490e2616
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939220"
---
# <a name="accesspackage-resource-type"></a>accessPackage 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在[AZURE AD 权限管理](entitlementmanagement-root.md)中，访问包定义了资源角色的集合，以及一个或多个用户如何获取对这些资源的访问权限的策略。  
每个访问包都由一个访问包目录引用，并从该目录中的资源链接到来自定义该程序包提供的访问权限的特定于资源的角色作用域。  访问包还链接到访问包分配策略，每个分配策略都定义了可以请求或分配访问包分配的成员。

若要将用户分配到访问包，请[创建一个](../api/accesspackageassignmentrequest-post.md)引用访问包和访问包分配策略的 accessPackageAssignmentRequest。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 accessPackages](../api/accesspackage-list.md) | [accessPackage](accesspackage.md)集合 | 检索**accesspackage**对象的列表。 |
| [创建 accessPackage](../api/accesspackage-post.md) | [accessPackage](accesspackage.md) | 创建新的**accesspackage**对象。 |
| [获取 accessPackage](../api/accesspackage-get.md) | [accessPackage](accesspackage.md) | 读取**accesspackage**对象的属性和关系。 |
| [删除 accessPackage](../api/accesspackage-delete.md) | | 删除**accesspackage**。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 描述 |
|:-------------|:------------|:------------|
|catalogId|字符串|引用此访问包的访问包目录的 ID。 只读。|
|createdBy|字符串|创建此资源的主题的用户或标识的 UPN。 只读。|
|createdDateTime|DateTimeOffset|时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。 只读。|
|说明|String|访问包的说明。|
|displayName|String|访问包的显示名称。|
|id|字符串| 只读。|
|isHidden|Boolean|访问包是否在请求程序中是隐藏的。|
|isRoleScopesVisible|Boolean|指示角色范围是否可见。|
|modifiedBy|字符串|上次修改此资源的用户的 UPN。 只读。|
|modifiedDateTime|DateTimeOffset|时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。 只读。 |

## <a name="relationships"></a>关系

| 关系 | 类型        | 描述 |
|:-------------|:------------|:------------|
|accessPackageAssignmentPolicies|[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md)集合| 此为只读属性。 可为 Null。|
|accessPackageCatalog|[accessPackageCatalog](accesspackagecatalog.md)| 此为只读属性。 可为 Null。|
|accessPackageResourceRoleScopes|[accessPackageResourceRoleScope](accesspackageresourcerolescope.md)集合| 可为 Null。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackage",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
    "id":"360fa7de-90be-48dc-a2ce-fc40094a93dd",
    "description":"Sample access package",
    "displayName":"Access package for testing",
    "isHidden":false,
    "catalogId":"662d99e7-6ceb-4c21-9cb4-9b0bbfdefccc",
    "isRoleScopesVisible":false,
    "createdDateTime":"2019-01-27T18:19:50.74Z",
    "modifiedDateTime":"2019-01-27T18:19:50.74Z",
    "createdBy":"TestGA@example.com",
    "modifiedBy":"TestGA@example.com"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackage resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
