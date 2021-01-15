---
title: passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration 资源类型
description: 代表 Microsoft Authenticator 无密码电话登录身份验证方法策略。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e27424264293d87775937c7893546ec321728b4a
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872280"
---
# <a name="passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-resource-type-deprecated"></a>passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration 资源类型 (已弃) 

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表 Microsoft Authenticator 无密码电话登录身份验证方法策略。 身份验证方法策略定义配置设置以及已启用使用身份验证方法的用户或组。

> [!CAUTION]
> Microsoft Authenticator 无密码电话登录身份验证方法策略 API 已弃用，2020 年 12 月 31 日停止返回结果。 请使用新的 [Microsoft Authenticator 身份验证方法策略](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md)。


## <a name="methods"></a>方法
|方法|返回类型|Description|
|:---|:---|:---|
|[获取](../api/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-get.md) (弃) |[passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md)|读取无密码MicrosoftAuthenticatorAuthenticationMethodConfiguration 对象的属性和关系。|
|[更新](../api/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-update.md) (弃用)  |[passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md)|更新无密码MicrosoftAuthenticatorAuthenticationMethodConfiguration 对象的属性。|
|[删除](../api/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-delete.md) (已弃) |无|将无密码MicrosoftAuthenticatorAuthenticationMethodConfiguration 对象还原到其默认配置。|


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|身份验证方法策略标识符。|
|state|authenticationMethodState|可取值为：`enabled`、`disabled`。|

## <a name="relationships"></a>关系
|关系|类型|Description|
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
