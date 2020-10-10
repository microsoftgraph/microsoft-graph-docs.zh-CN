---
title: passwordlessMicrosoftAuthenticatorAuthenticationMethod 资源类型
description: 向用户注册的 Microsoft 身份验证 Passwordless 电话登录方法的表示形式。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b34b807106591390198c58d26d7804dc6ada5460
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418270"
---
# <a name="passwordlessmicrosoftauthenticatorauthenticationmethod-resource-type"></a>passwordlessMicrosoftAuthenticatorAuthenticationMethod 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

向用户注册的 Microsoft 身份验证 Passwordless 电话登录方法的表示形式。

> [!NOTE]
> 在 Api 位于 Mirosoft Graph beta 过程中时，规划用于管理 Microsoft 身份验证器应用程序的 Api 的大量架构更改。 由于调用模式将发生更改，因此我们建议您不要对这些 Api 进行生产依赖。


## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List](../api/passwordlessmicrosoftauthenticatorauthenticationmethod-list.md)|[passwordlessMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) 集合|检索用户的 passwordlessMicrosoftAuthenticatorAuthenticationMethod 对象及其属性的列表。|
|[获取](../api/passwordlessmicrosoftauthenticatorauthenticationmethod-get.md)|[passwordlessMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md)|读取用户的 passwordlessMicrosoftAuthenticatorAuthenticationMethod 对象的属性和关系。|
|[删除](../api/passwordlessmicrosoftauthenticatorauthenticationmethod-delete.md)|无|删除用户的 passwordlessMicrosoftAuthenticatorAuthenticationMethod 对象。|


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|身份验证方法标识符。|
|displayName|字符串|由用户指定的移动设备的显示名称。|
|creationDateTime|DateTimeOffset|向用户注册此方法时的时间戳。|


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

