---
title: openIdConnectIdentityProvider 资源类型
description: 表示 B2C 租户中的 OpenIDConnect Azure Active Directory提供程序。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: bbdbb83f6fd1eef7acb4cadeaca174b1e45ddbfb
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53580896"
---
# <a name="openidconnectidentityprovider-resource-type"></a>openIdConnectIdentityProvider 资源类型
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 B2C 连接中的 OpenID Azure Active Directory标识提供程序。

通过配置 B2C 连接中的 OpenID 提供程序，用户可以使用应用程序中的自定义标识提供程序进行注册和登录。

此类型将从 [identityProviderBase](../resources/identityproviderbase.md)。

## <a name="methods"></a>方法

| 方法       | 返回类型  |Description|
|:---------------|:--------|:----------|
|[List](../api/identityproviderbase-list.md)|[identityProviderBase](../resources/identityproviderbase.md)  集合|检索在租户中配置的所有标识提供程序，包括 OpenID 连接提供程序。|
|[Create](../api/identityproviderbase-post-identityproviders.md)|openIdConnectIdentityProvider|创建新的 OpenID 连接标识提供程序。|
|[Get](../api/identityproviderbase-get.md) |openIdConnectIdentityProvider|检索 OpenID 属性连接提供程序。|
|[更新](../api/identityproviderbase-update.md)|无|更新 OpenID 连接标识提供程序。|
|[删除](../api/identityproviderbase-delete.md)|无|删除 OpenID 连接标识提供程序。|
|[列出可用的提供程序类型](../api/identityproviderbase-list-availableprovidertypes.md)|String 集合|检索租户中所有可用的标识提供程序类型。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---------------|:--------|:----------|
|clientId|字符串|使用身份提供程序注册应用时获取的应用客户端 ID。 必填。|
|clientSecret|字符串|使用身份提供程序注册应用时获取的应用客户端密码。 clientSecret 依赖于 **responseType**。 <ul><li>当 **responseType** `code` 为 时，身份验证代码交换需要密码。</li><li>当 **responseType** `id_token` 为密码时不是必需的，因为没有代码交换。 授权id_token返回授权请求。</li></ul> 这是只读的。 读取操作返回 `****`。|
|id|String|标识提供程序的标识符。必填。 继承自 [identityProviderBase](../resources/identityproviderbase.md)。 只读。|
|displayName|字符串|标识提供程序的显示名称。 |
|claimsMapping|[claimsMapping](claimsmapping.md)|OIDC 提供程序将 ID 令牌发送回 Azure AD 后，Azure AD 需要能够将收到的令牌中的声明映射到 Azure AD 识别和使用声明。 此复杂类型捕获该映射。 必填。|
|domainHint|String|域提示可用于直接跳到指定标识提供程序的登录页面，而不是让用户在可用标识提供程序列表中进行选择。|
|metadataUrl|String|OpenID 元数据文档的 URL 连接提供程序。 每个 OpenID 连接标识提供程序都描述一个元数据文档，其中包含执行登录所需的大部分信息。 这包括要使用的 URL 以及服务的公共签名密钥的位置等信息。 OpenID 连接元数据文档始终位于 以 结尾的终结点 `.well-known/openid-configuration` 。 提供您添加的 OpenID 连接标识提供程序的元数据 URL。 只读。 必填。|
|responseMode|String|响应模式定义用于将数据从自定义标识提供程序发送回 Azure AD B2C 的方法。 可能的值 `form_post` `query` ：、。 必填。|
|responseType|String|响应类型描述在初始调用中发送回自定义标识提供程序authorization_endpoint类型。 可能的值 `code` `id_token` `token` ：、、。  必填。|
|scope|String|范围定义要从自定义标识提供程序收集的信息和权限。 OpenID 连接请求必须包含 openid 范围值才能从标识提供程序接收 ID 令牌。 如果没有 ID 令牌，用户将无法使用自定义标识提供程序登录到 Azure AD B2C。 其他范围可以追加，用空格分隔。 有关范围限制的更多详细信息，请参阅 [RFC6749 第 3.3 节](https://tools.ietf.org/html/rfc6749#section-3.3)。 必填。|

### <a name="responsemode-value"></a>responseMode 值
|值|说明|
:--------|:----------|
|form_post|为获得最佳安全性，建议采用此响应模式。 响应通过 HTTP POST 方法传输，使用 application/x-www-form-urlencoded 格式在正文中编码代码或令牌。|
|查询|代码或令牌作为查询参数返回。|

### <a name="responsetype-value"></a>responseType 值
|值|说明|
:--------|:----------|
|code|根据授权代码流，代码将返回到 Azure AD B2C。 Azure AD B2C 继续调用 token_endpoint 以交换令牌代码。|
|id_token|ID 令牌从自定义标识提供程序返回回 Azure AD B2C。|
|令牌|访问令牌从自定义标识提供程序返回回 Azure AD B2C。  (当前 Azure AD B2C 不支持) |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.openIdConnectIdentityProvider"
} -->

```json
{
  "id": "String",
  "displayName": "String",
  "clientId": "String",
  "clientSecret": "String",
  "claimsMapping": {
      "@odata.type": "#microsoft.graph.claimsMapping",
      "userId": "String",
      "givenName": "String",
      "surname": "String",
      "email": "String",
      "displayName": "String"
  },
  "domainHint": "String",
  "metadataUrl": "String",
  "responseMode": "String",
  "responseType": "String",
  "scope": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2021-03-30 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
 "description": "openidconnectIdentityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
