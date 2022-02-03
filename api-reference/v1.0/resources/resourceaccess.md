---
title: resourceAccess 资源类型
description: 指定 OAuth 2.0 权限范围或应用程序所需的应用程序角色。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 18b1c5b3f42b3f7203363a95b94ed1cf036e7fed
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62347995"
---
# <a name="resourceaccess-resource-type"></a>resourceAccess 资源类型

命名空间：microsoft.graph

用于通过 [requiredResourceAccess](requiredresourceaccess.md) 资源类型的 **resourceAccess** 属性指定 OAuth 2.0 权限范围或应用程序所需的应用程序角色的对象。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|Guid|资源应用程序公开 [的应用程序角色](approle.md) 或 [委派权限](permissionScope.md) 的唯一标识符。 对于委派权限，这应该与资源应用程序的服务主体的 **oauth2PermissionScopes** 集合中委派权限之一的 **id** [属性相匹配](serviceprincipal.md)。[](permissionscope.md) 对于应用程序 (权限) ，这应该与资源应用程序服务主体的 **appRoles** 集合中的应用角色 **的 id** [属性相匹配](serviceprincipal.md)。[](approle.md)|
|type|String|指定 **id** 属性引用委派权限还是应用程序角色 [ (](permissionscope.md)应用程序) 。[](approle.md) 可能的值包括： `Scope` (`Role` 权限) 或 (角色) 。|

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

