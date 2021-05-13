---
title: servicePrincipal：addTokenSigningCertificate
description: 将签名证书添加到 servicePrincipal。
localization_priority: Normal
author: luleonpla
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 8cb462e31817c229b44ac2042e8d61073af58479
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474655"
---
# <a name="serviceprincipal-addtokensigningcertificate"></a>servicePrincipal：addTokenSigningCertificate

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建自签名签名证书并返回 [selfSignedCertificate，](../resources/selfsignedcertificate.md)这是生成的证书的公共部分。 自签名签名证书由以下资源组成：使用 = "Sign") 的私钥 ([keyCredential、](../resources/keycredential.md) 使用 = "verify") 的公钥 ([keyCredential](../resources/keycredential.md) 和 [passwordCredential](../resources/passwordcredential.md)。 所有已创建的资源具有相同的 **customKeyIdentifier**。

**passwordCredential** 用于打开 pfx/私钥。 此外，它还与具有相同 **keyId** 的 privateKey 相关联。 证书的主题是一个常量值。 它不受 POST 调用中提供的可选 **displayName** 的影响。 **startDateTime** 设置为使用 操作创建证书的同一时间。 **endDateTime** 可在证书创建后最多三年。

## <a name="permissions"></a>权限

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Application.ReadWrite.All、Directory.ReadWrite.All |
|委派（个人 Microsoft 帐户） | 无。    |
|应用程序 | Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.ReadWrite.All |


## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/addTokenSigningCertificate
```

## <a name="request-body"></a>请求正文

在请求正文中，提供以下必需属性。

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
| displayName | string | 密钥的友好名称。  它必须以 `CN=` 开始。|
| endDateTime | DateTimeOffset |凭据过期的日期和时间。 从证书创建之日起，最多 3 年。 如果未提供，则默认值为自创建时起三年。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示："2014-01-01T00：00：00Z"。|

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和新 `200 OK` [selfSignedCertificate](../resources/selfsignedcertificate.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_addtokensigningcertificate"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/004375c5-6e2e-4dec-95e3-626838cb9f80/addTokenSigningCertificate
Content-type: application/json

{
    "displayName":"CN=customDisplayName",
    "endDateTime":"2024-01-25T00:00:00Z"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-addtokensigningcertificate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-addtokensigningcertificate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-addtokensigningcertificate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-addtokensigningcertificate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.selfSignedCertificate"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.selfSignedCertificate",
  "customKeyIdentifier": "2iD8ppbE+D6Kmu1ZvjM2jtQh88E=",
  "displayName": "CN=customDisplayName",
  "endDateTime": "2024-01-25T00:00:00Z",
  "key": "MIICuDCCAaCgAwIBAgIIYXJsNtL4oUMwDQYJKoZIhvcNAQEL...StP8s/w==",
  "keyId": "93bc223f-7235-4b9c-beea-d66847531c49",
  "startDateTime": "2021-05-05T18:38:51.8100763Z",
  "thumbprint": "DA20FCA696C4F83E8A9AED59BE33368ED421F3C1",
  "type": "AsymmetricX509Cert",
  "usage": "Verify"
}
```
<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2021-01-15 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePrincipal: selfSignedCertificate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: serviceprincipal_selfsignedcertificate:\r\n      Resource type was null or missing, so we assume there is no response to validate."
    ]
} -->

