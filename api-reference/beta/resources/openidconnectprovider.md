---
title: openIdConnectProvider 资源类型
description: 表示 Azure Active Directory B2C 租户中的 OpenIDConnect 标识提供程序。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: namkedia
ms.openlocfilehash: 9a7567ee550432dc5a0d98ce9c3a6ae7c51a0160
ms.sourcegitcommit: c6e8a2097267ace4c78124be48646f9129114b26
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/03/2020
ms.locfileid: "47340007"
---
# <a name="openidconnectprovider-resource-type"></a>openIdConnectProvider 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Azure Active Directory B2C 租户中的 OpenID Connect 标识提供程序。 

在 B2C 租户中配置 OpenID Connect provider 使用户能够在应用程序中使用其自定义标识提供程序进行注册并登录。

继承自 [identityprovider.read.all](../resources/identityprovider.md)。

## <a name="methods"></a>方法

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
|clientId|字符串|使用身份提供程序注册应用时获取的应用客户端 ID。 继承自 [identityprovider.read.all](../resources/identityprovider.md)。 此属性是必需的。|
|clientSecret|字符串|使用身份提供程序注册应用时获取的应用客户端密码。 ClientSecret 对 responseType 具有依赖性。 在 responseType = code 的情况下，授权代码交换需要机密，但在 responseType = id_token 不是必需的，因为没有代码交换，而是直接从授权响应返回 id_token。这是只写的。 读取操作将返回“\*\*\*\*”。 继承自 [identityprovider.read.all](../resources/identityprovider.md)。|
|id|字符串|标识提供程序的 ID。 它是必需的属性，在创建后是只读的。|
|name|字符串|标识提供程序的显示名称。 它是必需的属性，在创建后是只读的。|
|type|字符串|标识提供程序类型。 必须是 `OpenIDConnect` 。它是必需的属性，在创建后是只读的。|
|claimsMapping|[claimsMapping](../resources/claimsmapping.md)|在 OIDC 提供程序将 ID 令牌发送回 Azure AD 之后，Azure AD 需要能够将声明从收到的令牌映射到 Azure AD 可识别和使用的声明。 此复杂类型将捕获该映射。 它是必需的属性。|
|domainHint|String|可以使用域提示直接跳到指定标识提供程序的登录页，而不是让用户在可用标识提供程序列表中进行选择。|
|metadataUrl|String|OpenID Connect 标识提供程序的元数据文档的 URL。 每个 OpenID Connect 标识提供程序都介绍了包含执行登录所需的大多数信息的元数据文档。 其中包括要使用的 Url 和服务的公共签名密钥的位置等信息。 OpenID Connect 元数据文档总是位于的终结点处。众所周知/OpenID-配置。 对于要添加的 OpenID Connect 标识提供程序，您将需要提供元数据 URL。 它是必需的属性，在创建后是只读的。|
|responseMode|String|响应模式定义应用于将数据从自定义标识提供程序发送回 Azure AD B2C 的方法。 可以使用以下响应模式： <ul><li/>`form_post` ：建议使用此响应模式以获得最佳安全性。 响应通过 HTTP POST 方法传输，其中的代码或令牌使用应用程序/x www 格式 urlencoded 格式在正文中进行编码。<li/>`query` ：代码或令牌作为查询参数返回。</ul> 它是必需的属性。|
|responseType|String|响应类型描述在对自定义标识提供程序的 authorization_endpoint 的初始调用中发送回的信息类型。 可以使用以下响应类型：<ul><li/> `code` ：按照授权代码流，代码将返回到 Azure AD B2C。 Azure AD B2C 将继续调用 token_endpoint 以交换令牌的代码。<li/> `id_token` ：从自定义标识提供程序向 Azure AD B2C 返回 ID 令牌。 <li/>`token` ：从自定义标识提供程序向 Azure AD B2C 返回访问令牌。 目前，Azure AD B2C 不支持此值 () </ul> 它是必需的属性。|
|scope|String|作用域定义要从自定义标识提供程序中收集的信息和权限。 OpenID Connect 请求必须包含 openid 作用域值，才能接收标识提供程序中的 ID 令牌。 如果没有 ID 令牌，用户将无法使用自定义标识提供程序登录 Azure AD B2C。 可以通过空格分隔其他作用域。 有关范围限制的详细信息，请参阅 [RFC6749 节 3.3](https://tools.ietf.org/html/rfc6749#section-3.3)。 它是必需的属性。|

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
