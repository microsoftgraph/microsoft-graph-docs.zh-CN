---
title: builtInIdentityProvider 资源类型
description: 表示 Azure Active Directory 租户中的内置标识提供程序。
localization_priority: Priority
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: 3abed0479d6746c1ba1c1279512317ab60445377
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/22/2021
ms.locfileid: "53534101"
---
# <a name="builtinidentityprovider-resource-type"></a>builtInIdentityProvider 资源类型
命名空间：microsoft.graph

表示具有 Azure Active Directory [租户](/azure/active-directory/external-identities/) 标识的内置标识提供程序。

对于 Azure AD 租户中的 Azure AD B2B 方案，内置标识提供程序类型可以是 Azure Active Directory （AAD）、Microsoft 帐户（MSA）或电子邮件一次密码 （EmailOTP）。

此类型继承自 [identityProviderBase](../resources/identityproviderbase.md)。

## <a name="methods"></a>方法

| 方法       | 返回类型  |Description|
|:---------------|:--------|:----------|
|[List](../api/identityproviderbase-list.md)|[identityProviderBase](../resources/identityproviderbase.md) 集合|检索租户中配置的所有标识提供程序，包括内置标识提供程序。|
|[Get](../api/identityproviderbase-get.md) |builtInIdentityProvider|检索内置标识提供程序的属性。|
|[列出可用的提供程序类型](../api/identityproviderbase-list-availableprovidertypes.md)|String 集合|检索租户中所有可用的标识提供程序类型。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---------------|:--------|:----------|
|id|String|标识提供程序的标识符。 继承自 [identityProviderBase](../resources/identityproviderbase.md)。 只读。|
|displayName|字符串|标识提供者的显示名称。继承自 [identityProviderBase](../resources/identityproviderbase.md)。|
|identityProviderType|字符串|标识提供程序类型。 对于 B2B 方案，可能的值： `AADSignup`、 `MicrosoftAccount`、 `EmailOTP`。 此为必需属性。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.builtInIdentityProvider"
} -->

```json
{
    "id": "String",
    "identityProviderType": "String",
    "displayName": "String",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2021-03-30 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
 "description": "builtinIdentityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
