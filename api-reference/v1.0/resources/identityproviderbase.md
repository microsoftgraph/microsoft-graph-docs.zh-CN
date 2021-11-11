---
title: identityProviderBase 资源类型
description: 代表 Azure Active Directory 租户和 Azure AD B2C 租户中的身份提供程序。
ms.localizationpriority: high
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: 661c9ca5f1a76af52112d22671d02bd2c801b79f
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2021
ms.locfileid: "60890169"
---
# <a name="identityproviderbase-resource-type"></a>identityProviderBase 资源类型
命名空间：microsoft.graph

表示标识提供者， [Azure Active Directory （Azure AD） 和 Azure AD B2C 租户的外部标识](/azure/active-directory/external-identities/) 。

对于Azure AD目录中的Azure AD B2B 方案，标识提供者可以是 [socialIdentityProvider](../resources/socialidentityprovider.md) 或 [builtinIdentityProvider](../resources/builtinidentityprovider.md)，这两者都继承自 identityProviderBase 资源类型。

通过在 Azure AD B2C 中配置身份提供程序，可实现新 Azure AD B2B 来宾方案。 例如，某组织在 Microsoft 365 中具有需要与 Gmail 用户共享的资源。 Gmail 将使用其 Google 帐户凭据来验证和访问文档。

在 Azure AD B2C 目录中，标识提供者类型可以是 [socialIdentityProvider](../resources/socialidentityprovider.md) 或 [appleManagedIdentityProvider](../resources/applemanagedidentityprovider.md)，所有这些都继承自 identityProviderBase 资源类型。

在 Azure AD B2C 租户中配置身份提供程序，用户可在应用程序中使用社交帐户或自定义 OpenID Connect 支持的提供程序进行注册和登录。 例如，应用程序可使用 Azure AD B2C 让用户能够通过 Facebook 帐户或他们自己的符合 OIDC 协议的自定义身份提供程序注册服务。

## <a name="methods"></a>方法

| 方法       | 返回类型  |Description|
|:---------------|:--------|:----------|
|[List](../api/identitycontainer-list-identityproviders.md)|[identityProviderBase](../resources/identityproviderbase.md) 集合|检索在租户中配置的所有标识提供程序。|
|[创建](../api/identitycontainer-post-identityproviders.md)| [socialidentityprovider](../resources/socialidentityprovider.md) 或 [appleManagedIdentityProvider](../resources/applemanagedidentityprovider.md) |创建以下对象类型之一的新对象： <br/><ul><li> [socialidentityprovider](../resources/socialidentityprovider.md)（Azure AD或Azure AD B2C） <li> [appleManagedIdentityProvider](../resources/applemanagedidentityprovider.md)（Azure AD B2C） </li></ul>|
|[获取](../api/identityproviderbase-get.md) |[socialidentityprovider](../resources/socialidentityprovider.md)、[builtInIdentityProvider](../resources/builtinidentityprovider.md) 或 [appleManagedIdentityProvider](../resources/applemanagedidentityprovider.md)| 检索以下对象类型之一的属性： <br/><ul><li> [socialidentityprovider](../resources/socialidentityprovider.md)（Azure AD或Azure AD B2C） <li> [builtInIdentityProvider](../resources/builtinidentityprovider.md)（Azure AD或Azure AD B2C） <li> [appleManagedIdentityProvider](../resources/applemanagedidentityprovider.md)（Azure AD B2C） </li></ul>|
|[更新](../api/identityproviderbase-update.md)|无|更新以下对象类型之一： <br/><ul><li> [socialidentityprovider](../resources/socialidentityprovider.md)（Azure AD或Azure AD B2C） <li> [appleManagedIdentityProvider](../resources/applemanagedidentityprovider.md)（Azure AD B2C） </li></ul>|
|[删除](../api/identityproviderbase-delete.md)|无|删除以下对象类型之一： <br/><ul><li> [socialidentityprovider](../resources/socialidentityprovider.md)（Azure AD或Azure AD B2C） <li> [appleManagedIdentityProvider](../resources/applemanagedidentityprovider.md) （Azure AD B2C） （Azure AD B2C）|
|[列出可用的提供程序类型](../api/identityproviderbase-availableprovidertypes.md)|String 集合|检索租户中所有受支持的标识提供者类型。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---------------|:--------|:----------|
|id|String|标识提供程序的标识符。|
|displayName|字符串|标识提供程序的显示名称。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.identityProviderBase"
} -->

```json
{
    "id": "String",
    "displayName": "String"
}
```
