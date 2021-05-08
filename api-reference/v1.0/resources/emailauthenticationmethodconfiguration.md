---
title: emailAuthenticationMethodConfiguration 资源类型
description: 代表电子邮件 OTP 身份验证方法策略
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 06b7159cd14df1ee5826f4d11275e44f7819008a
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231820"
---
# <a name="emailauthenticationmethodconfiguration-resource-type"></a>emailAuthenticationMethodConfiguration 资源类型

命名空间：microsoft.graph

表示此租户的电子邮件 OTP 身份验证方法策略。 身份验证方法策略定义配置设置以及能够使用身份验证方法的用户或组。 租户的云本机用户可能会使用电子邮件 OTP 进行自助服务密码重置，或者外部用户在邀请兑换和自助注册用户流中的特定应用期间进行身份验证。

## <a name="methods"></a>方法

|方法|返回类型|说明|
|:---|:---|:---|
|[获取 emailAuthenticationMethodConfiguration](../api/emailauthenticationmethodconfiguration-get.md)|[emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md)|读取 emailAuthenticationMethodConfiguration 对象的属性和关系。|
|[更新 emailAuthenticationMethodConfiguration](../api/emailauthenticationmethodconfiguration-update.md)|[emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md)|更新 emailAuthenticationMethodConfiguration 对象的属性。|
|[删除 emailAuthenticationMethodConfiguration](../api/emailauthenticationmethodconfiguration-delete.md)|无|删除 emailAuthenticationMethodConfiguration 对象。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|id|String|身份验证方法策略标识符。 继承自 [authenticationMethodConfiguration](../resources/authenticationmethodconfiguration.md)。|
|状态|authenticationMethodState|指示是否启用此身份验证方法。 可取值为：`enabled`、`disabled`。|
|allowExternalIdToUseEmailOtp|externalEmailOtpState|确定外部用户是否可以使用电子邮件 OTP 进行身份验证。 可取值为：`default`、`enabled`、`disabled`、`unknownFutureValue`。 从 2021 年 10 开始，不使用公共预览的州中的租户将自动启用电子邮件 `default` OTP。|

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
