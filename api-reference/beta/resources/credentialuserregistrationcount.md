---
title: credentialUserRegistrationCount 资源类型
description: 表示您的组织中的多少用户为自助密码重置和多重身份验证功能注册的用户的当前状态。
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: cd08bbcd6a189c2f76c130d28ea749745a5f8fca
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507343"
---
# <a name="credentialuserregistrationcount-resource-type"></a>credentialUserRegistrationCount 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示您的组织中的多少用户为自助密码重置和多重身份验证功能注册的用户的当前状态。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [getCredentialUserRegistrationCount](../api/reportroot-getcredentialuserregistrationcount.md) | credentialUserRegistrationCount 集合 | 报告您的组织中的多少用户为自助密码重置和多重身份验证（MFA）功能注册的用户的当前状态。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
| id | String | 活动的唯一标识符。 只读。 |
| totalUserCount | Int64 | 提供租户中的总用户计数。 |
| userRegistrationCounts | [userRegistrationCount](userregistrationcount.md)集合 | 租户中用户的注册计数和状态信息的集合。 |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.credentialUserRegistrationCount",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id" : "String",
  "totalUserCount" : 23123,
  "userRegistrationCounts" :
  [
    { "registrationStatus":"registered", "registrationCount": 23423 },
    { "registrationStatus":"enabled", "registrationCount": 4234 },
    { "registrationStatus":"capable", "registrationCount": 323 },
    { "registrationStatus":"mfaRegistered", "registrationCount": 33 }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "credentialUserRegistrationCount resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->