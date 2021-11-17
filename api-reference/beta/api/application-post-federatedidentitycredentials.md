---
title: Create federatedIdentityCredential
description: 为应用程序创建新的 federatedIdentityCredential 对象。
author: kjyam98
ms.localizationpriority: medium
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 32c78ddb7525c2331dd16cbb5bc4661f49e260df
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60983028"
---
# <a name="create-federatedidentitycredential"></a>Create federatedIdentityCredential
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

为应用程序 [创建新的 federatedIdentityCredential](../resources/federatedidentitycredential.md) 对象。 通过[](/azure/active-directory/develop/workload-identity-federation-create-trust)为计算平台配置 Azure AD 应用程序注册和标识提供程序之间的信任关系，可以使用该平台颁发的令牌向 Microsoft 标识平台 进行身份验证，并调用 Microsoft 生态系统中的 API。 最多可向应用程序添加 20 个对象。

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
POST /applications/{applicationsId}/federatedIdentityCredentials
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [federatedIdentityCredential](../resources/federatedidentitycredential.md) 对象的 JSON 表示形式。

下表显示创建 [federatedIdentityCredential](../resources/federatedidentitycredential.md)时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|访问群体|String collection|列出可在外部令牌中显示访问群体。 此字段是必需的，默认为"api://AzureADTokenExchange"。 它指出Microsoft 标识平台令牌中的 `aud` 声明应接受哪些信息。 此值表示Azure AD标识提供程序中的令牌，并且未跨标识固定值 - 可能需要在标识提供程序中创建新的应用程序注册，以用作此令牌的受众。 必需。|
|issuer|String|T外部标识提供程序的 URL，并且必须与要交换的外部令牌的颁发者声明相匹配。 颁发者和主题的值组合在应用中必须是唯一的。 必需。|
|name|String|联合标识凭据的唯一标识符，其字符限制为 120 个字符，并且必须为 URL 友好。 创建后不可变|
|subject|String|必需。 外部标识提供程序中的外部软件工作负荷的标识符。 与访问群体值一样，它没有固定格式，因为每个标识提供程序都使用其自己的格式，有时是 GUID，有时是冒号分隔的标识符，有时是任意字符串。 此处的值必须与向用户呈现的令牌中的子声明Azure AD。 颁发者和 **主题****的组合在** 应用中必须是唯一的。|



## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [federatedIdentityCredential](../resources/federatedidentitycredential.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_federatedidentitycredential_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/applications/bcd7c908-1c4d-4d48-93ee-ff38349a75c8/federatedIdentityCredentials/
Content-Type: application/json

{
    "name": "testing02",
    "issuer": "https://login.microsoftonline.com/3d1e2be9-a10a-4a0c-8380-7ce190f98ed9/v2.0",
    "subject": "a7d388c3-5e3f-4959-ac7d-786b3383006a",
    "audiences": [
        "api://AzureADTokenExchange"
    ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-federatedidentitycredential-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-federatedidentitycredential-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-federatedidentitycredential-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-federatedidentitycredential-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-federatedidentitycredential-from--go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.federatedIdentityCredential"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#applications('bcd7c908-1c4d-4d48-93ee-ff38349a75c8')/federatedIdentityCredentials/$entity",
    "@odata.id": "https://graph.microsoft.com/v2/3d1e2be9-a10a-4a0c-8380-7ce190f98ed9/directoryObjects/$/Microsoft.DirectoryServices.Application('bcd7c908-1c4d-4d48-93ee-ff38349a75c8')/federatedIdentityCredentials/d9b7bf1e-429e-4678-8132-9b00c9846cc4",
    "id": "d9b7bf1e-429e-4678-8132-9b00c9846cc4",
    "name": "testing02",
    "issuer": "https://login.microsoftonline.com/3d1e2be9-a10a-4a0c-8380-7ce190f98ed9/v2.0",
    "subject": "a7d388c3-5e3f-4959-ac7d-786b3383006a",
    "description": null,
    "audiences": [
        "api://AzureADTokenExchange"
    ]
}
```

