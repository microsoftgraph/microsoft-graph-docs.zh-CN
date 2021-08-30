---
title: b2cAuthenticationMethodsPolicy资源类型
description: 表示注册给在 Azure Active Directory （Azure AD） B2C 租户中配置的用户的本地帐户身份验证方法。
ms.localizationpriority: high
author: namkedia
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: e960e3809122d70ed52369d47f6985e82dd4f70a
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/30/2021
ms.locfileid: "58694872"
---
# <a name="b2cauthenticationmethodspolicy-resource-type"></a>b2cAuthenticationMethodsPolicy资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure Active Directory （Azure AD） B2C 允许租户管理员选择让最终用户通过本地账户注册的机制。 本地帐户是指由 Azure AD 执行标识断言的帐户，而不是Google或Facebook等联合身份提供商。

Azure AD B2C 中的本地帐户未遵循来自 Azure AD 的设置或范式。 Azure ad B2C 未使用或执行 Azure AD 身份验证方法策略。 Azure AD B2C 将这些设置存储在不同的策略中，由用户流来消耗。

## <a name="methods"></a>方法

| 方法       | 返回类型 | Description |
|:-------------|:------------|:------------|
| [获取 b2cAuthenticationMethodsPolicy](../api/b2cauthenticationmethodspolicy-get.md) | [b2cauthenticationmethodspolicy](b2cauthenticationmethodspolicy.md) | 读取 **b2cauthenticationmethodspolicy** 对象的属性。 |
| [更新 b2cAuthenticationMethodsPolicy](../api/b2cauthenticationmethodspolicy-update.md) | 无 | 更新 **b2cauthenticationmethodspolicy** 对象的属性。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String|B2C认证方式策略的id。 这是一个只读属性，也是关键所在。|
|isEmailPasswordAuthenticationEnabled|布尔值|如果启用了电子邮件和密码身份验证方法，租户管理员可以使用电子邮件配置本地帐户。|
|isUserNameAuthenticationEnabled|布尔值|如果启用了用户名和密码身份验证方法，租户管理员可以使用用户名配置本地帐户。|
|isPhoneOneTimePasswordAuthenticationEnabled|布尔值|如果已启用电话号码和一次性密码身份验证方法，则租户管理员可以使用电话号码配置本地帐户。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.b2cAuthenticationMethodsPolicy",
  "keyProperty": "id"
}-->

```json
{
    "id": "b2CAuthenticationMethodsPolicy",
    "isEmailPasswordAuthenticationEnabled": true,
    "isUserNameAuthenticationEnabled": false,
    "isPhoneOneTimePasswordAuthenticationEnabled": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "b2cAuthenticationMethodsPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
