---
title: userRegistrationDetails 资源类型
description: 表示用户的身份验证方法的状态，包括哪些方法已注册，哪些功能是用户注册的，哪些功能能够 (，例如多重身份验证、自助式密码重置和无密码身份验证) 。
author: besiler
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 55e3805de8619ef8e8b64f541b342991da6a44f7
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/01/2022
ms.locfileid: "65820187"
---
# <a name="userregistrationdetails-resource-type"></a>userRegistrationDetails 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示用户的身份验证方法的状态，包括哪些方法已注册，哪些功能是用户注册的，哪些功能能够 (，例如多重身份验证、自助式密码重置和无密码身份验证) 。

继承自 [entity](../resources/entity.md)。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 userRegistrationDetails](../api/authenticationmethodsroot-list-userregistrationdetails.md)|[userRegistrationDetails](../resources/userregistrationdetails.md) 集合|获取 [userRegistrationDetails](../resources/userregistrationdetails.md) 对象及其属性的列表。|
|[获取 userRegistrationDetails](../api/userregistrationdetails-get.md)|[userRegistrationDetails](../resources/userregistrationdetails.md)|读取 [userRegistrationDetails](../resources/userregistrationdetails.md) 对象的属性和关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|defaultMfaMethod|defaultMfaMethodType|选择作为默认方法的用户或管理员为用户执行多重身份验证的方法。 可取值包括：`none`、`mobilePhone`、`alternateMobilePhone`、`officePhone`、`microsoftAuthenticatorPush`、`softwareOneTimePasscode`、`unknownFutureValue`。|
|id|String|Azure AD 中的用户对象标识符。 继承自 [entity](../resources/entity.md)。|
|isMfaCapable|Boolean|用户是否注册了用于多重身份验证的强身份验证方法。 [身份验证方法](../resources/authenticationmethodspolicy.md)策略必须允许该方法。 支持 `$filter`（`eq`）。|
|isMfaRegistered|布尔|用户是否注册了用于多重身份验证的强身份验证方法。 [身份验证方法](../resources/authenticationmethodspolicy.md)策略不一定允许该方法。  支持 `$filter`（`eq`）。|
|isPasswordlessCapable|Boolean|用户是否注册了无密码强身份验证方法 (包括 FIDO2、Windows Hello 企业版 和Microsoft Authenticator ([身份验证方法策略](../resources/authenticationmethodspolicy.md)允许的无密码) ) 。 支持 `$filter`（`eq`）。|
|isSsprCapable|布尔|用户是否注册了自助式密码重置所需的身份验证方法数，并允许用户按策略执行自助密码重置。 支持 `$filter`（`eq`）。|
|isSsprEnabled|布尔|是否允许用户按策略执行自助密码重置。 用户可能不一定已注册自助密码重置所需的身份验证方法数。 支持 `$filter`（`eq`）。|
|isSsprRegistered|布尔|用户是否注册了自助密码重置所需的身份验证方法数。 不一定允许用户按策略执行自助密码重置。 支持 `$filter`（`eq`）。|
|methodsRegistered|String collection|注册的身份验证方法的集合，例如`mobilePhone`， `email``fido2` 支持 `$filter` (`any`) `eq` 。|
|userDisplayName|String| 用户显示名称，例如 `Adele Vance`。 支持 `$filter` (`eq`、 `startsWith`) 和 `$orderBy`。|
|userPrincipalName|String|用户主体名称，例如 `AdeleV@contoso.com`。 支持 `$filter` (`eq`、 `startsWith`) 和 `$orderBy`。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userRegistrationDetails",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userRegistrationDetails",
  "defaultMethod": "String",
  "id": "String (identifier)",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "isMfaRegistered": "Boolean",
  "isMfaCapable": "Boolean",
  "isSsprRegistered": "Boolean",
  "isSsprEnabled": "Boolean",
  "isSsprCapable": "Boolean",
  "isPasswordlessCapable": "Boolean",
  "methodsRegistered": [
    "String"
  ]
}
```

