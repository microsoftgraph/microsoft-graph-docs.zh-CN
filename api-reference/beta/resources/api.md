---
title: api 资源类型
description: 指定 Web API 应用程序的设置。
localization_priority: Normal
ms.openlocfilehash: 50c21c31fec7434514408e1a214c6edf2b838c98
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845204"
---
# <a name="api-resource-type"></a>api 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

指定 Web API 应用程序的设置。

## <a name="properties"></a>属性

| 属性 | 类型 | Description |
|:---------------|:--------|:----------|
|requestedAccessTokenVersion|Int32| 指定当前 API 资源的接受的访问令牌版本。 可能的值为 1 或 2。  |
|oauth2PermissionScopes|[permissionScope](permissionscope.md)集合| 客户端应用程序公开 web API （资源） 应用程序的 OAuth 2.0 权限范围的集合。 这些权限范围可能期间同意授予客户端应用程序。 |

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.api"
}-->

```json
{
  "requestedAccessTokenVersion": 1,
  "oauth2PermissionScopes": [{"@odata.type": "microsoft.graph.permissionScope"}]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "api resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
