---
title: 列出 temporaryAccessPassMethods
description: 获取用户的 temporaryAccessPassAuthenticationMethod 对象的列表。
author: tilarso
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: d742a2bcb2664aab4152ee35306475b23a83f576
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66096348"
---
# <a name="list-temporaryaccesspassmethods"></a>列出 temporaryAccessPassMethods
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


检索用户的 [临时AccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) 对象及其属性的列表。 此 API 只会返回集合中的单个对象，因为用户只能有一个临时访问传递方法。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

### <a name="permissions-acting-on-self"></a>对自我执行操作的权限

|权限类型      | 权限（从最低特权到最高特权）              |
|:---------------------------------------|:-------------------------|
| 委派（工作或学校帐户）     | UserAuthenticationMethod.Read、UserAuthenticationMethod.ReadWrite |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | 不支持。 |

### <a name="permissions-acting-on-other-users"></a>对其他用户执行操作的权限

|权限类型      | 权限（从最低特权到最高特权）              |
|:---------------------------------------|:-------------------------|
| 委派（工作或学校帐户）     | UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All |


对于管理员对另一用户执行操作的委派方案，管理员需要以下 [角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)之一：

* 全球管理员
* 全局读取者
* 特权身份验证管理员
* 身份验证管理员

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/temporaryAccessPassMethods
GET /users/{id | userPrincipalName}/authentication/temporaryAccessPassMethods
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法不支持自定义响应的可选查询参数。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request"></a>请求 
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) 对象的集合。  此调用仅返回一个对象，因为用户只能设置一个 **temporaryAccessPassAuthenticationMethod** 。

## <a name="examples"></a>示例

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "list_temporaryaccesspassauthenticationmethod"
}
-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/071cc716-8147-4397-a5ba-b2105951cc0b/authentication/temporaryAccessPassMethods
```

### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.temporaryAccessPassAuthenticationMethod)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('071cc716-8147-4397-a5ba-b2105951cc0b')/authentication/temporaryAccessPassMethods",
     "value": [
        {
            "id": "bdaede67-61e0-4349-9347-d2d6afd84009",
            "temporaryAccessPass": null,
            "createdDateTime": "2022-06-06T16:43:04.6438213Z",
            "startDateTime": "2022-06-06T16:48:03.027Z",
            "lifetimeInMinutes": 60,
            "isUsableOnce": false,
            "isUsable": false,
            "methodUsabilityReason": "NotYetValid"
        }
    ]
}
```
