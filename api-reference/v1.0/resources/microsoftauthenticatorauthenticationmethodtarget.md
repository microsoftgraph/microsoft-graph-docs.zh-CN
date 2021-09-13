---
title: microsoftAuthenticatorAuthenticationMethodTarget 资源类型
description: 启用以使用身份验证方法策略Microsoft Authenticator组的集合。
author: mmcla
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 810403eff5801ebcbafd56cf3de6252fe1f68bf8
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59067078"
---
# <a name="microsoftauthenticatorauthenticationmethodtarget-resource-type"></a>microsoftAuthenticatorAuthenticationMethodTarget 资源类型
命名空间：microsoft.graph

在 Azure AD 中启用以使用Microsoft Authenticator[方法策略的用户](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md)或组的集合。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|Azure AD 用户或组的对象 ID。|
|authenticationMode|microsoftAuthenticatorAuthenticationMode|确定可用于登录的通知类型。 可能的值包括 `any` `deviceBasedPush` ：、 (无密码) 、 `push` 。|
|featureSettings|authenticatorAppFeatureSettings|确定应用于其他设置Microsoft Authenticator。 可能的值是 `null` `requireNumberMatching` ：、 (需要匹配 MFA 通知的号码。 对于电话登录通知，此值将被忽略) 。|
|isRegistrationRequired|Boolean|确定是否强制用户注册身份验证方法。 *不支持*。 |
|shownContext|authenticatorAppContextType| (个人预览) 确定应在通知正文中向用户显示有关登录的上下文类型。 可取值为：`location`、`app`。|
|targetType|authenticationMethodTargetType| 可取值为：`user`、`group`。|

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
