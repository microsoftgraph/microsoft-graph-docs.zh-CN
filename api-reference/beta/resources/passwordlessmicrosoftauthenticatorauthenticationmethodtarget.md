---
title: passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget 资源类型
description: 启用了用户或组的集合，以使用 Microsoft 身份验证器 Passwordless Phone 登录身份验证方法策略。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a26a8fe76da954d3dc44a238665954539df0fa72
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418268"
---
# <a name="passwordlessmicrosoftauthenticatorauthenticationmethodtarget-resource-type"></a>passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

启用使用 Microsoft authentication Passwordless Phone 登录身份验证方法策略] ( 的用户或组的集合。。/resources/passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration.md) 在 Azure AD 中。

> [!NOTE]
> 在 Api 位于 Mirosoft Graph beta 过程中时，规划用于管理 Microsoft 身份验证器应用程序的 Api 的大量架构更改。 由于调用模式将发生更改，因此我们建议您不要对这些 Api 进行生产依赖。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|Azure AD 用户或组的对象 ID。|
|isRegistrationRequired|布尔|确定是否强制用户注册身份验证方法。|
|shownContext|authenticatorAppContextType|可取值为：`location`、`app`。|
|targetType|authenticationMethodTargetType|可取值为：`user`、`group`。|
|useForSignIn|布尔|确定身份验证方法是否可用于登录 Azure AD。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget",
  "baseType": "microsoft.graph.authenticationMethodTarget",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget",
  "id": "String (identifier)",
  "targetType": "String",
  "isRegistrationRequired": "Boolean",
  "useForSignIn": "Boolean",
  "shownContext": "String"
}
```
