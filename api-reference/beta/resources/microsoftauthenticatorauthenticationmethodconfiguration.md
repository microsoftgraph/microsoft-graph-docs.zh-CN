---
title: microsoftAuthenticatorAuthenticationMethodConfiguration 资源类型
description: 表示 Microsoft Authenticator 身份验证方法策略。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7f2d5dbc64fe81b629f89cf0b98bd3f2d32c1411
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49874465"
---
# <a name="microsoftauthenticatorauthenticationmethodconfiguration-resource-type"></a>microsoftAuthenticatorAuthenticationMethodConfiguration 资源类型
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Microsoft Authenticator 身份验证方法策略。 身份验证方法策略定义配置设置以及已启用使用身份验证方法的用户或组。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取](../api/microsoftauthenticatorauthenticationmethodconfiguration-get.md)|[microsoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md)|读取 microsoftAuthenticatorAuthenticationMethodConfiguration 对象的属性和关系。|
|[更新](../api/microsoftauthenticatorauthenticationmethodconfiguration-update.md)|[microsoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md)|更新 microsoftAuthenticatorAuthenticationMethodConfiguration 对象的属性。|
|[删除](../api/microsoftauthenticatorauthenticationmethodconfiguration-delete.md)|无|将 microsoftAuthenticatorAuthenticationMethodConfiguration 对象还原到其默认配置。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|身份验证方法策略标识符。|
|state|authenticationMethodState|可取值为：`enabled`、`disabled`。|

## <a name="relationships"></a>关系
|关系|类型|Description|
|:---|:---|:---|
|includeTargets|[microsoftAuthenticatorAuthenticationMethodTarget](../resources/microsoftauthenticatorauthenticationmethodtarget.md) 集合|允许使用身份验证方法的用户或组的集合。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration",
  "baseType": "microsoft.graph.authenticationMethodConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String"
}
```

