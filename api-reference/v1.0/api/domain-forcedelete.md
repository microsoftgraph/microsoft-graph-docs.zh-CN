---
title: 强制域删除
description: 删除使用长时间运行的异步操作的域。
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 22ad640195fa9b14e0407a479438bf618d8f19c1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831351"
---
# <a name="force-domain-deletion"></a>强制域删除

删除使用长时间运行的异步操作的域。

此操作的一部分执行下列操作：

* 更新`userPrincipalName`， `mail`，和`proxyAddresses`属性`users`与要使用初始 onmicrosoft.com 域的已删除域的引用。

* 更新`mail`属性`groups`与要使用初始 onmicrosoft.com 域的已删除域的引用。

* 更新`identifierUris`属性`applications`与要使用初始 onmicrosoft.com 域的已删除域的引用。

* 如果要重命名的对象的数量大于 1000年，则返回错误。

* 如果的`applications`要重命名为多租户应用程序，则返回一个错误。

域删除完成后，已删除的域的 API 操作将返回 HTTP 404 状态代码。 若要验证删除的域，可以执行[get 域](domain-get.md)操作。

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

| 名称 | 说明 |
|:---------------|:----------|
| Authorization  | Bearer {token}。必需。|
| Content-Type  | application/json |

## <a name="request-body"></a>请求正文

在请求正文中，提供具有以下参数的 JSON 对象。

| 参数 | 类型 | Description |
|:---------------|:--------|:----------|
|`disableUserAccounts`|`Boolean`| 若要禁用其重命名用户帐户的选项。 如果禁用的用户帐户，则用户将不允许登录。 如果设置为**true** `users`更新为属于此操作将被禁用。  默认值为**true**。 |

## <a name="response-body"></a>响应正文

如果成功，此方法返回`HTTP/1.1 204 OK`状态代码。

## <a name="example"></a>示例

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "domain_forcedelete"
}-->

```http
POST https://graph.microsoft.com/beta/domains/{id}/forceDelete
Content-type: application/json
Content-length: 33

{
  "disableUserAccounts": true
}
```

### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
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
  "tocPath": ""
}-->
