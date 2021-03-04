---
title: passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration 资源类型
description: 代表 Microsoft Authenticator 无密码电话登录身份验证方法策略。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 054a8c01e0a8ccb1523622fe5df20e8e60831f60
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444061"
---
# <a name="passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-resource-type-deprecated"></a>passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration 资源类型 (已弃) 

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表 Microsoft Authenticator 无密码电话登录身份验证方法策略。 身份验证方法策略定义配置设置以及启用使用身份验证方法的用户或组。

> [!CAUTION]
> Microsoft Authenticator 无密码电话登录身份验证方法策略 API 已弃用，并停止在 2020 年 12 月 31 日返回结果。 请使用新的 [Microsoft Authenticator 身份验证方法策略](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md)。


## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[获取](../api/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-get.md) (弃) |[passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md)|读取无密码MicrosoftAuthenticatorAuthenticationMethodConfiguration 对象的属性和关系。|
|[更新](../api/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-update.md) (弃用)  |[passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md)|更新无密码MicrosoftAuthenticatorAuthenticationMethodConfiguration 对象的属性。|
|[删除](../api/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-delete.md) (弃) |无|将 passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration 对象恢复为其默认配置。|


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|身份验证方法策略标识符。|
|state|authenticationMethodState|可取值为：`enabled`、`disabled`。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|includeTargets|[passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodtarget.md) 集合|允许使用身份验证方法的用户或组的集合。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration",
  "baseType": "microsoft.graph.authenticationMethodConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String",
  "includeTargets": [ { "@odata.type": "microsoft.graph.authenticationMethodTarget" } ]
}
```
