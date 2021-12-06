---
title: 强制删除域
description: 使用异步长时间运行的操作删除域。
author: adimitui
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 6ba7dd7cf8a29ddfa008931ee8f210caf6bcc872
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60973927"
---
# <a name="force-domain-deletion"></a>强制删除域

命名空间：microsoft.graph

使用异步长时间运行的操作删除域。

在调用 [forceDelete](domain-forcedelete.md)之前，必须更新或删除对 **Exchange设置服务** 的任何引用。

以下操作作为此操作的一部分执行：

* 使用 `userPrincipalName` 对 `mail` 已删除域的引用更新 的 、 和 属性，以使用初始 `proxyAddresses` onmicrosoft.com `users` 域。

* 使用对已删除域的引用更新 的 属性 `mail` `groups` ，以使用初始 onmicrosoft.com 域。

* 使用对已删除域的引用更新 的 属性 `identifierUris` `applications` ，以使用初始 onmicrosoft.com 域。

* 如果要重命名的对象数大于 1000，则返回错误。

* 如果要重命名的 `applications` 之一是多租户应用，则返回错误。

域删除完成后，已删除域的 API 操作将返回 HTTP 404 状态代码。 若要验证是否删除域，可以执行 get [域](domain-get.md) 操作。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Domain.ReadWrite.All  |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Domain.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /domains/{id}/forceDelete
```

> 对于 {id}，请使用其完全限定的域名指定该域。

## <a name="request-headers"></a>请求头

| 名称 | 说明 |
|:---------------|:----------|
| Authorization  | Bearer {token}。必需。|
| Content-Type  | application/json |

## <a name="request-body"></a>请求正文

在请求正文中，提供具有以下参数的 JSON 对象。

| 参数 | 类型 | 说明 |
|:---------------|:--------|:----------|
|`disableUserAccounts`|`Boolean`| 用于禁用重命名的用户帐户的选项。 如果禁用用户帐户，将不允许用户登录。 如果设置为 **true，** 将禁用作为此操作的 `users` 一部分进行更新。  默认值为 **True**。 |

## <a name="response-body"></a>响应正文

如果成功，此方法将返回 `HTTP/1.1 204 OK` 状态代码。

## <a name="example"></a>示例

### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "domain_forcedelete"
}-->

```http
POST https://graph.microsoft.com/v1.0/domains/{id}/forceDelete
Content-type: application/json

{
  "disableUserAccounts": true
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/domain-forcedelete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/domain-forcedelete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/domain-forcedelete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/domain-forcedelete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/domain-forcedelete-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domain: forcedelete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

