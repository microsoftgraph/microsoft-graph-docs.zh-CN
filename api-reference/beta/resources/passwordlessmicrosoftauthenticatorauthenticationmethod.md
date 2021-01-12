---
title: passwordlessMicrosoftAuthenticatorAuthenticationMethod 资源类型
description: 向用户注册的 Microsoft Authenticator 无密码电话登录方法的表示形式。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8815d84a8a85491399e97f7d10aa2e6cc1aeaf9d
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796547"
---
# <a name="passwordlessmicrosoftauthenticatorauthenticationmethod-resource-type-deprecated"></a>passwordlessMicrosoftAuthenticatorAuthenticationMethod 资源类型 (已弃) 

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

向用户注册的 Microsoft Authenticator 无密码电话登录方法的表示形式。

> [!CAUTION]
> Microsoft Authenticator 无密码电话登录方法 API 已弃用，将在 2020 年 12 月 31 日停止返回结果。 请使用新的 [Microsoft Authenticator 身份验证方法](../resources/microsoftAuthenticatorAuthenticationMethod.md)。


## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出](../api/passwordlessmicrosoftauthenticatorauthenticationmethod-list.md) (弃) |[passwordlessMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) 集合|检索用户的无密码MicrosoftAuthenticatorAuthenticationMethod 对象及其属性的列表。|
|[获取](../api/passwordlessmicrosoftauthenticatorauthenticationmethod-get.md) (弃) |[passwordlessMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md)|读取用户的无密码MicrosoftAuthenticatorAuthenticationMethod 对象的属性和关系。|
|[删除](../api/passwordlessmicrosoftauthenticatorauthenticationmethod-delete.md) (弃) |无|删除用户的无密码MicrosoftAuthenticatorAuthenticationMethod 对象。|


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|身份验证方法标识符。|
|displayName|String|用户显示名称移动设备的运行时间。|
|creationDateTime|DateTimeOffset|向用户注册此方法的时间戳。|


## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethod",
  "baseType": "microsoft.graph.authenticationMethod",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethod",
  "id": "String (identifier)",
  "displayName": "String",
  "creationDateTime": "String (timestamp)"
}
```

