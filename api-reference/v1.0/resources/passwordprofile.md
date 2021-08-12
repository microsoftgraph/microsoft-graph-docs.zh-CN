---
title: passwordProfile 资源类型
description: 包含与用户关联的密码配置文件。用户实体的 **passwordProfile** 属性是一个 **passwordProfile** 对象。
localization_priority: Priority
author: eketo-msft
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 7288d2f737c0e04be9919ba0b2412df2ba1ebda8c377e1c66a3d6a91992af858
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54189399"
---
# <a name="passwordprofile-resource-type"></a>passwordProfile 资源类型

命名空间：microsoft.graph

包含与用户关联的密码配置文件。[用户](user.md) 实体的 **passwordProfile** 属性是一个 **passwordProfile** 对象。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|forceChangePasswordNextSignIn|Boolean| 如果用户在下次登录时必须更改密码，则为 `true`；否则为 `false`。 如未设置，默认值为 `false`。 **注意：** 对于 Azure B2C 租户，设置为`false`，并在首次登录时改为使用自定义策略和用户流强制重置密码。 请参阅[首次登录时强制密码重置](https://github.com/azure-ad-b2c/samples/tree/master/policies/force-password-reset-first-logon)。|
|forceChangePasswordNextSignInWithMfa|Boolean| 如果为 `true`，则在下次登录时，用户必须先执行多重身份验证 (MFA)，然后才会被强制更改密码。 该行为与 **forceChangePasswordNextSignIn** 相同，除了在更改密码之前用户必须先执行多重身份验证。 密码更改后，此属性将自动重置为 `false`。 如未设置，默认值为 `false`。 |
|密码|String|用户的密码。创建用户时此属性是必需的。此属性可以更新，但用户在下次登录时必须更改密码。密码必须满足用户的 **passwordPolicies** 属性指定的最低要求。默认情况下，必须使用强密码。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordProfile"
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

## <a name="see-also"></a>另请参阅

[更新用户的 passwordProfile](../api/user-update.md#example-3-update-the-passwordprofile-of-a-user-to-reset-their-password)
