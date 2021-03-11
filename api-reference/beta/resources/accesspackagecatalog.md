---
title: accessPackageCatalog 资源类型
description: 访问包目录是访问包的容器。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 87c2541179cd94472eadab692544a40a1d8b81b7
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720422"
---
# <a name="accesspackagecatalog-resource-type"></a>accessPackageCatalog 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 [Azure AD 权利管理](entitlementmanagement-root.md)中，访问包目录是零个或多个访问包的容器。  访问包目录可能还具有链接的资源，这些资源用于这些访问包以提供访问权限。


## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 accessPackageCatalogs](../api/accesspackagecatalog-list.md) | [accessPackageCatalog](accesspackagecatalog.md) 集合 | 检索 accesspackagecatalog 对象的列表。 |
| [创建 accessPackageCatalog](../api/accesspackagecatalog-post.md) | [accessPackageCatalog](accesspackagecatalog.md) | 创建新的 accessPackageCatalog 对象。 |
| [获取 accessPackageCatalog](../api/accesspackagecatalog-get.md) | [accessPackageCatalog](accesspackagecatalog.md) | 读取 accessPackageCatalog 对象的属性和关系。 |
| [更新 accessPackageCatalog](../api/accesspackagecatalog-update.md)|无 | 更新 accessPackageCatalog 对象的属性。 |
| [删除 accessPackageCatalog](../api/accesspackagecatalog-delete.md) | | 删除 accessPackageCatalog。 |
| [列出 accessPackageCatalog 资源](../api/accesspackagecatalog-list-accesspackageresources.md) | [accessPackageResource](accesspackageresource.md) 集合 | 检索目录中 accessPackageResource 对象的列表。 |
| [列出 accessPackageCatalog 资源角色](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | [accessPackageResourceRole](accesspackageresourcerole.md) 集合 | 检索目录中资源的 accessPackageResourceRole 对象列表。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|catalogStatus|String|如果访问 `Published` 包可用于管理，则具有值。|
|catalogType|String|或 `UserManaged` `ServiceDefault` 。 |
|createdBy|String|创建此资源的用户的 UPN。 只读。|
|createdDateTime|DateTimeOffset|时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。|
|说明|String|访问包目录的说明。|
|displayName|String|访问显示名称目录的索引。|
|id|String| 只读。|
|isExternallyVisible|布尔|租户外部的用户是否可以请求此目录中的访问包。|
|modifiedBy|String|上次修改此资源的用户的 UPN。 只读。|
|modifiedDateTime|DateTimeOffset|时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。 |


## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|accessPackages|[accessPackage](accesspackage.md) 集合| 此目录中的访问包。 只读。 可为 NULL。|
|accessPackageResources|[accessPackageResource](accesspackageresource.md) 集合| 只读。可为空。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageCatalog",
  "keyProperty": "id"
}-->

```json
{
    "id":"360fa7de-90be-48dc-a2ce-fc40094a93dd",
    "description":"Sample access package catalog",
    "displayName":"Access package catalog for testing",
    "isExternallyVisible":false,
    "catalogType":"UserManaged",
    "catalogStatus":"Published",
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
  "description": "accessPackageCatalog resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


