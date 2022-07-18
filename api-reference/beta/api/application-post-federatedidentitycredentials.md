---
title: Create federatedIdentityCredential
description: 为应用程序创建新的 federatedIdentityCredential 对象。
author: shahzad-khalid
ms.localizationpriority: medium
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: b110f00734c7d7ad2044f289917713ad5d19887a
ms.sourcegitcommit: 995056279c2151d7ce4a0fcff067fbc6edced728
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/20/2022
ms.locfileid: "65602696"
---
# <a name="create-federatedidentitycredential"></a>Create federatedIdentityCredential
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

为应用程序创建新的 [federatedIdentityCredential](../resources/federatedidentitycredential.md) 对象。 通过在 Azure AD 应用程序注册与计算平台的标识提供者之间[配置信任关系](/azure/active-directory/develop/workload-identity-federation-create-trust)，可以使用该平台颁发的令牌对Microsoft 标识平台进行身份验证，并在 Microsoft 生态系统中调用 API。 最多可向应用程序添加 20 个对象。

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

下表显示了创建 [federatedIdentityCredential](../resources/federatedidentitycredential.md) 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|观众|字符串集合|列出可以在外部令牌中显示的受众。 此字段是必需的，默认为“api://AzureADTokenExchange”。 它说明了Microsoft 标识平台应该接受`aud`传入令牌中的声明。 此值表示外部标识提供程序中的 Azure AD，并且在标识提供者之间没有固定值 - 可能需要在标识提供者中创建新的应用程序注册，以充当此令牌的受众。 必需项。|
|发行|String|外部标识提供者的 URL，必须与要交换的外部令牌的颁发者声明匹配。 **颁发者** 和 **主题** 的值的组合在应用中必须是唯一的。 必需项。|
|name|String|联合标识凭据的唯一标识符，其字符限制为 120 个字符，并且必须对 URL 友好。 创建后它是不可变的|
|subject|String|必需。 外部标识提供程序中外部软件工作负荷的标识符。 与受众值一样，它没有固定格式，因为每个标识提供者都使用自己的标识提供者 - 有时是 GUID，有时是冒号分隔标识符，有时是任意字符串。 此处的值必须与显示给 Azure AD 的令牌中的子声明匹配。 **颁发者** 和 **主题** 的组合在应用中必须是唯一的。|



## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [federatedIdentityCredential](../resources/federatedidentitycredential.md) 对象。

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

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-federatedidentitycredential-from--go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-federatedidentitycredential-from--powershell-snippets.md)]
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

