---
title: resourceAccess 资源类型
description: 指定 OAuth 2.0 权限范围或应用程序所需的应用程序角色。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: 0072bf231fe8dba66b34188952804083593afaa1
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761070"
---
# <a name="resourceaccess-resource-type"></a>resourceAccess 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定 OAuth 2.0 权限范围或应用程序所需的应用程序角色。 **requiredResourceAccess** 类型的 [resourceAccess](requiredresourceaccess.md)属性是 **ResourceAccess 的集合**。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|Guid|资源应用程序公开其中一个 [oauth2PermissionScopes](permissionscope.md) 或 [appRole](approle.md) 实例的唯一标识符。|
|type|String|指定 id **属性引用** [oauth2PermissionScopes](permissionscope.md) 还是 [appRole](approle.md)。 可能的值为 `Scope` 或 `Role`。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resourceAccess"
}-->

```json
{
  "id": "guid",
  "type": "string"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "resourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


