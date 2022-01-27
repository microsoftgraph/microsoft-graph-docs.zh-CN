---
title: authenticationMethodConfigurations
description: authenticationMethodConfigurations 对象。
author: mmcla
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 8ea9d69b724be32eff0f9d6bafc4ef1bff7c33a7
ms.sourcegitcommit: de9df4bf6313b49afba74b6e9ef819907669c662
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/27/2022
ms.locfileid: "62239118"
---
# <a name="authenticationmethodconfiguration-resource-type"></a>authenticationMethodConfiguration 资源类型
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

这是一个抽象类型，表示每个身份验证方法的设置。 它可配置租户是启用还是禁用特定身份验证方法，以及哪些用户和组可以注册和使用该方法。

以下身份验证方法派生自 **authenticationMethodConfiguration** 资源类型：
+ [emailAuthenticationMethodConfiguration](emailauthenticationmethodconfiguration.md)
+ [fido2AuthenticationMethodConfiguration](fido2authenticationmethodconfiguration.md)
+ [microsoftAuthenticatorAuthenticationMethodConfiguration](microsoftauthenticatorauthenticationmethodconfiguration.md)
+ [smsAuthenticationMethodConfiguration](smsauthenticationmethodconfiguration.md)
+ [temporaryAccessPassAuthenticationMethodConfiguration](smsauthenticationmethodconfiguration.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|策略名称。|
|state|authenticationMethodState|策略的状态。 可取值为：`enabled`、`disabled`。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationMethodConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String"
}
```
