---
title: fido2AuthenticationMethodConfiguration 资源类型
description: 表示 FIDO2 身份验证方法策略
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7684b8b2c6601b4afdad25b3d3c32b7a6b68667d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964684"
---
# <a name="fido2authenticationmethodconfiguration-resource-type"></a>fido2AuthenticationMethodConfiguration 资源类型

命名空间：microsoft.graph

表示 FIDO2 身份验证方法策略。 身份验证方法策略定义配置设置以及能够使用身份验证方法的用户或组。


## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[获取](../api/fido2authenticationmethodconfiguration-get.md)|[fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md)|读取 fido2AuthenticationMethodConfiguration 对象的属性和关系。|
|[更新](../api/fido2authenticationmethodconfiguration-update.md)|[fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md)|更新 fido2AuthenticationMethodConfiguration 对象的属性。|
|[删除](../api/fido2authenticationmethodconfiguration-delete.md)|无|将 fido2AuthenticationMethodConfiguration 对象还原到其默认配置。|


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|身份验证方法策略标识符。|
|isAttestationEnforced|Boolean|确定是否必须对 FIDO2 安全密钥注册强制执行证明。|
|isSelfServiceRegistrationAllowed|Boolean|确定用户能否注册新的 FIDO2 安全密钥。|
|keyRestrictions|[fido2KeyRestrictions](../resources/fido2keyrestrictions.md)|控制是否对 FIDO2 安全密钥实施密钥限制，允许或禁止验证器证明 GUID (AAGUID) 定义的某些密钥类型，即指示验证器的类型 (例如验证器的 make 和 model) 。|
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
