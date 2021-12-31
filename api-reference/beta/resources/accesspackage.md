---
title: accessPackage 资源类型
description: 访问包定义资源角色的集合以及一个或多个用户如何获取对这些资源的访问权限的策略。
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 0f46825d8ae8dd1c5487a7c0f1f5b97d18337e87
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2021
ms.locfileid: "61650627"
---
# <a name="accesspackage-resource-type"></a>accessPackage 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在[Azure AD管理](entitlementmanagement-overview.md)中，访问包定义资源角色的集合以及一个或多个用户可以如何访问这些资源的策略。  

每个访问包都由一个访问包目录引用，并且具有指向该目录中的资源的链接，这些资源通过定义包提供的访问的资源特定角色作用域。  访问包还链接到访问包分配策略，其中每个策略定义可以请求或分配访问包分配的人。

若要将用户分配给访问包，请创建引用访问包和访问包分配策略的[accessPackageAssignmentRequest。](../api/entitlementmanagement-post-accesspackageassignmentrequests.md)

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 accessPackages](../api/entitlementmanagement-list-accesspackages.md) | [accessPackage](accesspackage.md) 集合 | 检索 **accesspackage 对象** 的列表。 |
| [创建 accessPackage](../api/entitlementmanagement-post-accesspackages.md) | [accessPackage](accesspackage.md) | 创建新的 **accesspackage** 对象。 |
| [获取 accessPackage](../api/accesspackage-get.md) | [accessPackage](accesspackage.md) | 读取 **accesspackage 对象的属性和** 关系。 |
| [更新 accessPackage](../api/accesspackage-update.md)|无 | 更新 **accesspackage 对象** 的属性。 |
| [删除 accessPackage](../api/accesspackage-delete.md) |无 | 删除 **accesspackage**。 |
| [列出 accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md) | [accessPackageResourceRoleScope](accesspackageresourcerolescope.md) 集合 | 检索此访问 **包的 accessPackageResourceRoleScope** 对象列表。 |
| [创建 accessPackageResourceRoleScope](../api/accesspackage-post-accesspackageresourcerolescopes.md) |无 | 为此访问 **包创建新的 accessPackageResourceRoleScope** 对象。 |
| [列出 incompatibleAccessPackages](../api/accesspackage-list-incompatibleaccesspackages.md) | [accessPackage](accesspackage.md) 集合 | 检索此访问包 **的不兼容 accesspackage** 对象的列表。 |
| [将 accessPackage 添加到 incompatibleAccessPackages](../api/accesspackage-post-incompatibleaccesspackage.md) | 无 | 添加一个链接以指示另一 **个 accesspackage** 与指定的访问包不兼容。 |
| [从 incompatibleAccessPackages 中删除 accessPackage](../api/accesspackage-delete-incompatibleaccesspackage.md) | 无 | 删除指示 **accesspackage 不兼容** 的链接。 |
| [列出 incompatibleGroups](../api/accesspackage-list-incompatiblegroups.md) | [group](group.md) 集合 | 检索此 **访问包的** 不兼容组对象的列表。 |
| [将组添加到 incompatibleGroups](../api/accesspackage-post-incompatiblegroup.md) | 无 | 添加链接以指示组的成员身份 **与** 指定的访问包不兼容。 |
| [从 incompatibleGroups 中删除组](../api/accesspackage-delete-incompatiblegroup.md) | 无 | 删除指示组成员身份 **不兼容** 的链接。|
| [列出 accessPackagesIncompatibleWith](../api/accesspackage-list-accesspackagesincompatiblewith.md) | [accessPackage](accesspackage.md) 集合 | 检索  **accesspackage 对象** 的列表，这些对象将此访问包列出为不兼容。 |
|[filterByCurrentUser](../api/accesspackage-filterbycurrentuser.md)|[accessPackage](../resources/accesspackage.md) 集合|检索在已登录用户上筛选的 **accessPackage** 对象列表。|
| [getApplicablePolicyRequirements](../api/accesspackage-getapplicablepolicyrequirements.md) | [accessPackageAssignmentRequestRequirements](../resources/accesspackageassignmentrequestrequirements.md) 集合 | 检索具有请求要求的 **accessPackageAssignmentRequestRequirement** 对象的列表。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|catalogId|String|引用此访问包的访问包目录的标识符。 只读。|
|createdBy|String|创建此资源的主题的用户或标识的 userPrincipalName。 只读。|
|createdDateTime|DateTimeOffset|时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。|
|说明|String|访问包的说明。|
|displayName|String|访问显示名称的组。 支持$filter (`eq` `contains` 、) 。|
|id|String| 只读。|
|IsHidden|布尔值|访问包是否对请求程序隐藏。|
|isRoleScopesVisible|Boolean|指示角色作用域是否可见。|
|modifiedBy|String|上次修改此资源的用户的 userPrincipalName。 只读。|
|modifiedDateTime|DateTimeOffset|时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。 |

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|accessPackageAssignmentPolicies|[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) 集合| 只读。 可为 NULL。 支持 `$expand`。|
|accessPackageCatalog|[accessPackageCatalog](accesspackagecatalog.md)| 只读。可为 NULL。|
|accessPackageResourceRoleScopes|[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) 集合| 可为 NULL。|
| incompatibleAccessPackages | [accessPackage](accesspackagecatalog.md) 集合 | 为其分配用户不符合资格分配此访问包的访问包。 |
| accessPackagesIncompatibleWith | [accessPackage](accesspackagecatalog.md) 集合 | 与此包不兼容的访问包。 只读。 |
| incompatibleGroups | [group](group.md) 集合 | 其成员无资格分配此访问包的组。 |


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


