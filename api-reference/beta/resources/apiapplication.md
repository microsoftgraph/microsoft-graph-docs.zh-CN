---
title: api 资源类型
description: 指定 Web API 应用程序的设置。
localization_priority: Normal
ms.openlocfilehash: f26a568d05c85059e914b355d971755f19627cac
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348350"
---
# <a name="api-resource-type"></a>api 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定 Web API 应用程序的设置。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
|requestedAccessTokenVersion|Int32| 为当前 API 资源指定接受的访问令牌版本。 可能的值为1或2。  |
|oauth2PermissionScopes|[permissionScope](permissionscope.md)集合| web API (资源) 应用程序向客户端应用程序公开的 OAuth 2.0 权限范围的集合。 在同意期间, 可以向客户端应用程序授予这些权限范围。 |

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.apiApplication"
}-->

```json
{
  "requestedAccessTokenVersion": 1,
  "oauth2PermissionScopes": [{"@odata.type": "microsoft.graph.permissionScope"}]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "api resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
