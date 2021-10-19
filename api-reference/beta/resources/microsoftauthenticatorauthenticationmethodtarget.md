---
title: microsoftAuthenticatorAuthenticationMethodTarget 资源类型
description: 启用以使用身份验证方法策略Microsoft Authenticator或组的集合。
author: mmcla
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 8276f01bca86025c11eddeef21d5cce28263c379
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/19/2021
ms.locfileid: "60493478"
---
# <a name="microsoftauthenticatorauthenticationmethodtarget-resource-type"></a>microsoftAuthenticatorAuthenticationMethodTarget 资源类型
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

启用以使用 Microsoft Authenticator[身份验证方法](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md)策略的用户或组Azure AD。  继承自 [authenticationMethodTarget](authenticationMethodTarget.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|authenticationMode|microsoftAuthenticatorAuthenticationMode|确定可用于登录的通知类型。 可能的值包括 `deviceBasedPush` ： (、和) 无 `push` 密码 `any` 。|
|id|String|用户或组Azure AD标识符。 继承自 [authenticationMethodTarget](authenticationmethodtarget.md)。|
|isRegistrationRequired|Boolean|确定是否强制用户注册身份验证方法。 继承自 [authenticationMethodTarget](authenticationmethodtarget.md)。 *不支持*。 |
|targetType|authenticationMethodTargetType| 可能的值为： `user`、 `group`和 `unknownFutureValue`。 继承自 [authenticationMethodTarget](authenticationMethodTarget.md)。|
|numberMatchingRequiredState|advancedConfigState|需要匹配 MFA 通知的号码。 手机登录通知的值将被忽略。 可取值为：`enabled`、`disabled`、`default`。|
|displayAppInformationRequiredState|advancedConfigState|确定用户是否在应用通知中Authenticator上下文。 在通知Authenticator正文中，用户将显示他们登录的应用以及身份验证请求源自的位置。 可取值为：`enabled`、`disabled`、`default`。|

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
  "numberMatchingRequiredState": "String",
  "displayAppInformationRequiredState": "String"
}

```
