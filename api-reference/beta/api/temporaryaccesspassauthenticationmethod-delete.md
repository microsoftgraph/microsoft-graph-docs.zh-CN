---
title: 删除 temporaryAccessPassAuthenticationMethod
description: 删除用户的 temporaryAccessPassAuthenticationMethod 对象。
author: tilarso
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: d247ced1bfe21dd7e7b9235eb2b7c9b57492a6d0
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66093967"
---
# <a name="delete-temporaryaccesspassauthenticationmethod"></a>删除 temporaryAccessPassAuthenticationMethod
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

删除用户的 [临时AccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) 对象。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

### <a name="permissions-acting-on-self"></a>对自我执行操作的权限

|权限类型      | 权限（从最低特权到最高特权）              |
|:---------------------------------------|:-------------------------|
| 委派（工作或学校帐户）     | UserAuthenticationMethod.ReadWrite |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | 不支持。 |

### <a name="permissions-acting-on-other-users"></a>对其他用户执行操作的权限

|权限类型      | 权限（从最低特权到最高特权）              |
|:---------------------------------------|:-------------------------|
| 委派（工作或学校帐户）     | UserAuthenticationMethod.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | UserAuthenticationMethod.ReadWrite.All |

对于管理员对另一用户执行操作的委派方案，管理员需要以下 [Azure AD 角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)之一：
* 全局管理员
* 特权身份验证管理员
* 身份验证管理员

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{id | userPrincipalName}/authentication/temporaryAccessPassMethods/{id}
DELETE /me/authentication/temporaryAccessPassMethods/{id}
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "delete_temporaryAccessPassAuthenticationMethod"
}
-->
```msgraph-interactive
DELETE https://graph.microsoft.com/beta/users/071cc716-8147-4397-a5ba-b2105951cc0b/authentication/temporaryAccessPassMethods/05267842-25b2-4b21-8abd-8e4982796f7f
```

### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
