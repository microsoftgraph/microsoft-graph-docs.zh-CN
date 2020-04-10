---
title: 'trustFrameworkKeySet: uploadPkcs12'
description: 将 PKCS 12 格式密钥（PFX）上传到键集。
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 64d5b2d2c10194156a1b577437d1e7a90773b80a
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/10/2020
ms.locfileid: "43219009"
---
# <a name="trustframeworkkeyset-uploadpkcs12"></a>trustFrameworkKeySet: uploadPkcs12

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

将 PKCS12 格式密钥（PFX）上载到[trustFrameworkKeyset](../resources/trustframeworkkeyset.md)。 输入是 Pfx 证书内容的 base-64 编码值。 此方法返回[trustFrameworkKey](../resources/trustframeworkkey.md)。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | TrustFrameworkKeySet |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | TrustFrameworkKeySet |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets/{id}/uploadPkcs12
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
|Key|字符串|这是用于发送 pfx 内容的字段。 该值应为实际证书内容的以64编码的版本。|
|密码|String|这是将密码发送给 PFX 内容的字段。|

## <a name="response"></a>响应

如果成功，此方法在响应`200 OK`正文中返回响应代码和新的[trustFrameworkKey](../resources/trustframeworkkey.md)对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "trustframeworkkeyset_uploadpkcs12"
}-->

```http
POST https://graph.microsoft.com/beta/trustFramework/keySets/{id}/uploadPkcs12
Content-type: application/json

{
  "key": "Base64-encoded-pfx-content",
  "password": "password-value"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/trustframeworkkeyset-uploadpkcs12-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/trustframeworkkeyset-uploadpkcs12-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/trustframeworkkeyset-uploadpkcs12-objc-snippets.md)]
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
    "use": "sig",
    "kty": "OCT",
    "nbf": 1508969811,
    "exp": 1508973711
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "trustFrameworkKeySet: uploadPkcs12",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
