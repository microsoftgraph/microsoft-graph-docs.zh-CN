---
title: credentialUserRegistrationDetails 资源类型
description: 表示所有注册用户的 MFA 身份验证中自助服务密码重置和多重 (身份验证) 的详细信息。
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: c7e45b186e1ef7a3a96115f408cb5a0992e538fe
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159904"
---
# <a name="credentialuserregistrationdetails-resource-type"></a>credentialUserRegistrationDetails 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示所有注册用户的 MFA 身份验证中自助服务密码重置和多重 (身份验证) 的详细信息。 详细信息包括用户信息、注册状态和使用的身份验证方法。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 credentialUserRegistrationDetails](../api/reportroot-list-credentialuserregistrationdetails.md) | credentialUserRegistrationDetails 集合 | 获取给定租户 [的 credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) 对象列表。
 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
| authMethods | registrationAuthMethod 集合 | 表示用户已注册的身份验证方法。 可能的值是：、 (仅用于自助服务密码重置) 、和 (仅支持在注册 `email` `mobilePhone` `officePhone` `securityQuestion` `appNotification` `appCode` `alternateMobilePhone`) 。 |
| id | String | 活动的唯一标识符。 只读。|
| isCapable | 布尔 | 指示用户是否已准备好执行自助服务密码重置或 MFA。 |
| isEnabled | Boolean | 指示用户是否已启用执行自助服务密码重置。 |
| isMfaRegistered | 布尔 | 指示用户是否已注册 MFA。 |
| isRegistered | 布尔 | 指示用户是否已注册任何用于自助密码重置的身份验证方法。 |
| userDisplayName | String | 提供相应用户的用户名。 |
| userPrincipalName | String | 提供相应用户的用户主体名称。 |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.credentialUserRegistrationDetails",
  "keyProperty": "id"
}-->

```json
{
  "id" : "String",
  "userPrincipalName":"String",
  "userDisplayName": "String",
  "authMethods": ["string"],
  "isRegistered" : false,
  "isEnabled" : true,
  "isCapable" : false,
  "isMfaRegistered" : true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "credentialUserRegistrationDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


