---
title: identityProviderBase 资源类型
description: 代表 Azure Active Directory 租户和 Azure AD B2C 租户中的身份提供程序。
ms.localizationpriority: high
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: aacf2b128e8cf60f445fb59d93e6be8d84b8deb0
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59032382"
---
# <a name="identityproviderbase-resource-type"></a>identityProviderBase 资源类型
命名空间：microsoft.graph

表示标识提供者， [Azure Active Directory （Azure AD） 和 Azure AD B2C 租户的外部标识](/azure/active-directory/external-identities/) 。 它是由 [socialIdentityProvider](../resources/socialidentityprovider.md) 继承的抽象类型， [builtinIdentityProvider](../resources/builtinidentityprovider.md)。

对于 Azure AD B2B 方案，标识提供者是 [socialIdentityProvider](../resources/socialidentityprovider.md) 或 [builtinIdentityProvider](../resources/builtinidentityprovider.md)。 通过在 Azure AD B2C 中配置身份提供程序，可实现新 Azure AD B2B 来宾方案。 例如，具有Microsoft 365资源的组织可以与 Gmail 用户共享它们。 Gmail 将使用其 Google 帐户凭据来验证和访问文档。

在Azure AD B2C目录中，标识提供者类型是 [socialIdentityProvider](../resources/socialidentityprovider.md)。 在Azure AD B2C目录中配置标识提供者使用户能够使用应用程序中的社交帐户进行注册和登录。 例如，应用程序可使用 Azure AD B2C 让用户能够通过 Facebook 帐户注册服务。

## <a name="methods"></a>方法

| 方法       | 返回类型  |Description|
|:---------------|:--------|:----------|
|[List](../api/identitycontainer-list-identityproviders.md)|[identityProviderBase](../resources/identityproviderbase.md) 集合|检索在租户中配置的所有标识提供程序。|
|[创建](../api/identitycontainer-post-identityproviders.md)|[socialIdentityProvider](../resources/socialidentityprovider.md)|创建新的 [socialIdentityProvider](../resources/socialidentityprovider.md) （Azure AD或Azure AD B2C）。|
|[获取](../api/identityproviderbase-get.md) |[socialIdentityProvider](../resources/socialidentityprovider.md) 或 [builtinIdentityProvider](../resources/builtinidentityprovider.md)|检索 [socialIdentityProvider](../resources/socialidentityprovider.md) （Azure AD 或Azure AD B2C）或 [builtinIdentityProvider](../resources/builtinidentityprovider.md) （Azure AD） 的属性。|
|[更新](../api/identityproviderbase-update.md)|无|更新 [socialIdentityProvider](../resources/socialidentityprovider.md) （Azure AD或Azure AD B2C）。|
|[删除](../api/identityproviderbase-delete.md)|无|删除 [socialIdentityProvider](../resources/socialidentityprovider.md) （Azure AD 或Azure AD B2C）。|
|[列出可用的提供程序类型](../api/identityproviderbase-availableprovidertypes.md)|String 集合|检索所有受支持的标识提供者类型。|

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
