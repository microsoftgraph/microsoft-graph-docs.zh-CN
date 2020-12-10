---
title: emailAuthenticationMethodConfiguration 资源类型
description: 代表电子邮件 OTP 身份验证方法策略
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3e3e18973759d7f120dd0bd8e984c98568054960
ms.sourcegitcommit: d9c167f6be71bdb4a023c5ace2733b9854c846d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2020
ms.locfileid: "49617113"
---
# <a name="emailauthenticationmethodconfiguration-resource-type"></a>emailAuthenticationMethodConfiguration 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示此租户的电子邮件 OTP 身份验证方法策略。 身份验证方法策略定义启用使用身份验证方法的配置设置和用户或组。 租户的云本机用户可以使用电子邮件 OTP 进行自助密码重置，也可以在某些情况下由外部用户用于身份验证。

## <a name="methods"></a>方法

|方法|返回类型|说明|
|:---|:---|:---|
|[获取 emailAuthenticationMethodConfiguration](../api/emailauthenticationmethodconfiguration-get.md)|[emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md)|读取 emailAuthenticationMethodConfiguration 对象的属性和关系。|
|[更新 emailAuthenticationMethodConfiguration](../api/emailauthenticationmethodconfiguration-update.md)|[emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md)|更新 emailAuthenticationMethodConfiguration 对象的属性。|
|[删除 emailAuthenticationMethodConfiguration](../api/emailauthenticationmethodconfiguration-delete.md)|无|删除一个 emailAuthenticationMethodConfiguration 对象。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|id|String|身份验证方法策略标识符。 继承自 [authenticationMethodConfiguration](../resources/authenticationmethodconfiguration.md)。|
|state|authenticationMethodState|指示是否启用此身份验证方法。 可取值为：`enabled`、`disabled`。|
|allowExternalIdToUseEmailOtp|externalEmailOtpState|确定外部用户是否可使用电子邮件 OTP 进行身份验证。 可取值为：`default`、`enabled`、`disabled`、`unknownFutureValue`。 `default`未使用公共预览版的状态中的租户将自动启用电子邮件 OTP （从3月2021开始）。|

## <a name="relationships"></a>关系

|关系|类型|说明|
|:---|:---|:---|
|includeTargets|[authenticationMethodTarget](../resources/authenticationmethodtarget.md) 集合|启用使用身份验证方法的用户或组的集合。|

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
