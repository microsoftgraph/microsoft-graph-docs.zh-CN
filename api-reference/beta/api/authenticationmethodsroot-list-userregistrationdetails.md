---
title: 列出 userRegistrationDetails
description: 获取为用户注册的身份验证方法的列表，如 userRegistrationDetails 对象中的定义。
author: danielwood95
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: f89d322841c7b9d3e1d6c3153bd6e9e06415b5cb
ms.sourcegitcommit: de9df4bf6313b49afba74b6e9ef819907669c662
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/27/2022
ms.locfileid: "62239006"
---
# <a name="list-userregistrationdetails"></a>列出 userRegistrationDetails
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取为用户注册的身份验证方法的列表，如 [userRegistrationDetails](../resources/userregistrationdetails.md) 对象中的定义。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|UserAuthenticationMethod.Read.All、AuditLog.Read.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|UserAuthenticationMethod.Read.All、AuditLog.Read.All|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/authenticationMethods/userRegistrationDetails
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法仅支持 `$filter` 和 `$orderBy` OData 查询参数来帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [userRegistrationDetails](../resources/userregistrationdetails.md) 对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_userregistrationdetails"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/authenticationMethods/userRegistrationDetails
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-userregistrationdetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-userregistrationdetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-userregistrationdetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-userregistrationdetails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-userregistrationdetails-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-userregistrationdetails-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.userRegistrationDetails)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#reports/authenticationMethods/userRegistrationDetails",
    "value": [
        {
            "id": "86462606-fde0-4fc4-9e0c-a20eb73e54c6",
            "userPrincipalName": "AlexW@Contoso.com",
            "userDisplayName": "Alex Wilber",
            "isSsprRegistered": false,
            "isSsprEnabled": false,
            "isSsprCapable": false,
            "isMfaRegistered": true,
            "isMfaCapable": true,
            "isPasswordlessCapable": false,
            "methodsRegistered": [
                "microsoftAuthenticatorPush",
                "softwareOneTimePasscode"
            ]
        },
        {
            "id": "c6ad1942-4afa-47f8-8d48-afb5d8d69d2f",
            "userPrincipalName": "AllanD@Contoso.com",
            "userDisplayName": "Allan Deyoung",
            "isSsprRegistered": false,
            "isSsprEnabled": false,
            "isSsprCapable": false,
            "isMfaRegistered": false,
            "isMfaCapable": false,
            "isPasswordlessCapable": false,
            "methodsRegistered": []
        },
        {
            "id": "c8096958-797c-44fa-8fde-a6fb62567cf0",
            "userPrincipalName": "BiancaP@Contoso.com",
            "userDisplayName": "Bianca Pisani",
            "isSsprRegistered": true,
            "isSsprEnabled": false,
            "isSsprCapable": false,
            "isMfaRegistered": true,
            "isMfaCapable": true,
            "isPasswordlessCapable": false,
            "methodsRegistered": [
                "mobilePhone",
                "microsoftAuthenticatorPush",
                "softwareOneTimePasscode"
            ]
        }
    ]
}
```

