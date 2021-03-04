---
title: fido2AuthenticationMethodConfiguration 资源类型
description: 代表 FIDO2 身份验证方法策略
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: b5d823caefba62a66fc9b2a7236c063cfaeee69b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440316"
---
# <a name="fido2authenticationmethodconfiguration-resource-type"></a>fido2AuthenticationMethodConfiguration 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 FIDO2 身份验证方法策略。 身份验证方法策略定义配置设置以及允许使用身份验证方法的用户或组。


## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[获取](../api/fido2authenticationmethodconfiguration-get.md)|[fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md)|读取 fido2AuthenticationMethodConfiguration 对象的属性和关系。|
|[更新](../api/fido2authenticationmethodconfiguration-update.md)|[fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md)|更新 fido2AuthenticationMethodConfiguration 对象的属性。|
|[删除](../api/fido2authenticationmethodconfiguration-delete.md)|无|将 fido2AuthenticationMethodConfiguration 对象恢复为其默认配置。|


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|身份验证方法策略标识符。|
|isAttestationEnforced|布尔|确定是否必须对 FIDO2 安全密钥注册强制执行证明。|
|isSelfServiceRegistrationAllowed|布尔|确定用户能否注册新的 FIDO2 安全密钥。|
|keyRestrictions|[fido2KeyRestrictions](../resources/fido2keyrestrictions.md)|控制是否对 FIDO2 安全密钥强制执行密钥限制，允许或禁止验证器证明 GUID (AAGUID) 定义的某些密钥类型，AAGUID) 是指示类型 (的标识符，例如验证器的制作和型号) 。|
|state|authenticationMethodState|可取值为：`enabled`、`disabled`。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|includeTargets|[authenticationMethodTarget](../resources/authenticationmethodtarget.md) 集合|允许使用身份验证方法的用户或组的集合。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.fido2AuthenticationMethodConfiguration",
  "baseType": "microsoft.graph.authenticationMethodConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.fido2AuthenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String",
  "isSelfServiceRegistrationAllowed": "Boolean",
  "isAttestationEnforced": "Boolean",
  "keyRestrictions": {
    "@odata.type": "microsoft.graph.fido2KeyRestrictions"
  },
  "includeTargets": [ { "@odata.type": "microsoft.graph.authenticationMethodTarget" } ]
}
```
