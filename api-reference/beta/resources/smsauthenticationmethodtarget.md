---
title: smsAuthenticationMethodTarget 资源类型
description: 已启用使用短信身份验证方法策略的用户或组的集合。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 4309316adfeff126f845dd362d5ffb8899a77e60
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761028"
---
# <a name="smsauthenticationmethodtarget-resource-type"></a>smsAuthenticationMethodTarget 资源类型
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 Azure AD 中启用使用 [短信身份验证方法策略的用户](../resources/smsAuthenticationMethodConfiguration.md) 或组的集合。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|Azure AD 用户或组的对象 ID。|
|isRegistrationRequired|布尔|确定是否强制用户注册身份验证方法。 **不支持**。|
|isUsableForSignIn|布尔|确定用户或组能否使用此身份验证方法登录到 Azure AD。 该值始终为 `true` 。|
|targetType|authenticationMethodTargetType| 可取值为：`user`、`group`。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.smsAuthenticationMethodTarget",
  "baseType": "microsoft.graph.authenticationMethodTarget",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.smsAuthenticationMethodTarget",
  "targetType": "String",
  "id": "String (identifier)",
  "isRegistrationRequired": "Boolean",
  "isUsableForSignIn": "Boolean"
}
```
