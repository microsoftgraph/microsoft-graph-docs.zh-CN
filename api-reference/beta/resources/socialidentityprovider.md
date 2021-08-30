---
title: socialIdentityProvider 资源类型
description: 代表 Azure Active Directory 租户和 Azure AD B2C 租户中的社交标识提供程序。
ms.localizationpriority: high
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: ef47509cf1ca212d7e2e7dda9f76a1352037ba7b
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/30/2021
ms.locfileid: "58696972"
---
# <a name="socialidentityprovider-resource-type"></a>socialIdentityProvider 资源类型
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示具有Azure Active Directory （Azure AD） 和 Azure AD B2C 租户的 [外部标识](/azure/active-directory/external-identities/) 的社交标识提供者。

继承自 [identityProviderBase](../resources/identityproviderbase.md)。

对于 Azure AD 租户中的 Azure AD B2B 方案，身份提供程序类型可以是 Google 或 Facebook。

通过在 Azure AD B2C 中配置身份提供程序，可实现新 Azure AD B2B 来宾方案。 例如，某组织在 Microsoft 365 中具有需要与 Gmail 用户共享的资源。 Gmail 将使用其 Google 帐户凭据来验证和访问文档。

在 Azure AD B2C 租户中，标识提供程序类型可以是 Microsoft、Google、Facebook、Amazon、LinkedIn或 Twitter。 以下身份提供程序正处于预览阶段：微博、QQ、微信和 GitHub。

在 Azure AD B2C 租户中配置标识提供程序使用户可以在应用程序中使用支持的社交帐户提供程序进行注册和登录。 例如，应用程序可使用 Azure AD B2C 让用户能够通过 Facebook 帐户注册服务。

## <a name="methods"></a>方法

| 方法       | 返回类型  |Description|
|:---------------|:--------|:----------|
|[List](../api/identitycontainer-list-identityproviders.md)|[identityProviderBase](../resources/identityproviderbase.md) 集合|检索租户中配置的所有标识提供程序，包括 [socialIdentityProvider](../resources/socialidentityprovider.md) 对象类型。 无法仅检索租户中的社交标识提供者。|
|[Create](../api/identitycontainer-post-identityproviders.md)|socialidentityprovider |创建新的[socialIdentityProvider](../resources/socialidentityprovider.md) 对象。|
|[Get](../api/identityproviderbase-get.md) |socialidentityprovider |检索 [socialIdentityProvider](../resources/socialidentityprovider.md) 对象的属性。|
|[更新](../api/identityproviderbase-update.md)|无|更新[socialIdentityProvider](../resources/socialidentityprovider.md) 对象。|
|[删除](../api/identityproviderbase-delete.md)|无|删除[socialIdentityProvider](../resources/socialidentityprovider.md) 对象。|
|[列出可用的提供程序类型](../api/identityproviderbase-availableprovidertypes.md)|String 集合|检索租户中所有可用的标识提供程序类型。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---------------|:--------|:----------|
|clientId|字符串|向标识提供程序注册应用程序时获取的应用程序的客户端标识符。必需。|
|clientSecret|字符串|向标识提供程序注册时获取的应用程序的客户端密码。 这是只读的。 读取操作返回 `****`。 必需。|
|id|String|标识提供程序的标识符。继承自 [identityProviderBase](../resources/identityproviderbase.md)。只读。|
|displayName|字符串|标识提供者的显示名称。继承自 [identityProviderBase](../resources/identityproviderbase.md)。|
|identityProviderType|String|对于 B2B 方案，可能的值为： `Google`、 `Facebook`。 对于 B2C 方案，可能的值： `Microsoft`、 `Google`、 `Amazon`、 `LinkedIn`、 `Facebook`、 `GitHub`、 `Twitter`、 `Weibo`、 `QQ`、 `WeChat`。 必填。|

### <a name="where-to-get-the-client-identifier-and-secret"></a>在何处获取客户端标识符和密码

每个标识提供程序都有一个用于创建应用注册的进程。 例如，用户在 [developers.facebook.com](https://developers.facebook.com/) 处向 Facebook 创建一个应用注册。 生成的客户端 ID 和客户端密码可传递用于[创建 identityProvider](../api/identitycontainer-post-identityproviders.md)。 然后，目录中的每个用户对象都可联合到租户的任意标识提供程序中进行身份验证。 这样，用户即可通过在标识提供程序的登录页面上输入评估凭据来进行登录。 来自标识提供程序的令牌先由 Azure AD 进行验证，然后租户再向应用程序发出一个令牌。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.socialIdentityProvider"
} -->

```json
{
    "id": "String",
    "identityProviderType": "String",
    "displayName": "String",
    "clientId": "String",
    "clientSecret": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
 "description": "socialIdentityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
