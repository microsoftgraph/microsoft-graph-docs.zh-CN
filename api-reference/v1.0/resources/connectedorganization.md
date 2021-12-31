---
title: connectedOrganization 资源类型
description: 在Azure AD管理中，连接的组织是一个对用户可以请求访问权限的另一个组织的目录或域的引用。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 30f8ed82aba6a9e4ab22f90dca8f9c912ba2e947
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2021
ms.locfileid: "61651201"
---
# <a name="connectedorganization-resource-type"></a>connectedOrganization 资源类型

命名空间：microsoft.graph


在[Azure AD管理](entitlementmanagement-overview.md)中，连接的组织是一个对另一个组织（其用户可以请求访问）的目录或域的引用。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 connectedOrganizations](../api/entitlementmanagement-list-connectedorganizations.md)|[connectedOrganization](connectedorganization.md) 集合|检索 connectedOrganization 对象的列表。 |
|[创建 connectedOrganization](../api/entitlementmanagement-post-connectedorganizations.md)|[connectedOrganization](connectedorganization.md)|创建新的 connectedOrganization 对象。 |
|[获取 connectedOrganization](../api/connectedorganization-get.md)|[connectedOrganization](connectedorganization.md)|读取 connectedOrganization 对象的属性和关系。 |
|[更新 connectedOrganization](../api/connectedorganization-update.md)|[connectedOrganization](connectedorganization.md) 集合|更新 connectedOrganization。 |
|[删除 connectedOrganization](../api/connectedorganization-delete.md)|无|删除 connectedOrganization。 |
|[列出 externalSponsors](../api/connectedorganization-list-externalsponsors.md)|[directoryObject](directoryobject.md) collection|检索 connectedOrganization 的外部发起人的列表。 |
|[添加 externalSponsors](../api/connectedorganization-post-externalsponsors.md)|无|将用户或组添加到 connectedOrganization 的外部发起人。 |
|[列出 internalSponsors](../api/connectedorganization-list-internalsponsors.md)|[directoryObject](directoryobject.md) collection|检索 connectedOrganization 的内部发起人的列表。 |
|[添加 internalSponsors](../api/connectedorganization-post-internalsponsors.md)|无|将用户或组添加到 connectedOrganization 的内部发起人。 |
|[删除 internalSponsors](../api/connectedorganization-delete-internalsponsors.md)|无|从 connectedOrganization 的内部发起人中删除用户或组。 |
|[删除 externalSponsors](../api/connectedorganization-delete-externalsponsors.md)|无|从 connectedOrganization 的外部发起人中删除用户或组。 |

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。|
|说明|String|已连接组织的说明。|
|displayName|String|已显示名称组织的成员。 支持 `$filter`（`eq`）。|
|id|String|只读。|
|identitySources|[identitySource](../resources/identitysource.md) 集合|此已连接组织中的身份源[，azureActiveDirectoryTenant、domainIdentitySource](azureactivedirectorytenant.md)或[externalDomainFederation 之一](externaldomainfederation.md)。 [](domainidentitysource.md) 可为 NULL。|
|modifiedDateTime|DateTimeOffset|*时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。|
|state|connectedOrganizationState|已连接组织的状态定义具有请求者作用域类型的分配策略 `AllConfiguredConnectedOrganizationSubjects` 是否适用。  可能的值包括 `configured`、`proposed`、`unknownFutureValue`。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|externalSponsors|[directoryObject](directoryobject.md) 集合|可为 NULL。|
|internalSponsors|[directoryObject](directoryobject.md) collection|可为 Null。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.connectedOrganization",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.connectedOrganization",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "identitySources": [
    {
      "@odata.type": "microsoft.graph.azureActiveDirectoryTenant"
    }
  ],
  "state": "String"
}
```


