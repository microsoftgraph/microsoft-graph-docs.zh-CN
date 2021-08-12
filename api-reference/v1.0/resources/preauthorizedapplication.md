---
title: preAuthorizedApplication 资源类型
description: 列出预授权的客户端应用程序
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: f59bdd28a23ff92705914ba6361bcce860df4650791c8dcabd22f96753fc0f50
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54202145"
---
# <a name="preauthorizedapplication-resource-type"></a>preAuthorizedApplication 资源类型

命名空间：microsoft.graph

列出具有访问此应用程序 API 的指定权限的预授权客户端应用程序。 对于用户指定的权限，用户无需同意任何 (应用程序) 。 但是，未在预AuthorizedApplications中 (增量许可请求的其他权限（例如) ）将需要用户同意。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
|appId|String| 应用程序的唯一标识符。 |
|permissionIds|String collection| 应用程序所需的 [oauth2PermissionScopes 的唯](permissionscope.md) 一标识符。 |

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

