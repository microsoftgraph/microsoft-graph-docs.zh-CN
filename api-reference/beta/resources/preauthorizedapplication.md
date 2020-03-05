---
title: preAuthorizedApplication 资源类型
description: 列出预授权的客户端应用程序
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: b84e9a49d293978754a06bdae229806f529690ba
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521577"
---
# <a name="preauthorizedapplication-resource-type"></a>preAuthorizedApplication 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

列出使用指定权限预授权的客户端应用程序，以访问此应用程序的 Api。 用户无需同意任何预先授权的应用程序（针对指定的权限）。 但是，preAuthorizedApplications 中未列出的任何其他权限（例如，通过增量许可请求）将需要用户同意。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
|appId|String| 应用程序的唯一标识符。 |
|permissionIds|String 集合| 应用程序所需的[oauth2PermissionScopes](permissionscope.md)的唯一标识符。 |

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.preAuthorizedApplication"
}-->

```json
{
  "appId": "String",
  "permissionIds": ["String"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "preAuthorizedApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
