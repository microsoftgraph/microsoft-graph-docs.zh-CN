---
title: apiApplication 资源类型
description: 指定 Web API 应用程序的设置。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 81d0431a21ca230d96de0dd8f826a166fa16bace
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135000"
---
# <a name="apiapplication-resource-type"></a>apiApplication 资源类型

命名空间：microsoft.graph

指定实现 Web API 的应用程序的设置。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
|`acceptMappedClaims`| Boolean | 如果为 true，则允许应用程序使用声明映射，而不指定自定义签名密钥。 |
|`knownClientApplications`| Guid 集合 |如果你的解决方案包含两个部分：客户端应用和自定义 Web API 应用，用于捆绑许可。 如果将客户端应用的 appID 设置为此值，则用户仅同意客户端应用一次。 Azure AD 知道，同意客户端意味着隐式同意 Web API，并同时自动为两个 API 设置服务主体。 客户端和 Web API 应用都必须在同一租户中注册。|
|`oauth2PermissionScopes`| [permissionScope](permissionscope.md) 集合 | 由此应用程序注册表示的 Web API 公开的委派权限的定义。 这些委派权限可能由客户端应用程序请求，并且可能由用户或管理员在同意期间授予。 委派的权限有时称为 OAuth 2.0 范围。 |
|`preAuthorizedApplications`| [preAuthorizedApplication](preauthorizedapplication.md) 集合 | 列出具有访问此应用程序 API 的指定委派权限的预授权客户端应用程序。 对于用户指定的权限，用户无需同意 (授权的应用程序) 。 但是，通过增量同意（例如 (请求获取的 preAuthorizedApplications 中未) 权限将需要用户同意。 |
|`requestedAccessTokenVersion`| Int32 | 指定此资源预期的访问令牌版本。 这将更改独立于用于请求访问令牌的终结点或客户端生成的 JWT 的版本和格式。 <br><br> 使用的终结点 v1.0 或 v2.0 由客户端选择，并且仅影响 id_tokens。 资源需要显式配置 `requestedAccessTokenVersion` 以指示受支持的访问令牌格式。 <br><br> 可能的值为 `requestedAccessTokenVersion` `1` ， `2` 或 `null` 。 如果值为 `null` ，则默认值为 `1` ，对应于 v1.0 终结点。 <br><br> 如果 `signInAudience` 应用程序配置为，则 `AzureADandPersonalMicrosoftAccount` 此属性的值必须为 `2` |

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

