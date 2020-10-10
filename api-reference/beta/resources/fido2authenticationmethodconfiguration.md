---
title: fido2AuthenticationMethodConfiguration 资源类型
description: 表示 FIDO2 身份验证方法策略
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 62aa22fa22b70235f5221bc820cee5178b55b51b
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418201"
---
# <a name="fido2authenticationmethodconfiguration-resource-type"></a>fido2AuthenticationMethodConfiguration 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 FIDO2 身份验证方法策略。 身份验证方法策略定义启用使用身份验证方法的配置设置和用户或组。


## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取](../api/fido2authenticationmethodconfiguration-get.md)|[fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md)|读取 fido2AuthenticationMethodConfiguration 对象的属性和关系。|
|[更新](../api/fido2authenticationmethodconfiguration-update.md)|[fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md)|更新 fido2AuthenticationMethodConfiguration 对象的属性。|
|[删除](../api/fido2authenticationmethodconfiguration-delete.md)|无|将 fido2AuthenticationMethodConfiguration 对象还原为其默认配置。|


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|身份验证方法策略标识符。|
|isAttestationEnforced|布尔|确定是否必须为 FIDO2 安全密钥注册强制实施证明。|
|isSelfServiceRegistrationAllowed|布尔|确定用户是否可以注册新的 FIDO2 安全密钥。|
|keyRestrictions|[fido2KeyRestrictions](../resources/fido2keyrestrictions.md)|控制是否在 FIDO2 安全密钥上强制实施密钥限制，允许或禁止使用身份验证器证明 GUID (AAGUID) 定义的某些密钥类型。一个标识符，指示 (的类型（例如，) 身份验证器的模型）。|
|state|authenticationMethodState|可取值为：`enabled`、`disabled`。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|includeTargets|[authenticationMethodTarget](../resources/authenticationmethodtarget.md) 集合|启用使用身份验证方法的用户或组的集合。|

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
