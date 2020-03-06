---
title: apiApplication 资源类型
description: 指定 Web API 应用程序的设置。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 94be61bf19b74ca95c4659c3bd9c8166dc7c01a1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532125"
---
# <a name="apiapplication-resource-type"></a>apiApplication 资源类型

命名空间：microsoft.graph

指定实现 Web API 的应用程序的设置。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
|`acceptMappedClaims`| Boolean | 如果为 true，则允许应用程序在未指定自定义签名密钥的情况下使用声明映射。 |
|`knownClientApplications`| Guid 集合 |如果您有一个包含两部分的解决方案，则可用于捆绑许可：客户端应用程序和自定义 web API 应用程序。 如果将客户端应用程序的 appID 设置为此值，则用户仅对客户端应用程序同意一次。 Azure AD 知道，同意客户端表示隐式同意 web API 并同时自动为这两个 Api 设置服务主体。 客户端和 web API 应用都必须在同一个租户中注册。|
|`oauth2PermissionScopes`| [permissionScope](permissionscope.md)集合 | Web API （资源）应用程序向客户端应用程序公开的 OAuth 2.0 权限范围的集合。 在同意期间，可以向客户端应用程序授予这些权限范围。 |
|`preAuthorizedApplications`| [preAuthorizedApplication](preauthorizedapplication.md)集合 | 列出使用指定委派权限预授权的客户端应用程序，以访问此应用程序的 Api。 用户无需同意任何预先授权的应用程序（针对指定的权限）。 但是，preAuthorizedApplications 中未列出的任何其他权限（例如，通过增量许可请求）将需要用户同意。 |
|`requestedAccessTokenVersion`| Int32 | 指定此资源所需的访问令牌版本。 这会更改与终结点或客户端（用于请求访问令牌）独立生成的 JWT 的版本和格式。 <br><br> 使用的终结点为 v1.0 或 v2.0，由客户端选择，只影响 id_tokens 的版本。 资源需要显式配置`requestedAccessTokenVersion` ，以指示支持的访问令牌格式。 <br><br> 的可能值`requestedAccessTokenVersion`为`1`、 `2`或`null`。 如果值为`null`，则默认为`1`，它对应于1.0 版终结点。 <br><br> 如果`signInAudience`将应用程序配置为`AzureADandPersonalMicrosoftAccount`，则此属性的值必须为`2` |

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
  "acceptMappedClaims": true,
  "knownClientApplications": ["Guid"],
  "oauth2PermissionScopes": [{"@odata.type": "microsoft.graph.permissionScope"}],
  "preAuthorizedApplications": [{"@odata.type": "microsoft.graph.preAuthorizedApplication"}],
  "requestedAccessTokenVersion": 2
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
