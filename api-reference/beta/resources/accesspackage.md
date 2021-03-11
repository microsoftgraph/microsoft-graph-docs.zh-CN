---
title: accessPackage 资源类型
description: 访问包定义资源角色的集合以及一个或多个用户如何访问这些资源的策略。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 98e9a22137f9f6faaa39fbbb010a32b40f8f0254
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720835"
---
# <a name="accesspackage-resource-type"></a>accessPackage 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 [Azure AD 权利管理](entitlementmanagement-root.md)中，访问包定义资源角色的集合以及一个或多个用户可以如何访问这些资源的策略。  
每个访问包都由单个访问包目录引用，并且具有通过定义包提供的访问的资源特定角色作用域从该目录访问资源的链接。  访问包还链接到访问包分配策略，其中每个策略定义可以请求或分配访问包分配的人。

若要将用户分配给访问包，请创建引用访问包和访问包分配策略的[accessPackageAssignmentRequest。](../api/accesspackageassignmentrequest-post.md)

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 accessPackages](../api/accesspackage-list.md) | [accessPackage](accesspackage.md) 集合 | 检索 **accesspackage 对象** 的列表。 |
| [创建 accessPackage](../api/accesspackage-post.md) | [accessPackage](accesspackage.md) | 创建新的 **accesspackage** 对象。 |
| [获取 accessPackage](../api/accesspackage-get.md) | [accessPackage](accesspackage.md) | 读取 **accesspackage 对象的属性和** 关系。 |
| [更新 accessPackage](../api/accesspackage-update.md)|无 | 更新 **accesspackage** 对象的属性。 |
| [删除 accessPackage](../api/accesspackage-delete.md) |无 | 删除 **accesspackage**。 |
| [列出 accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md) | [accessPackageResourceRoleScope](accesspackageresourcerolescope.md) 集合 | 检索此访问 **包的 accessPackageResourceRoleScope** 对象列表。 |
| [创建 accessPackageResourceRoleScope](../api/accesspackage-post-accesspackageresourcerolescopes.md) |无 | 为此访问 **包创建新的 accessPackageResourceRoleScope** 对象。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|catalogId|String|引用此访问包的访问包目录的 ID。 只读。|
|createdBy|String|创建此资源的主题的用户或标识的 UPN。 只读。|
|createdDateTime|DateTimeOffset|时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。|
|说明|String|访问包的说明。|
|displayName|String|访问显示名称的组。|
|id|String| 只读。|
|isHidden|布尔|访问包是否对请求程序隐藏。|
|isRoleScopesVisible|布尔|指示角色作用域是否可见。|
|modifiedBy|String|上次修改此资源的用户的 UPN。 只读。|
|modifiedDateTime|DateTimeOffset|时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。 |

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|accessPackageAssignmentPolicies|[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) 集合| 只读。 可为 NULL。|
|accessPackageCatalog|[accessPackageCatalog](accesspackagecatalog.md)| 只读。 可为 NULL。|
|accessPackageResourceRoleScopes|[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) 集合| 可为 Null。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackage",
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


