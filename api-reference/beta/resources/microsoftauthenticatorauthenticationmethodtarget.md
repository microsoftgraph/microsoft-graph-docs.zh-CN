---
title: microsoftAuthenticatorAuthenticationMethodTarget 资源类型
description: 已启用使用 Microsoft Authenticator 身份验证方法策略的用户或组的集合。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: db612bd2ac7aec387574fe1e45c967e2525c2b12
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960382"
---
# <a name="microsoftauthenticatorauthenticationmethodtarget-resource-type"></a>microsoftAuthenticatorAuthenticationMethodTarget 资源类型
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 Azure AD 中启用了使用 [Microsoft Authenticator 身份验证方法策略](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md) 的用户或组的集合。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|Azure AD 用户或组的对象 ID。|
|authenticationMode|microsoftAuthenticatorAuthenticationMode|确定可用于登录的通知类型。 可能的值是 `any` `deviceBasedPush` ：、 (无密码) 、 `push` 。|
|featureSettings|authenticatorAppFeatureSettings|确定应用于 Microsoft Authenticator 的其他设置。 可能的值是 `null` `requireNumberMatching` ：、 (需要匹配 MFA 通知的号码。 对于手机登录通知，此值将被忽略) 。|
|isRegistrationRequired|Boolean|确定是否强制用户注册身份验证方法。 *不支持*。 |
|shownContext (Private Preview) |authenticatorAppContextType|确定应在通知正文中向用户显示有关登录的上下文类型。 可取值为：`location`、`app`。|
|targetType|authenticationMethodTargetType| 可取值为：`null`、`user`、`group`。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftAuthenticatorAuthenticationMethodTarget",
  "baseType": "microsoft.graph.authenticationMethodTarget",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftAuthenticatorAuthenticationMethodTarget",
  "targetType": "String",
  "id": "String (identifier)",
  "isRegistrationRequired": "Boolean",
  "authenticationMode": "String",
  "shownContext": "String",
  "featureSettings": "String"
}

```
