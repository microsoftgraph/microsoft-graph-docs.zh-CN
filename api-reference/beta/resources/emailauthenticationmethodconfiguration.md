---
title: emailAuthenticationMethodConfiguration 资源类型
description: 代表电子邮件 OTP 身份验证方法策略
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 73b620a3fd5bea62aa927722a7dac7ce3d5a9fab
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440358"
---
# <a name="emailauthenticationmethodconfiguration-resource-type"></a>emailAuthenticationMethodConfiguration 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示此租户的电子邮件 OTP 身份验证方法策略。 身份验证方法策略定义配置设置以及允许使用身份验证方法的用户或组。 在某些情况下，租户的云本机用户可能会使用电子邮件 OTP 进行自助服务密码重置，或由外部用户用于身份验证。

## <a name="methods"></a>Methods

|方法|返回类型|说明|
|:---|:---|:---|
|[获取 emailAuthenticationMethodConfiguration](../api/emailauthenticationmethodconfiguration-get.md)|[emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md)|读取 emailAuthenticationMethodConfiguration 对象的属性和关系。|
|[更新 emailAuthenticationMethodConfiguration](../api/emailauthenticationmethodconfiguration-update.md)|[emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md)|更新 emailAuthenticationMethodConfiguration 对象的属性。|
|[删除 emailAuthenticationMethodConfiguration](../api/emailauthenticationmethodconfiguration-delete.md)|无|删除 emailAuthenticationMethodConfiguration 对象。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|id|String|身份验证方法策略标识符。 继承自 [authenticationMethodConfiguration](../resources/authenticationmethodconfiguration.md)。|
|state|authenticationMethodState|指示是否启用此身份验证方法。 可取值为：`enabled`、`disabled`。|
|allowExternalIdToUseEmailOtp|externalEmailOtpState|确定外部用户是否可以使用电子邮件 OTP 进行身份验证。 可取值为：`default`、`enabled`、`disabled`、`unknownFutureValue`。 从 2021 年 3 月开始，不使用公共预览的州中的租户将自动启用电子邮件 `default` OTP。|

## <a name="relationships"></a>关系

|关系|类型|说明|
|:---|:---|:---|
|includeTargets|[authenticationMethodTarget](../resources/authenticationmethodtarget.md) 集合|允许使用身份验证方法的用户或组的集合。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.emailAuthenticationMethodConfiguration",
  "baseType": "microsoft.graph.authenticationMethodConfiguration",
  "openType": false
}
-->

```json
{
  "@odata.type": "#microsoft.graph.emailAuthenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String",
  "allowExternalIdToUseEmailOtp": "String",
  "includeTargets": [ { "@odata.type": "microsoft.graph.authenticationMethodTarget" } ]
}
```
