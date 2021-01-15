---
title: passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget 资源类型
description: 启用使用 Microsoft Authenticator 无密码电话登录身份验证方法策略的用户或组的集合。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ef62b251d6c943bd6290a07fa2b018bddca81ab5
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872266"
---
# <a name="passwordlessmicrosoftauthenticatorauthenticationmethodtarget-resource-type-deprecated"></a>passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget 资源类型 (已弃) 

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

已启用使用 Microsoft Authenticator 无密码电话登录身份验证方法策略的用户或组的集合] (。/resources/passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration.md) Azure AD 中。

> [!CAUTION]
> Microsoft Authenticator 无密码电话登录身份验证方法策略 API 已弃用，2020 年 12 月 31 日停止返回结果。 请使用新的 [Microsoft Authenticator 身份验证方法策略](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|Azure AD 用户或组的对象 ID。|
|isRegistrationRequired|Boolean|确定是否强制用户注册身份验证方法。|
|shownContext|authenticatorAppContextType|可取值为：`location`、`app`。|
|targetType|authenticationMethodTargetType|可取值为：`user`、`group`。|
|useForSignIn|Boolean|确定是否可以使用身份验证方法登录到 Azure AD。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget",
  "baseType": "microsoft.graph.authenticationMethodTarget",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget",
  "id": "String (identifier)",
  "targetType": "String",
  "isRegistrationRequired": "Boolean",
  "useForSignIn": "Boolean",
  "shownContext": "String"
}
```
