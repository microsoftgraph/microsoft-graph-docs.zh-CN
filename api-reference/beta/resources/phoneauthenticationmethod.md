---
title: phoneAuthenticationMethod 资源类型
description: 注册到用户的电话的表示形式。
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 0cab7a96923f49c77e6d160d68e8746530f8dcf2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964546"
---
# <a name="phoneauthenticationmethod-resource-type"></a>phoneAuthenticationMethod 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

注册到用户的电话的表示形式。 此资源包括电话号码、电话类型，以及是否将电话配置为允许用户通过短信登录。

电话有三种类型之一：移动、备用移动或办公室。 用户可以为每种类型注册一个号码，并且必须拥有移动电话才能添加备用移动电话。 当使用手机进行多重身份验证 (MFA) 或自助服务密码重置 (SSPR) 时，移动电话为默认值，备用移动电话为备份。 

移动电话可用于短信和语音呼叫，具体取决于租户设置。

Office 电话只能接收语音呼叫，不能接收短信。

## <a name="methods"></a>Methods

| 方法       | 返回类型 | Description |
|:-------------|:------------|:------------|
| [List](../api/Authentication-list-phonemethods.md) | [phoneAuthenticationMethod](phoneauthenticationmethod.md) | 读取此用户的所有 phoneAuthenticationMethod 对象的属性和关系。 |
| [获取](../api/phoneauthenticationmethod-get.md) | [phoneAuthenticationMethod](phoneauthenticationmethod.md) | 读取 phoneAuthenticationMethod 对象的属性和关系。 |
| [更新](../api/phoneauthenticationmethod-update.md) | [phoneAuthenticationMethod](phoneauthenticationmethod.md) | 更新 phoneAuthenticationMethod 对象。 |
| [删除](../api/phoneauthenticationmethod-delete.md) | 无 | 删除 phoneAuthenticationMethod 对象。 |
|[禁用短信登录](../api/phoneauthenticationmethod-disablesmssignin.md)|无|关闭用户的短信登录。|
|[启用短信登录](../api/phoneauthenticationmethod-enablesmssignin.md)|无|为用户启用短信登录。|

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String| 注册到此用户的此电话的标识符。 只读。 <br/><br/>id 的值是下列值之一：<ul><li>`b6332ec1-7057-4abe-9331-3d72feddfe41` - 其中 **phoneType** 为 `alternateMobile` 。</li><li>`e37fc753-ff3b-4958-9484-eaa9425c82bc` - 其中 **phoneType** 为 `office` 。</li><li>`3179e48a-750b-4051-897c-87b9720928f7` - 其中 **phoneType** 为 `mobile` 。</li>|
|phoneNumber|String|要发送文本或呼叫进行身份验证的电话号码。 电话号码使用格式"+ \<country code\> \<number\> \<extension\> x"，分机号可选。 例如，+1 5555551234 或 +1 5555551234x123 有效。 如果数字与所需格式不匹配，则创建/更新时将拒绝数字。 |
|phoneType|authenticationPhoneType|此电话的类型。 可能的值为： `mobile`、 `alternateMobile`或 `office`。|
|smsSignInState|authenticationMethodSignInState|电话是否可用于短信登录。 可能的值是 `notSupported` `notAllowedByPolicy` `notEnabled` ：、、、、 `phoneNumberNotUnique` `ready` 或 `notConfigured` `unknownFutureValue` 。|

### <a name="smssigninstate-values"></a>smsSignInState 值

SMS 登录状态属性提供有关电话号码是否已准备好通过短信登录的信息。 以下是可能的值。

|值|说明|
|--------|-----------|
|notSupported|此身份验证方法不支持主登录 - 例如，只能对用户的主移动电话号码（而非备用号码）启用登录。|
|notAllowedByPolicy|策略不启用此用户以将此方法用作主登录。|
|notConfigured|策略启用此用户以将此方法用作主登录，但需要执行其他操作来配置它。|
|phoneNumberNotUnique|此用户尝试将电话号码设置为主登录，但该号码不是唯一的，不能用作登录名。|
|ready|此身份验证方法已做好在主登录中的使用准备。|
|notEnabled|此登录方法未启用|

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


