---
title: 域： forceDelete
description: 删除使用异步操作的域。
author: lleonard-msft
ms.openlocfilehash: 4af5b70fca7600538d4212768243d8de82eb79ed
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316210"
---
# <a name="domain-forcedelete"></a>域： forceDelete

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

删除使用异步操作的域。

此操作的一部分执行下列操作：

* 重命名的 UPN、 EmailAddress 和 ProxyAddress 具有引用的已删除的域的用户。

* 重命名与引用的已删除的域的组的电子邮件地址。

* 重命名应用程序与已删除的域引用的 identifierUris。

* 如果要重命名的对象的数量大于 1000年，则返回错误。

* 如果要重命名的应用程序之一是多租户应用程序，则返回错误。

域删除完成后，已删除的域的 API 操作将返回 404 的 HTTP 响应代码。 若要验证删除的域，您可以执行[获取域](domain-get.md)。 如果已成功删除域，将在响应中返回 404 的 HTTP 响应代码。

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

| Name       | 说明|
|:---------------|:----------|
| Authorization  | Bearer {token}。必需。|
| Content-Type  | application/json |

## <a name="request-body"></a>请求正文

在请求正文中，提供具有以下参数的 JSON 对象。

| 参数    | Type   |说明|
|:---------------|:--------|:----------|
|disableUserAccounts|Boolean| 若要禁用重命名的用户帐户的选项。 如果禁用的用户帐户，则用户将不允许登录。<br>*True*（默认值）-重命名此操作的一部分的帐户被禁用的用户。<br>未禁用*false* -重命名此操作的一部分的用户帐户。 |

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
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domain: forcedelete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->