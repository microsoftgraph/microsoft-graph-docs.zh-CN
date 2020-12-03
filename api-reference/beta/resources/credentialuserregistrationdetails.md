---
title: credentialUserRegistrationDetails 资源类型
description: 表示对所有注册用户使用自助密码重置和多重身份验证 (MFA) 的详细信息。
localization_priority: Normal
author: besiler
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 56d3f603fd9a8daf0c19e30c566379390aca7aed
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523726"
---
# <a name="credentialuserregistrationdetails-resource-type"></a>credentialUserRegistrationDetails 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示对所有注册用户使用自助密码重置和多重身份验证 (MFA) 的详细信息。 详细信息包括用户信息、注册状态和使用的身份验证方法。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 credentialUserRegistrationDetails](../api/reportroot-list-credentialuserregistrationdetails.md) | credentialUserRegistrationDetails 集合 | 获取给定租户的 [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) 对象的列表。
 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
| authMethods | registrationAuthMethod 集合 | 表示用户已注册的身份验证方法。 可能的值为： `email` 、 `mobilePhone` 、、 `officePhone` `securityQuestion` (仅用于自助密码重置) 、、 `appNotification` `appCode` 和 `alternateMobilePhone` (仅在注册) 中受支持。 |
| id | String | 活动的唯一标识符。 只读。|
| isCapable | 布尔值 | 指示用户是否已准备好执行自助密码重置或进行 MFA。 |
| isEnabled | Boolean | Indiciates 是否允许用户执行自助密码重置。 |
| isMfaRegistered | 布尔值 | Indiciates 是否为用户注册了 MFA。 |
| isRegistered | 布尔值 | 指示用户是否已将任何身份验证方法注册为自助密码重置。 |
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
  "baseType": "",
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


