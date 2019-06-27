---
title: '域: forceDelete'
description: 使用异步操作删除域。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f1220513f2ba5abf2957fa8c0e550e22985d2635
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260477"
---
# <a name="domain-forcedelete"></a>域: forceDelete

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

使用异步操作删除域。

在此操作过程中, 将执行以下操作:

* 使用对已删除域的引用重命名用户的 UPN、EmailAddress 和 ProxyAddress。

* 使用对已删除域的引用重命名组的 EmailAddress。

* 将应用程序的 identifierUris 重命名为对已删除的域的引用。

* 如果要重命名的对象的数量大于 1000, 则返回错误。

* 如果要重命名的某个应用程序是多租户应用程序, 则会返回错误。

域删除完成后, 已删除域的 API 操作将返回 404 HTTP 响应代码。 若要验证域的删除, 可以执行[获取域](domain-get.md)。 如果已成功删除域, 响应中将返回 404 HTTP 响应代码。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。


|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Directory.AccessAsUser.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Domain.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/forceDelete
```

> 对于 {id}，请使用其完全限定的域名指定该域。

## <a name="request-headers"></a>请求标头

| 名称       | 说明|
|:---------------|:----------|
| Authorization  | Bearer {token}。必需。|
| Content-Type  | application/json |

## <a name="request-body"></a>请求正文

在请求正文中，提供具有以下参数的 JSON 对象。

| 参数    | 类型   |说明|
|:---------------|:--------|:----------|
|disableUserAccounts|Boolean| 用于禁用重命名的用户帐户的选项。 如果用户帐户已禁用, 则不允许用户登录。<br>*True*(默认值)-已禁用作为此操作的一部分重命名的用户帐户。<br>*False* -不禁用作为此操作的一部分重命名的用户帐户。 |

## <a name="response"></a>响应

如果成功，此方法返回 `200 OK` 响应代码。 

## <a name="example"></a>示例
##### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "domain_forcedelete"
}-->
```http
POST https://graph.microsoft.com/beta/domains/contoso.com/forceDelete
Content-type: application/json
Content-length: 33

{
  "disableUserAccounts": true
}
```

##### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a>SDK 示例代码
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/domain_forcedelete-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/domain_forcedelete-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[目标-C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/domain_forcedelete-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "domain: forcedelete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/domain-forcedelete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/domain-forcedelete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/domain-forcedelete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
