---
title: passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration 资源类型
description: 表示 Microsoft 验证 Passwordless 电话登录身份验证方法策略。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ddf6a66abbf745a769a44cf323ebb245c31ecf60
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418269"
---
# <a name="passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-resource-type"></a>passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Microsoft 验证 Passwordless 电话登录身份验证方法策略。 身份验证方法策略定义启用使用身份验证方法的配置设置和用户或组。

> [!NOTE]
> 在 Api 位于 Mirosoft Graph beta 过程中时，规划用于管理 Microsoft 身份验证器应用程序的 Api 的大量架构更改。 由于调用模式将发生更改，因此我们建议您不要对这些 Api 进行生产依赖。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取](../api/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-get.md)|[passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md)|读取 passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration 对象的属性和关系。|
|[更新](../api/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-update.md)|[passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md)|更新 passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration 对象的属性。|
|[删除](../api/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-delete.md)|无|将 passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration 对象还原为其默认配置。|


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|身份验证方法策略标识符。|
|state|authenticationMethodState|可取值为：`enabled`、`disabled`。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|includeTargets|[passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodtarget.md) 集合|启用使用身份验证方法的用户或组的集合。|

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
