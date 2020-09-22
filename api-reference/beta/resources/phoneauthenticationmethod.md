---
title: phoneAuthenticationMethod 资源类型
description: 向用户注册的电话的表示形式。
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 93bf64756d0da1e4199fdede55990e695f434480
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997835"
---
# <a name="phoneauthenticationmethod-resource-type"></a>phoneAuthenticationMethod 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

向用户注册的电话的表示形式。 此资源包括电话号码、电话类型以及电话是否配置为用户通过 SMS 登录。

电话具有以下三种类型之一：移动、备用移动或办公室。 用户可以为每种类型注册一个号码，并且在添加备用移动电话之前，必须有一个移动电话。 将电话用于多重身份验证 (MFA) 或自助服务密码重置 (SSPR) 中，移动电话是默认设置，备用移动电话是备份。 

移动电话可用于短信和语音呼叫，具体取决于租户设置。

办公室电话只能接收语音呼叫，不能接收短信消息。

SMS 登录状态属性提供有关电话号码是否已准备好通过短信登录的信息。 以下是可能的值。

|值|说明|
|--------|-----------|
|`notSupported`|此身份验证方法上不支持主登录-例如，只能在用户的主移动电话号码（而不是备用号码）上启用登录。|
|`notAllowedByPolicy`|此用户未通过策略启用以将此方法用作主要登录。|
|`notConfigured`|此用户由策略启用，以将此方法用作主要登录，但需要执行其他操作以进行配置。|
|`phoneNumberNotUnique`|此用户尝试将电话号码设置为主登录名，但该号码不是唯一的，并且不能用作登录名。|
|`ready`|此身份验证方法已准备就绪，可在主登录中使用。|

## <a name="methods"></a>方法

| 方法       | 返回类型 | Description |
|:-------------|:------------|:------------|
| [List](../api/Authentication-list-phonemethods.md) | [phoneAuthenticationMethod](phoneauthenticationmethod.md) | 读取此用户的所有 phoneAuthenticationMethod 对象的属性和关系。 |
| [获取](../api/phoneauthenticationmethod-get.md) | [phoneAuthenticationMethod](phoneauthenticationmethod.md) | 读取 phoneAuthenticationMethod 对象的属性和关系。 |
| [更新](../api/phoneauthenticationmethod-update.md) | [phoneAuthenticationMethod](phoneauthenticationmethod.md) | 更新 phoneAuthenticationMethod 对象。 |
| [删除](../api/phoneauthenticationmethod-delete.md) | 无 | 删除 phoneAuthenticationMethod 对象。 |
|[禁用短信登录](../api/phoneauthenticationmethod-disablesmssignin.md)|无|为用户关闭 SMS 登录。|
|[启用 SMS 登录](../api/phoneauthenticationmethod-enablesmssignin.md)|无|为用户启用 SMS 登录。|

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String| 注册到此用户的此电话的标识符。 只读。|
|phoneNumber|String|将电话号码设为文本或呼叫以进行身份验证。 电话号码使用格式 "+ \<country code\> \<number\> x \<extension\> "，扩展名为可选。 例如，+ 1 5555551234 或 + 1 5555551234x123 是有效的。 如果创建/更新时编号不符合要求的格式，则会拒绝编号。 |
|phoneType|字符串|此电话的类型。 可能的值包括： `mobile` 、 `alternateMobile` 或 `office` 。|
|smsSignInState|字符串|电话是否已准备好用于短信登录。 可能的值包括： `notSupported` 、、、、 `notAllowedByPolicy` `notEnabled` `phoneNumberNotUnique` `ready` 或 `notConfigured` 。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.phoneAuthenticationMethod",
  "baseType": "",
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


