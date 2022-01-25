---
title: userRegistrationDetails 资源类型
description: 表示用户的身份验证方法的状态，包括注册哪些方法以及用户注册哪些功能 (如多重身份验证、自助服务密码重置和无密码身份验证) 。
author: danielwood95
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 11d447b1b4c9069bd4c8d8c29271c4d0b6f51380
ms.sourcegitcommit: 9adf70c5da7c5b65f7d20f571d101ee06f023bc3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/25/2022
ms.locfileid: "62201763"
---
# <a name="userregistrationdetails-resource-type"></a>userRegistrationDetails 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示用户的身份验证方法的状态，包括注册哪些方法以及用户注册哪些功能 (如多重身份验证、自助服务密码重置和无密码身份验证) 。

继承自 [实体](../resources/entity.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 userRegistrationDetails](../api/authenticationmethodsroot-list-userregistrationdetails.md)|[userRegistrationDetails](../resources/userregistrationdetails.md) 集合|获取 [userRegistrationDetails](../resources/userregistrationdetails.md) 对象及其属性的列表。|
|[获取 userRegistrationDetails](../api/userregistrationdetails-get.md)|[userRegistrationDetails](../resources/userregistrationdetails.md)|读取 [userRegistrationDetails 对象的属性和](../resources/userregistrationdetails.md) 关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|用户对象标识符Azure AD。 继承自 [实体](../resources/entity.md)。|
|isMfaCapable|布尔值|用户是否已注册用于多重身份验证的强身份验证方法。 身份验证方法策略 必须允许 [此方法](../resources/authenticationmethodspolicy.md)。 支持 `$filter`（`eq`）。|
|isMfaRegistered|布尔值|用户是否已注册用于多重身份验证的强身份验证方法。 身份验证方法策略 不一定 [允许此方法](../resources/authenticationmethodspolicy.md)。  支持 `$filter`（`eq`）。|
|isPasswordlessCapable|布尔值|用户是否已注册无密码强身份验证方法 (包括身份验证方法策略所允许的 FIDO2、Windows Hello for Business 和 Microsoft Authenticator (Passwordless) ) 。 [](../resources/authenticationmethodspolicy.md) 支持 `$filter`（`eq`）。|
|isSsprCapable|布尔值|用户是否已注册自助服务密码重置所需的身份验证方法数，以及是否允许用户通过策略执行自助服务密码重置。 支持 `$filter`（`eq`）。|
|isSsprEnabled|布尔值|是否允许用户按策略执行自助服务密码重置。 用户不一定已注册自助服务密码重置所需的身份验证方法数。 支持 `$filter`（`eq`）。|
|isSsprRegistered|布尔值|用户是否已注册自助服务密码重置所需的身份验证方法数。 不一定允许用户通过策略执行自助服务密码重置。 支持 `$filter`（`eq`）。|
|methodsRegistered|字符串集合|注册的身份验证方法的集合，例如 `mobilePhone` 、 `email` `fido2` 、 。 支持 `$filter` `any` `eq` () 。|
|userDisplayName|String| 用户显示名称，例如 `Adele Vance` 。 支持 `$filter` (`eq` `startsWith` 、) 和 `$orderBy` 。|
|userPrincipalName|字符串|用户主体名称，例如 `AdeleV@contoso.com` 。 支持 `$filter` (`eq` `startsWith` 、) 和 `$orderBy` 。|

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

