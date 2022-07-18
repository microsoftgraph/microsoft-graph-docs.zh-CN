---
title: 创建 temporaryAccessPassMethod
description: 为用户创建新的 temporaryAccessPassAuthenticationMethod 对象。
author: tilarso
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 403d6e9bfa42df20820bd0db05b0c1a8acf10993
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66438521"
---
# <a name="create-temporaryaccesspassmethod"></a>创建 temporaryAccessPassMethod
命名空间：microsoft.graph

在用户上创建新的 [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) 对象。 用户只能有一个可在其指定生存期内可用的临时访问通行证。 如果用户在当前临时访问通行证有效时需要新的临时访问通行证，则管理员可以为用户创建新的临时访问通行证，删除以前的临时访问通行证，并创建新的临时访问通行证。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

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
POST /users/{id | userPrincipalName}/authentication/temporaryAccessPassMethods
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) 对象的 JSON 表示形式。

下表描述了创建 [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) 时可以使用的可选属性。

|属性|类型|说明|
|:---|:---|:---|
|isUsableOnce|布尔值|可选。 确定传递是否限制为一次性使用。 如果 `true`可以使用传递一次，则 `false`可在其生存期内多次使用该传递 **InMinutes** 设置。 多用临时访问传递 (`isUsableOnce = false`) ，只有在  [临时访问传递身份验证方法策略](../resources/temporaryaccesspassauthenticationmethodconfiguration.md)允许的情况下，才能创建并用于登录。|
|lifetimeInMinutes|Int32|可选。 临时AccessPass 的生存期（以分钟为单位），从创建时间开始，或者在 startDateTime（如果设置）。 必须介于 10 到 43200 (等效于 30 天) 。 如果未指定，则应用 [临时访问密码身份验证方法策略](../resources/temporaryaccesspassauthenticationmethodconfiguration.md)中的 **defaultLifetimeInMinutes** 设置。 |
|startDateTime|DateTimeOffset|可选。 临时AccessPass可供使用的日期和时间。 如果未指定，则临时访问密码在创建后可立即使用。| 

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_temporaryaccesspassauthenticationmethod_from_"
}
-->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/users/071cc716-8147-4397-a5ba-b2105951cc0b/authentication/temporaryAccessPassMethods
Content-Type: application/json

{
    "startDateTime": "2022-06-05T00:00:00.000Z",
    "lifetimeInMinutes": 60,
    "isUsableOnce": false
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-temporaryaccesspassauthenticationmethod-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-temporaryaccesspassauthenticationmethod-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-temporaryaccesspassauthenticationmethod-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-temporaryaccesspassauthenticationmethod-from--go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-temporaryaccesspassauthenticationmethod-from--powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.temporaryAccessPassAuthenticationMethod"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.temporaryAccessPassAuthenticationMethod",
    "id": "6f1967b7-15e8-4935-ac26-d50770ed07a7",
    "temporaryAccessPass": "+drkzqAD",
    "createdDateTime": "2022-06-02T16:21:09.765173Z",
    "startDateTime": "2022-06-05T00:00:00Z",
    "lifetimeInMinutes": 60,
    "isUsableOnce": false,
    "isUsable": false,
    "methodUsabilityReason": "NotYetValid"
}
```
