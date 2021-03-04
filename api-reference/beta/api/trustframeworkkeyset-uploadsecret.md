---
title: trustFrameworkKeySet：uploadSecret
description: 将密码上载到密钥集。
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: b008e1ae41d61fb14dbd80e5a820208355bb670d
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444971"
---
# <a name="trustframeworkkeyset-uploadsecret"></a>trustFrameworkKeySet：uploadSecret

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

将纯文本密码上载到 [trustFrameworkKeyset](../resources/trustframeworkkeyset.md)。 密码示例包括 Azure Active Directory、Google、Facebook 或其他任何标识提供程序中的应用程序密码。 他的方法返回 [trustFrameworkKey](../resources/trustframeworkkey.md)。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | TrustFrameworkKeySet.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| Application                            | TrustFrameworkKeySet.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets/{id}/uploadSecret
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明   |
|:--------------|:--------------|
| Authorization | Bearer {token}。必需。 |
| Content-type  | application/json. Required. |

## <a name="request-body"></a>请求正文

在请求正文中，提供具有以下参数的 JSON 对象。

| 参数    | 类型        | 说明 |
|:-------------|:------------|:------------|
|use|String|类似于 **trustFrameworkKey 的 use 属性**。 |
|k|String|类似于 **trustFrameworkKey** 的 **k** 属性。 这是用于发送密码的字段。|
|nbf|Int64|类似于 **trustFrameworkKey** 的 **nbf** 属性。|
|exp|Int64|类似于 **trustFrameworkKey 的** **exp** 属性。|

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回响应代码和新 `200 OK` [trustFrameworkKey](../resources/trustframeworkkey.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "trustframeworkkeyset_uploadsecret"
}-->

```http
POST https://graph.microsoft.com/beta/trustFramework/keySets/{id}/uploadSecret
Content-type: application/json

{
  "use": "use-value",
  "k": "application-secret-to-be-uploaded",
  "nbf": 1508969811,
  "exp": 1508973711
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/trustframeworkkeyset-uploadsecret-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/trustframeworkkeyset-uploadsecret-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/trustframeworkkeyset-uploadsecret-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/trustframeworkkeyset-uploadsecret-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkKey"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "kid": "kid-value",
    "use": "use-value",
    "kty": "OCT",
    "nbf": 1508969811,
    "exp": 1508973711
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "trustFrameworkKeySet: uploadSecret",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


