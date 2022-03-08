---
title: resourceAccess 资源类型
description: 指定 OAuth 2.0 权限范围或应用程序所需的应用程序角色。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 8986b14e5dba79eaf989fd0a6bf6a4ed479f5aa0
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63333146"
---
# <a name="resourceaccess-resource-type"></a>resourceAccess 资源类型

命名空间：microsoft.graph

用于通过 [requiredResourceAccess](requiredresourceaccess.md) 资源类型的 **resourceAccess** 属性指定 OAuth 2.0 权限范围或应用程序所需的应用程序角色的对象。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|Guid|资源应用程序公开 [的应用程序角色](approle.md) 或 [委派权限](permissionScope.md) 的唯一标识符。 对于委派权限，这应该与资源应用程序的服务主体的 **oauth2PermissionScopes** 集合中委派权限之一的 **id** [属性相匹配](serviceprincipal.md)。[](permissionscope.md) 对于应用程序 (角色) ，这应该与资源应用程序的服务主体的 **appRoles** 集合中的应用角色 **的 id** [属性相匹配](serviceprincipal.md)。[](approle.md)|
|type|String|指定 **id** 属性引用委派权限还是应用程序角色 [ (](permissionscope.md)应用程序) 。[](approle.md) 可能的值包括： `Scope` (委派权限 `Role`) 或 (角色) 。|

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
  "id": "Guid",
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

