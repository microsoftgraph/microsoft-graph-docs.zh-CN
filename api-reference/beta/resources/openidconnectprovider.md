---
title: openIdConnectProvider 资源类型
description: 表示 Azure Active Directory B2C 租户中的 OpenIDConnect 标识提供程序。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: a51cf99f05cd9a7016adbbe0770278481fcb793d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956867"
---
# <a name="openidconnectprovider-resource-type"></a>openIdConnectProvider 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Azure Active Directory B2C 租户中的 OpenID Connect 标识提供程序。 

通过配置 B2C 租户中的 OpenID Connect 提供程序，用户可以在应用程序中使用其自定义标识提供程序进行注册和登录。

继承自 [identityProvider](../resources/identityprovider.md)。

## <a name="methods"></a>Methods

| 方法       | 返回类型  |Description|
|:---------------|:--------|:----------|
|[List](../api/identityprovider-list.md)|identityProvider 集合|检索在租户中配置的所有标识提供程序。|
|[创建](../api/identityprovider-post-identityproviders.md)|identityProvider|创建新的 OpenID Connect 标识提供程序。|
|[获取](../api/identityprovider-get.md) |identityProvider|检索 OpenID Connect 标识提供程序的属性。|
|[更新](../api/identityprovider-update.md)|无|更新 OpenID Connect 标识提供程序。|
|[删除](../api/identityprovider-delete.md)|无|删除 OpenID Connect 标识提供程序。|
|[列出可用的提供程序类型](../api/identityprovider-list-availableprovidertypes.md)|String 集合|检索所有可用的身份提供程序类型。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---------------|:--------|:----------|
|clientId|字符串|向标识提供程序注册应用程序时获取的应用程序的客户端标识符。 继承自 [identityProvider](../resources/identityprovider.md)。 这是一个必需属性。|
|clientSecret|字符串|使用身份提供程序注册应用时获取的应用客户端密码。 clientSecret 依赖于 **responseType**。 当 **responseType** `code` 为 时，身份验证代码交换需要密码。 当 **responseType** `id_token` 为密码时，由于没有代码交换，因此无需密码交换，则直接从授权响应 `id_token` 中返回 。 这是只读的。 读取操作返回" \* \* \* \* "。 继承自 [identityProvider](../resources/identityprovider.md)。|
|id|字符串|标识提供程序的 ID。 它是一个必需属性，创建后为只读。|
|name|字符串|标识提供程序的显示名称。 它是一个必需属性，创建后为只读。|
|type|字符串|标识提供程序类型。 它必须是 `OpenIDConnect` 。它是一个必需属性，创建后为只读。|
|claimsMapping|[claimsMapping](../resources/claimsmapping.md)|OIDC 提供程序将 ID 令牌发送回 Azure AD 后，Azure AD 需要能够将收到的令牌中的声明映射到 Azure AD 识别和使用声明。 此复杂类型捕获该映射。 这是一个必需属性。|
|domainHint|String|域提示可用于直接跳到指定标识提供程序的登录页面，而不是让用户在可用标识提供程序列表中进行选择。|
|metadataUrl|String|OpenID Connect 标识提供程序的元数据文档的 URL。 每个 OpenID Connect 标识提供程序都描述一个元数据文档，该文档包含执行登录所需的大部分信息。 这包括要使用的 URL 以及服务的公共签名密钥的位置等信息。 OpenID Connect 元数据文档始终位于以 .well-known/openid-configuration 结尾的终结点。 对于要添加的 OpenID Connect 标识提供程序，需要提供元数据 URL。 它是一个必需属性，创建后为只读。|
|responseMode|openIdConnectResponseMode|响应模式定义用于将数据从自定义标识提供程序发送回 Azure AD B2C 的方法。 可以使用以下响应模式 `form_post` `query` ：、。 `query` 响应模式表示代码或令牌作为查询参数返回。 `form_post` 为获得最佳安全性，建议使用响应模式。 响应通过 HTTP POST 方法传输，使用 application/x-www-form-urlencoded 格式在正文中编码代码或令牌。 这是一个必需属性。|
|responseType|[openIdConnectResponseTypes](#openidconnectresponsetypes-values)| 响应类型描述在初始调用中发送回自定义标识提供程序authorization_endpoint类型的信息。 可以使用以下响应类型 `code` `id_token` ：、、。 `token` 这是一个必需属性。|
|scope|String|范围定义要从自定义标识提供程序收集的信息和权限。 OpenID Connect 请求必须包含 openid 范围值才能从标识提供程序接收 ID 令牌。 如果没有 ID 令牌，用户将无法使用自定义标识提供程序登录到 Azure AD B2C。 其他范围可以附加空格分隔。 有关范围限制的更多详细信息，请参阅 [RFC6749 第 3.3 节](https://tools.ietf.org/html/rfc6749#section-3.3)。 这是一个必需属性。|

### <a name="openidconnectresponsetypes-values"></a>openIdConnectResponseTypes 值

|成员|说明|
|:---|:---|
|code|根据授权代码流，代码将返回到 Azure AD B2C。 Azure AD B2C 继续调用 token_endpoint 以交换令牌代码。|
|id_token|ID 令牌从自定义标识提供程序返回回 Azure AD B2C。 |
|令牌|访问令牌从自定义标识提供程序返回回 Azure AD B2C。 当前不受 Azure AD B2C 支持。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.openIdConnectProvider"
} -->

```json
{
  "id": "String",
  "name": "String",
  "type": "String",
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


