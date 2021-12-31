---
title: accessPackage 资源类型
description: 访问包定义资源角色的集合以及一个或多个用户如何获取对这些资源的访问权限的策略。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 226715a4678b593e68a8364e326950c7af019212
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2021
ms.locfileid: "61651454"
---
# <a name="accesspackage-resource-type"></a>accessPackage 资源类型

命名空间：microsoft.graph

在[Azure AD管理](entitlementmanagement-overview.md)中，访问包定义资源角色的集合以及一个或多个用户可以如何访问这些资源的策略。  

每个访问包都由一个访问包目录引用，并且具有指向该目录中的资源的链接，这些资源通过定义包提供的访问的资源特定角色作用域。  访问包还链接到访问包分配策略，其中每个策略定义可以请求或分配访问包分配的人。



## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 accessPackages](../api/entitlementmanagement-list-accesspackages.md)|[accessPackage](accesspackage.md) 集合|检索 **accesspackage 对象** 的列表。 |
|[创建 accessPackage](../api/entitlementmanagement-post-accesspackages.md)|[accessPackage](accesspackage.md)|创建新的 **accesspackage** 对象。 |
|[获取 accessPackage](../api/accesspackage-get.md)|[accessPackage](accesspackage.md)|读取 **accesspackage 对象的属性和** 关系。 |
|[更新 accessPackage](../api/accesspackage-update.md)|无|更新 **accesspackage 对象** 的属性。 |
|[删除 accessPackage](../api/accesspackage-delete.md)|无|删除 **accesspackage**。 |
|[filterByCurrentUser](../api/accesspackage-filterbycurrentuser.md)|[accessPackage](../resources/accesspackage.md) 集合|检索在已登录用户上筛选的 **accessPackage** 对象列表。|
|[getApplicablePolicyRequirements](../api/accesspackage-getapplicablepolicyrequirements.md)|[accessPackageAssignmentRequestRequirements](../resources/accesspackageassignmentrequestrequirements.md) 集合|检索具有请求要求的 **accessPackageAssignmentRequestRequirement** 对象的列表。 |

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。|
|说明|String|访问包的说明。|
|displayName|String|访问显示名称的组。 支持$filter (`eq` `contains` 、) 。|
|id|String|只读。|
|IsHidden|布尔值|访问包是否对请求程序隐藏。|
|modifiedDateTime|DateTimeOffset|时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。 |

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|catalog|[accessPackageCatalog](../resources/accesspackagecatalog.md)|只读。可为空。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackage",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackage",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "isHidden": "Boolean",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)"
}
```


