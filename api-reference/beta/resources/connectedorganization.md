---
title: connectedOrganization 资源类型
description: 在 Azure AD 权利管理中，连接的组织是对用户可以请求访问权限的另一个组织的目录或域的引用。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: e31f0bb97022863f3c575fcd0321297b3f68db64
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65694902"
---
# <a name="connectedorganization-resource-type"></a>connectedOrganization 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 [Azure AD 权利管理](entitlementmanagement-overview.md)中，连接的组织是对用户可以请求访问权限的另一个组织的目录或域的引用。

## <a name="methods"></a>方法

|方法|返回类型|Description|
|:---|:---|:---|
|[列出 connectedOrganizations](../api/entitlementmanagement-list-connectedorganizations.md) | [connectedOrganization](connectedorganization.md) 集合 | 检索 connectedOrganization 对象的列表。 |
|[创建 connectedOrganization](../api/entitlementmanagement-post-connectedorganizations.md) | [connectedOrganization](connectedorganization.md) | 创建新的 connectedOrganization 对象。 |
|[获取 connectedOrganization](../api/connectedorganization-get.md) | [connectedOrganization](connectedorganization.md) | 读取 connectedOrganization 对象的属性和关系。 |
|[更新 connectedOrganization](../api/connectedorganization-update.md) | | 更新 connectedOrganization。 |
|[删除 connectedOrganization](../api/connectedorganization-delete.md) |无 | 删除 connectedOrganization。 |
|[列出 internalSponsors](../api/connectedorganization-list-internalsponsors.md) | [directoryObject](directoryobject.md) collection | 检索 connectedOrganization 的内部发起人的列表。 |
|[列出 externalSponsors](../api/connectedorganization-list-externalsponsors.md) | [directoryObject](directoryobject.md) collection | 检索 connectedOrganization 的外部发起人的列表。 |
|[添加 internalSponsors](../api/connectedorganization-post-internalsponsors.md) | 无 | 将用户或组添加到 connectedOrganization 的内部发起人。 |
|[添加 externalSponsors](../api/connectedorganization-post-externalsponsors.md) | 无 | 将用户或组添加到 connectedOrganization 的外部发起人。 |
|[删除 internalSponsors](../api/connectedorganization-delete-internalsponsors.md) | 无 | 从 connectedOrganization 的内部发起人中删除用户或组。 |
|[删除 externalSponsors](../api/connectedorganization-delete-externalsponsors.md) | 无 | 从 connectedOrganization 的外部发起人中删除用户或组。 |

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|createdBy|String|创建此资源的用户的 UPN。 只读。|
|createdDateTime|DateTimeOffset|时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。|
|说明|String|连接的组织的说明。|
|displayName|String|连接的组织的显示名称。 支持 `$filter`（`eq`）。|
|id|String| 只读。|
|modifiedBy|String|上次修改此资源的用户的 UPN。 只读。|
|modifiedDateTime|DateTimeOffset|时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。|
|state|connectedOrganizationState|连接的组织的状态定义具有请求者范围类型的 `AllConfiguredConnectedOrganizationSubjects` 分配策略是否适用。 可取值为：`configured`、`proposed`。|
|identitySources|[identitySource](identitySource.md) 集合| 此连接组织中的标识源（ [azureActiveDirectoryTenant](azureactivedirectorytenant.md)、 [crossCloudAzureActiveDirectoryTenant](crosscloudazureactivedirectorytenant.md)、 [domainIdentitySource](domainidentitysource.md) 或 [externalDomainFederation](externaldomainfederation.md) 之一）。 只读。 可为 NULL。 支持 `$select` 和 `$filter` () `eq` 。 若要按派生类型进行筛选，必须使用其完整的 OData 强制转换声明资源，例如 `$filter=identitySources/any(is:is/microsoft.graph.azureActiveDirectoryTenant/tenantId eq 'bcfdfff4-cbc3-43f2-9000-ba7b7515054f')`。|

## <a name="relationships"></a>关系

|关系|类型|描述|
|:---|:---|:---|
|internalSponsors| [directoryObject](directoryobject.md) collection| 可为 NULL。|
|externalSponsors| [directoryObject](directoryobject.md) 集合| 可为 Null。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.connectedOrganization",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdBy": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedBy": "String",
  "modifiedDateTime": "String (timestamp)",
  "identitySources": [
    {
      "@odata.type": "microsoft.graph.azureActiveDirectoryTenant",
      "tenantId": "String (identifier)",
      "displayName": "String"
    }
  ],
  "state": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "connectedOrganization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


