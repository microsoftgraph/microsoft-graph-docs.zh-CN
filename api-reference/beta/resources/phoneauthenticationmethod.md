---
title: phoneAuthenticationMethod 资源类型
description: 向用户注册的电话的表示形式。
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 2d0ec89e21ff6ab7aa39b05acabd81c2b22bd54f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442899"
---
# <a name="phoneauthenticationmethod-resource-type"></a>phoneAuthenticationMethod 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

向用户注册的电话的表示形式。 此资源包括电话号码、电话类型，以及是否将电话配置为用户通过短信登录。

电话有三种类型之一：移动、备用移动或办公室。 用户可以为每种类型注册一个号码，并且必须拥有移动电话，然后才能添加备用移动电话。 使用电话进行多重身份验证 (MFA) 或自助服务密码重置 (SSPR) 时，移动电话为默认值，备用移动电话为备份。 

移动电话可用于短信和语音呼叫，具体取决于租户设置。

Office 电话只能接收语音呼叫，不能接收短信。

SMS 登录状态属性提供有关电话号码是否已准备好通过短信登录的信息。 以下是可能的值。

|值|说明|
|--------|-----------|
|`notSupported`|此身份验证方法不支持主登录 -例如，只能对用户的主移动号码（而非备用号码）启用登录。|
|`notAllowedByPolicy`|策略不启用此用户以将此方法用作主登录。|
|`notConfigured`|策略使此用户能够使用此方法作为主登录，但需要执行其他操作来配置它。|
|`phoneNumberNotUnique`|此用户尝试将电话号码设置为主登录，但该号码不是唯一的，不能用作登录名。|
|`ready`|此身份验证方法可供主登录使用。|

## <a name="methods"></a>Methods

| 方法       | 返回类型 | Description |
|:-------------|:------------|:------------|
| [List](../api/Authentication-list-phonemethods.md) | [phoneAuthenticationMethod](phoneauthenticationmethod.md) | 读取该用户的所有 phoneAuthenticationMethod 对象的属性和关系。 |
| [获取](../api/phoneauthenticationmethod-get.md) | [phoneAuthenticationMethod](phoneauthenticationmethod.md) | 读取 phoneAuthenticationMethod 对象的属性和关系。 |
| [更新](../api/phoneauthenticationmethod-update.md) | [phoneAuthenticationMethod](phoneauthenticationmethod.md) | 更新 phoneAuthenticationMethod 对象。 |
| [删除](../api/phoneauthenticationmethod-delete.md) | 无 | 删除 phoneAuthenticationMethod 对象。 |
|[禁用短信登录](../api/phoneauthenticationmethod-disablesmssignin.md)|无|关闭用户的短信登录。|
|[启用短信登录](../api/phoneauthenticationmethod-enablesmssignin.md)|无|为用户启用短信登录。|

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String| 注册到此用户的此电话的标识符。 只读。|
|phoneNumber|String|发短信或呼叫进行身份验证的电话号码。 电话号码使用格式"+ \<country code\> \<number\> \<extension\> x"，分机是可选的。 例如，+1 5555551234 或 +1 5555551234x123 有效。 如果数字与所需格式不匹配，则创建/更新时将拒绝这些号码。 |
|phoneType|string|此电话的类型。 可能的值为： `mobile`、 `alternateMobile`或 `office`。|
|smsSignInState|string|电话是否已准备好用于短信登录。 可能的值是： `notSupported` `notAllowedByPolicy` 、 、 、 `notEnabled` 或 `phoneNumberNotUnique` `ready` `notConfigured` 。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.phoneAuthenticationMethod",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "phoneNumber": "String",
  "phoneType": "string",
  "smsSignInState": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "phoneAuthenticationMethod resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


