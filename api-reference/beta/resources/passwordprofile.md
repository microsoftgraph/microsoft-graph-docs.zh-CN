---
title: passwordProfile 资源类型
description: 包含与用户关联的密码配置文件。用户 实体的 **passwordProfile** 属性是一个 **passwordProfile** 对象。
localization_priority: Normal
ms.openlocfilehash: 11930b046fafaf89f8db751891b9b7f2f72fd99d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839002"
---
# <a name="passwordprofile-resource-type"></a>passwordProfile 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

包含与用户关联的密码配置文件。[用户](user.md) 实体的 **passwordProfile** 属性是一个 **passwordProfile** 对象。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|forceChangePasswordNextSignIn|布尔| 如果**true**，在下一步登录，用户必须更改其密码。 密码更改之后，此属性将自动重置为 ***false**。 如果不设置，默认值为**false**。 |
|forceChangePasswordNextSignInWithMfa|布尔| 如果**true**，在下一步登录，用户必须执行在之前的多因素身份验证 (MFA) 强制更改其密码。 行为等同于**forceChangePasswordNextSignIn**之处在于密码更改之前先执行多因素身份验证所需的用户。 密码更改之后，此属性将自动重置为**false**。 如果不设置，默认值为**false**。 |
|password|String|用户的密码。创建用户时此属性是必需的。此属性可以更新，但用户在下次登录时必须更改密码。密码必须满足用户的 **passwordPolicies** 属性指定的最低要求。默认情况下，必须使用强密码。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordprofile"
}-->

```json
{
  "forceChangePasswordNextSignIn": true,
  "forceChangePasswordNextSignInWithMfa": false,
  "password": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordProfile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
