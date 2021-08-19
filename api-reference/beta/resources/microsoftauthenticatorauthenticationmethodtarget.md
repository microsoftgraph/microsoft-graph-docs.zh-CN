---
title: microsoftAuthenticatorAuthenticationMethodTarget 资源类型
description: 启用以使用身份验证方法策略Microsoft Authenticator组的集合。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 4baf2713789a54707c65fe8c2b94fe60ac275626
ms.sourcegitcommit: b7e01a1331abe5f5c9aa2828d93dad08229573f1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58336668"
---
# <a name="microsoftauthenticatorauthenticationmethodtarget-resource-type"></a>microsoftAuthenticatorAuthenticationMethodTarget 资源类型
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 Azure AD 中启用以使用 Microsoft Authenticator[方法策略的用户](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md)或组的集合。  继承自 [authenticationMethodTarget](authenticationMethodTarget.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|authenticationMode|microsoftAuthenticatorAuthenticationMode|确定可用于登录的通知类型。 可能的值包括 `deviceBasedPush` ： (、和) 无 `push` 密码 `any` 。|
|featureSettings|authenticatorAppFeatureSettings|确定应应用于其他设置Microsoft Authenticator。 可能的值是 `requireNumberMatching` ： (MFA 通知需要匹配号码。 对于手机登录通知，此值将被忽略) 。 可为 NULL。|
|id|String|Azure AD 用户或组的对象标识符。 继承自 [authenticationMethodTarget](authenticationmethodtarget.md)。|
|isRegistrationRequired|布尔值|确定是否强制用户注册身份验证方法。 继承自 [authenticationMethodTarget](authenticationmethodtarget.md)。 *不支持*。 |
|targetType|authenticationMethodTargetType| 可能的值为： `user`、 `group`和 `unknownFutureValue`。 继承自 [authenticationMethodTarget](authenticationMethodTarget.md)。|
<!--
|numberMatchingRequiredState|advancedConfigState|Requires number matching for MFA notifications. Value is ignored for phone sign-in notifications. Possible values are: `enabled`, `disabled`, `default`.|
|displayLocationInformationRequiredState|advancedConfigState|Determines whether the location of the sign-in should be shown to the user in the body of the notification. Possible values are: `enabled`, `disabled`, `default`.|
|displayAppInformationRequiredState|advancedConfigState|Determines whether the app the user is signing into should be shown to the user in the body of the notification. Possible values are: `enabled`, `disabled`, `default`.|
-->

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftAuthenticatorAuthenticationMethodTarget",
  "baseType": "microsoft.graph.authenticationMethodTarget",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftAuthenticatorAuthenticationMethodTarget",
  "targetType": "String",
  "id": "String (identifier)",
  "isRegistrationRequired": "Boolean",
  "authenticationMode": "String",
  "featureSettings": "String"
}

```
