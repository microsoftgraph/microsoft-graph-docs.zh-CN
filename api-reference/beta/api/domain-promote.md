---
title: domain： promote
description: 将已验证的子域升级到根域。
author: franqq
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 73b17e18681d11b4ef103c363f4bf2a71b1c5fe9
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66446586"
---
# <a name="domain-promote"></a>domain： promote

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

将已验证的子域升级到根域。 已验证的域的 **isVerified** 属性设置为 `true`。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限  |
|:--------------------|:-------------|
|委派（工作或学校帐户） | Domain.ReadWrite.All |
|委派（个人 Microsoft 帐户） | 不支持。 |
|应用程序 | Domain.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/promote
```

> 对于 {id}，请使用其完全限定的域名指定该域。

## <a name="request-headers"></a>请求标头

| 名称       | 说明|
|:---------------|:----------|
| Authorization  | Bearer {token}。必需。|
| Content-Type  | application/json |

## <a name="request-body"></a>请求正文

## <a name="response"></a>响应

如果成功，此调用将返回一个 `200 OK` 响应和一个布尔值，该值指定内容类型的发布状态。

## <a name="example"></a>示例

### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "domain_promote"
}-->
```http
POST https://graph.microsoft.com/beta/domains/contoso.com/promote
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/domain-promote-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/domain-promote-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/domain-promote-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/domain-promote-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/domain-promote-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string"
}
-->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Edm.Boolean",
    "value": true
}
```
