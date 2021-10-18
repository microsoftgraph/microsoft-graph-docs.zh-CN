---
title: resourceAccess 资源类型
description: 指定 OAuth 2.0 权限范围或应用程序所需的应用程序角色。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 5feb228b1cc29d6a2f608431520cca78591f8b5b
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2021
ms.locfileid: "60452655"
---
# <a name="resourceaccess-resource-type"></a>resourceAccess 资源类型

命名空间：microsoft.graph

用于通过 [requiredResourceAccess](requiredresourceaccess.md)资源类型的 **resourceAccess** 属性指定 OAuth 2.0 权限范围或应用程序所需的应用程序角色的对象。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|GUID|资源应用程序公开其中一个 [oauth2PermissionScopes](permissionscope.md) 或 [appRole](approle.md) 实例的唯一标识符。|
|type|String|指定 id **属性引用** [oauth2PermissionScopes](permissionscope.md) 还是 [appRole](approle.md)。 可能的值包括 `Scope` ： (OAuth 2.0 权限范围) 或 (`Role` 应用角色) 。|

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
  "id": "GUID",
  "type": "String"
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

