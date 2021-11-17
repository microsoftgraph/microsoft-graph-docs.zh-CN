---
title: Get federatedIdentityCredential
description: 读取 federatedIdentityCredential 对象的属性和关系。
author: kjyam98
ms.localizationpriority: medium
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 15eab45b2b06d527a40c5b2eaf4bb17f9ec9d9f2
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60978301"
---
# <a name="get-federatedidentitycredential"></a>Get federatedIdentityCredential
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

读取 [federatedIdentityCredential](../resources/federatedidentitycredential.md) 对象的属性和关系。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Application.ReadWrite.All    |
|委派（个人 Microsoft 帐户） |  Application.ReadWrite.All |
|应用程序 | Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All |


## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /applications/{applicationsId}/federatedIdentityCredentials/{federatedIdentityCredentialId}
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 `$select` [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。

## <a name="request-headers"></a>请求头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [federatedIdentityCredential](../resources/federatedidentitycredential.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_federatedidentitycredential"
}
-->
``` http
GET https://graph.microsoft.com/beta/applications/acd7c908-1c4d-4d48-93ee-ff38349a75c8/federatedIdentityCredentials/bdad0963-4a7a-43ae-b569-e67e1da3f2c0
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-federatedidentitycredential-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-federatedidentitycredential-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-federatedidentitycredential-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-federatedidentitycredential-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-federatedidentitycredential-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
下面展示了示例响应。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.federatedIdentityCredential"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#applications('cd7c908-1c4d-4d48-93ee-ff38349a75c8')/federatedIdentityCredentials/$entity",
    "@odata.id": "https://graph.microsoft.com/v2/3d1e2be9-a10a-4a0c-8380-7ce190f98ed9/directoryObjects/$/Microsoft.DirectoryServices.Application('bcd7c908-1c4d-4d48-93ee-ff38349a75c8')/federatedIdentityCredentials('bdad0963-4a7a-43ae-b569-e67e1da3f2c0')/bdad0963-4a7a-43ae-b569-e67e1da3f2c0",
    "id": "bdad0963-4a7a-43ae-b569-e67e1da3f2c0",
    "name": "testing",
    "issuer": "https://login.microsoftonline.com/3d1e2be9-a10a-4a0c-8380-7ce190f98ed9/v2.0",
    "subject": "a7d388c3-5e3f-4959-ac7d-786b3383006a",
    "description": "This is my test  federated identity credential",
    "audiences": [
        "api://AzureADTokenExchange"
    ]
  }
}
```

