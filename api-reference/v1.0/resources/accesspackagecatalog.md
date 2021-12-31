---
title: accessPackageCatalog 资源类型
description: 访问包目录是访问包的容器。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: fa2614c7cdc70622bdab85b3afdd43666e253472
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2021
ms.locfileid: "61650676"
---
# <a name="accesspackagecatalog-resource-type"></a>accessPackageCatalog 资源类型

命名空间：microsoft.graph


在[Azure AD中](entitlementmanagement-overview.md)，访问包目录是零个或多个访问包的容器。 访问包目录还可能包含链接的资源，这些资源用于这些访问包中以提供访问权限。 若要查看或更改目录作用域角色的成员身份，请使用角色分配 [API](unifiedroleassignment.md) 和权利管理 RBAC 提供程序。



## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 accessPackageCatalogs](../api/entitlementmanagement-list-catalogs.md)|[accessPackageCatalog](accesspackagecatalog.md) 集合|检索 accessPackageCatalog 对象的列表。 |
|[创建 accessPackageCatalog](../api/entitlementmanagement-post-catalogs.md)|[accessPackageCatalog](accesspackagecatalog.md)|创建新的 accessPackageCatalog 对象。 |
|[获取 accessPackageCatalog](../api/accesspackagecatalog-get.md)|[accessPackageCatalog](accesspackagecatalog.md)|读取 accessPackageCatalog 对象的属性和关系。 |
|[更新 accessPackageCatalog](../api/accesspackagecatalog-update.md)|无|更新 accessPackageCatalog 对象的属性。 |
|[删除 accessPackageCatalog](../api/accesspackagecatalog-delete.md)|无|删除 accessPackageCatalog。 |

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|catalogType|accessPackageCatalogType|目录是由用户创建还是由权利管理创建。 可能的值包括 `userManaged`、`serviceDefault`、`serviceManaged`、`unknownFutureValue`。|
|createdDateTime|DateTimeOffset|时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。|
|说明|String|访问包目录的说明。|
|displayName|String|访问显示名称目录的索引。|
|id|String|只读。|
|isExternallyVisible|Boolean|租户外部的用户是否可以请求此目录中的访问包。|
|modifiedDateTime|DateTimeOffset|时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。 |
|state|accessPackageCatalogState|如果访问 `published` 包可用于管理，则具有 值。 可能的值包括 `unpublished`、`published`、`unknownFutureValue`。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|accessPackages|[accessPackage](accesspackage.md) 集合|此目录中的访问包。 只读。 可为 Null。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackageCatalog",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageCatalog",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "catalogType": "String",
  "state": "String",
  "isExternallyVisible": "Boolean",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)"
}
```


