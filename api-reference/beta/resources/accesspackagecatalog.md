---
title: accessPackageCatalog 资源类型
description: 访问包目录是访问包的容器。
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 6122c36481204c7f6e7269839be625e45db5432a
ms.sourcegitcommit: 0249c86925c9b4797908394c952073b5d9137911
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2022
ms.locfileid: "64477466"
---
# <a name="accesspackagecatalog-resource-type"></a>accessPackageCatalog 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在[Azure AD中，](entitlementmanagement-overview.md)访问包目录是零个或多个访问包的容器。 Azure AD权限管理包括一个名为"常规"的内置 **目录**。

访问包目录还可能包含链接的资源，这些资源用于这些访问包中以提供访问权限。 若要查看或更改目录作用域角色的成员身份，请使用角色 [分配 API 和](unifiedroleassignment.md) 权利管理 RBAC 提供程序。


## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 accessPackageCatalogs](../api/entitlementmanagement-list-accesspackagecatalogs.md) | [accessPackageCatalog](accesspackagecatalog.md) 集合 | 检索 accesspackagecatalog 对象的列表。 |
| [创建 accessPackageCatalog](../api/entitlementmanagement-post-accesspackagecatalogs.md) | [accessPackageCatalog](accesspackagecatalog.md) | 创建新的 accessPackageCatalog 对象。 |
| [获取 accessPackageCatalog](../api/accesspackagecatalog-get.md) | [accessPackageCatalog](accesspackagecatalog.md) | 读取 accessPackageCatalog 对象的属性和关系。 |
| [更新 accessPackageCatalog](../api/accesspackagecatalog-update.md)|无 | 更新 accessPackageCatalog 对象的属性。 |
| [删除 accessPackageCatalog](../api/accesspackagecatalog-delete.md) | | 删除 accessPackageCatalog。 |
| **访问包资源**| | |
| [列出 accessPackageCatalog 资源](../api/accesspackagecatalog-list-accesspackageresources.md) | [accessPackageResource](accesspackageresource.md) 集合 | 检索目录中的 accessPackageResource 对象列表。 |
| **访问包资源角色**| | |
| [列出 accessPackageCatalog 资源角色](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | [accessPackageResourceRole](accesspackageresourcerole.md) 集合 | 检索目录中资源的 accessPackageResourceRole 对象列表。 |
| **自定义访问包包工作流扩展**| | |
|[列出 customAccessPackageWorkflowExtensions](../api/accesspackagecatalog-list-customaccesspackageworkflowextensions.md)|[customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md) 集合|获取 [customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md) 对象及其属性的列表。|
|[Create customAccessPackageWorkflowExtensions](../api/accesspackagecatalog-post-customaccesspackageworkflowextensions.md)|[customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md)|创建新的 [customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md) 对象。|
|[获取 customAccessPackageWorkflowExtension](../api/customaccesspackageworkflowextension-get.md)|[customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md)|读取 [customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md) 对象的属性和关系。|
|[更新 customAccessPackageWorkflowExtension](../api/customaccesspackageworkflowextension-update.md)|[customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md)|更新 [customAccessPackageWorkflowExtension 对象](../resources/customaccesspackageworkflowextension.md) 的属性。|
|[删除 customAccessPackageWorkflowExtension](../api/customaccesspackageworkflowextension-delete.md)|无|删除 [customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md) 对象。|

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|catalogStatus|String|如果访问 `Published` 包可用于管理，则具有 值。|
|catalogType|String|`UserManaged`或`ServiceDefault`之一。 |
|createdBy|String|创建此资源的用户的 UPN。 只读。|
|createdDateTime|DateTimeOffset|时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。|
|说明|String|访问包目录的说明。|
|displayName|String|访问显示名称目录的索引。 支持 `$filter`（`eq`、`contains`）。|
|id|String| 只读。|
|isExternallyVisible|Boolean|租户外部的用户是否可以请求此目录中的访问包。|
|modifiedBy|String|上次修改此资源的用户的 UPN。 只读。|
|modifiedDateTime|DateTimeOffset|时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。 |


## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|accessPackages|[accessPackage](accesspackage.md) 集合| 此目录中的访问包。 只读。 可为 NULL。 支持 `$expand`。|
|accessPackageResources|[accessPackageResource](accesspackageresource.md) 集合| 只读。可为空。|
|accessPackageResourceRoles|[accessPackageResourceRole](accesspackageresourcerole.md) 集合|目录的每个资源中的角色。 只读。|
|accessPackageResourceScopes|[accessPackageResourceScope](accesspackageresourcescope.md) 集合|只读。|
|customAccessPackageWorkflowExtension|[customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md) 集合|逻辑应用的属性，可以在访问包请求和分配周期的各个阶段调用这些属性。 |

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

