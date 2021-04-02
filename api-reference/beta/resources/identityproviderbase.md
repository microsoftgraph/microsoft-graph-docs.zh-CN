---
title: identityProviderBase 资源类型
description: 代表 Azure Active Directory 租户和 Azure AD B2C 租户中的身份提供程序。
localization_priority: Priority
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: 1a3d26697c26b803bcbac9141d7ff011575f91f7
ms.sourcegitcommit: c7776e5659c391e7c9ce1cd46e242a5ddc38dba2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/01/2021
ms.locfileid: "51491104"
---
# <a name="identityproviderbase-resource-type"></a>identityProviderBase 资源类型
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

对 Azure Active Directory 租户和 Azure AD B2C 租户都标识具有[外部标识](/azure/active-directory/external-identities/)的身份提供程序。

对于 Azure AD 目录中的 Azure AD B2B 方案，标识提供程序可以是 [socialIdentityProvider](../resources/socialidentityprovider.md) 或 [builtinIdentityProvider](../resources/builtinidentityprovider.md)，它将从 identityProviderBase 资源类型继承。

通过在 Azure AD B2C 中配置身份提供程序，可实现新 Azure AD B2B 来宾方案。 例如，某组织在 Microsoft 365 中具有需要与 Gmail 用户共享的资源。 Gmail 将使用其 Google 帐户凭据来验证和访问文档。

在 Azure AD B2C 目录中，标识提供程序类型可以是 [socialIdentityProviders](../resources/socialidentityprovider.md)、 [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) 或 [appleIdentityProvider](../resources/appleidentityprovider.md)，它继承身份ProviderBase 资源类型。

在 Azure AD B2C 租户中配置身份提供程序，用户可在应用程序中使用社交帐户或自定义 OpenID Connect 支持的提供程序进行注册和登录。 例如，应用程序可使用 Azure AD B2C 让用户能够通过 Facebook 帐户或他们自己的符合 OIDC 协议的自定义身份提供程序注册服务。

## <a name="methods"></a>方法

| 方法       | 返回类型  |Description|
|:---------------|:--------|:----------|
|[List](../api/identityproviderbase-list.md)|identityProviderBase 集合|检索在租户中配置的所有标识提供程序。|
|[列出可用的提供程序类型](../api/identityproviderbase-list-availableprovidertypes.md)|String 集合|检索租户中所有可用的标识提供程序类型。|

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
    "displayName": "String",
}
```
