---
title: preAuthorizedApplication 资源类型
description: 列出预授权的客户端应用程序
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 276b6f618b01d80fd66fda40c0b617a8fd01a6ac
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760972"
---
# <a name="preauthorizedapplication-resource-type"></a>preAuthorizedApplication 资源类型

命名空间：microsoft.graph

列出具有访问此应用程序 API 的指定权限的预授权客户端应用程序。 对于用户指定的权限，用户无需同意任何 (应用程序) 。 但是，未在预AuthorizedApplications中 (增量许可请求的其他权限（例如) ）将需要用户同意。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
|appId|String| 应用程序的唯一标识符。 |
|delegatedPermissionIds|字符串集合| 应用程序所需的 [oauth2PermissionScopes 的唯](permissionscope.md) 一标识符。 |

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
  "delegatedPermissionIds": ["String"]
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

