---
title: identityProvider 资源类型
description: 代表 Azure Active Directory 租户和  Azure AD B2C 租户中的身份提供程序。
localization_priority: Priority
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: 11c793a01cd1b0027e12cd831984dc30cd04961c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945660"
---
# <a name="identityprovider-resource-type"></a>identityProvider 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

对 Azure Active Directory 租户和 Azure AD B2C 租户都标识具有[外部标识](/azure/active-directory/external-identities/)的身份提供程序。

对于 Azure AD 租户中的 Azure AD B2B 方案，身份提供程序类型可以是 Google 或 Facebook。

通过在 Azure AD B2C 中配置身份提供程序，可实现新 Azure AD B2B 来宾方案。 例如，某组织在 Microsoft 365 中具有需要与 Gmail 用户共享的资源。 Gmail 将使用其 Google 帐户凭据来验证和访问文档。

在 Azure AD B2C 租户中，标识提供程序类型可以是 **Microsoft**、 **Google**、 **Facebook**、 **Amazon**、 **LinkedIn**、 **Twitter** 或任何 [openIdConnectProvider](../resources/openidconnectprovider.md)。 以下标识提供者为预览版： **微博**、 **QQ**、 **We用户** 和 **GitHub**。

在 Azure AD B2C 租户中配置身份提供程序，用户可在应用程序中使用社交帐户或自定义 OpenID Connect 支持的提供程序进行注册和登录。 例如，应用程序可使用 Azure AD B2C 让用户能够通过 Facebook 帐户或他们自己的符合 OIDC 协议的自定义身份提供程序注册服务。


如果是具有 `OpenIDConnect` 且为 `type` 的自定义 OpenID Connect 身份提供程序， 则使用 [openIdConnectProvider](../resources/openidconnectprovider.md) 资源类型表示，该资源类型将继承自身份提供程序资源类型。 

## <a name="methods"></a>方法

| 方法       | 返回类型  |Description|
|:---------------|:--------|:----------|
|[List](../api/identityprovider-list.md)|identityProvider 集合|检索在租户中配置的所有标识提供程序。|
|[创建](../api/identityprovider-post-identityproviders.md)|identityProvider|新建身份提供程序。|
|[获取](../api/identityprovider-get.md) |identityProvider|检索身份提供程序的属性。|
|[更新](../api/identityprovider-update.md)|无|更新身份提供程序。|
|[删除](../api/identityprovider-delete.md)|无|删除身份提供程序。|
|[列出可用的提供程序类型](../api/identityprovider-list-availableprovidertypes.md)|String 集合|检索所有可用的身份提供程序类型。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---------------|:--------|:----------|
|clientId|字符串|使用身份提供程序注册应用时获取的应用客户端 ID。 这是必填字段。  必填。 不可为空。|
|clientSecret|字符串|使用身份提供程序注册应用时获取的应用客户端密码。 这是只读的。 读取操作将返回 `****`。 这是必填字段。 必填。 不可为空。|
|id|字符串|标识提供程序的 ID。|
|name|字符串|标识提供程序的显示名称。 不可为空。|
|type|字符串|身份提供程序类型是必填字段。 对于 B2B 方案： `Google`， `Facebook`。 对于 B2C 方案： `Microsoft`、 `Google`、 `Amazon`、 `LinkedIn`、 `Facebook`、 `GitHub`、 `Twitter`、 `Weibo`、`QQ`、 `WeChat`、 `OpenIDConnect`。 不可为空。|

### <a name="where-to-get-the-client-id-and-secret"></a>获取客户端 ID 和密码的位置

每个标识提供程序都有一个用于创建应用注册的进程。 例如，用户在 [developers.facebook.com](https://developers.facebook.com/) 处向 Facebook 创建一个应用注册。 生成的客户端 ID 和客户端密码可传递用于[创建 identityProvider](../api/identityprovider-post-identityproviders.md)。 然后，目录中的每个用户对象都可联合到租户的任意标识提供程序中进行身份验证。 这样，用户即可通过在标识提供程序的登录页面上输入评估凭据来进行登录。 来自标识提供程序的令牌先由 Azure AD 进行验证，然后租户再向应用程序发出一个令牌。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.identityProvider"
} -->

```json
{
    "id": "String",
    "type": "String",
    "name": "String",
    "clientId": "String",
    "clientSecret": "String"
}
```
