---
title: microsoftAuthenticatorAuthenticationMethodTarget 资源类型
description: 启用以使用身份验证方法策略Microsoft Authenticator组的集合。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: db534dfb13e288b82b49005b2b1a923b8bfd5112
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896639"
---
# <a name="microsoftauthenticatorauthenticationmethodtarget-resource-type"></a>microsoftAuthenticatorAuthenticationMethodTarget 资源类型
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 Azure AD 中启用以使用Microsoft Authenticator[方法策略的用户](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md)或组的集合。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|Azure AD 用户或组的对象 ID。|
|authenticationMode|microsoftAuthenticatorAuthenticationMode|确定可用于登录的通知类型。 可能的值是 `any` `deviceBasedPush` ：、 (无密码) 、 `push` 。|
|isRegistrationRequired|Boolean|确定是否强制用户注册身份验证方法。 *不支持*。 |
|numberMatchingRequiredState|advancedConfigState|需要匹配 MFA 通知的号码。 手机登录通知的值将被忽略。 可取值为：`enabled`、`disabled`、`default`。|
|displayLocationInformationRequiredState|advancedConfigState|确定是否应在通知正文中向用户显示登录的位置。 可取值为：`enabled`、`disabled`、`default`。|
|displayAppInformationRequiredState|advancedConfigState|确定是否应在通知正文中向用户显示用户登录的应用。 可取值为：`enabled`、`disabled`、`default`。|
|targetType|authenticationMethodTargetType| 可取值为：`null`、`user`、`group`。|

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
  "displayLocationInformationRequiredState": "String",
  "displayAppInformationRequiredState": "String"
}

```
