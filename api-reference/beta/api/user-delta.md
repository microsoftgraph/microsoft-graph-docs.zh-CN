---
title: 'user: delta'
description: 获取新创建、更新或删除的用户, 而无需对整个用户集执行完全读取。 有关详细信息, 请参阅跟踪更改。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6fd8eb71c1b647550219ae6686a0bc814420b2fa
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32536999"
---
# <a name="user-delta"></a>user: delta

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取新创建、更新或删除的用户, 而无需对整个用户集执行完全读取。 有关详细信息, 请参阅[跟踪更改](/graph/delta-query-overview)。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。


|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All    |
|委派（个人 Microsoft 帐户） | User.Read、User.ReadWrite    |
|应用程序 | User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

为开始跟踪更改，请在用户资源上发出包含 delta 函数的请求。

<!-- { "blockType": "ignored" } -->
```http
GET /users/delta
```

## <a name="query-parameters"></a>查询参数

跟踪用户的更改会产生一个或多个**delta**函数调用的往返。 如果使用任何查询参数 (而不是`$deltatoken` and `$skiptoken`), 则必须在初始**delta**请求中指定它。 Microsoft Graph 自动将任何指定的参数编码到响应中提供`nextLink`的`deltaLink` or URL 的令牌部分。

只需预先指定所需的任何查询参数一次。

在后续请求中，可以复制并应用之前响应中返回的 `nextLink` 或 `deltaLink` URL，因为此 URL 已包含所需的编码参数。

| 查询参数      | 类型   |说明|
|:---------------|:--------|:----------|
| $deltatoken | string | 对同一个用户集合之前的 **delta** 函数调用的 `deltaLink` URL 中返回的[状态令牌](/graph/delta-query-overview)，指示该组更改跟踪的完成状态。将此令牌包含在对该集合的下一组更改追踪的首次请求中，并保存和应用整个 `deltaLink` URL。|
| $skiptoken | string | 对之前的 **delta** 函数调用的 `nextLink` URL 中返回的[状态令牌](/graph/delta-query-overview)，指示同一个用户集合中有进一步的更改需要追踪。 |

### <a name="odata-query-parameters"></a>OData 查询参数

此方法支持可选的 OData 查询参数来帮助自定义响应。

- 像在任何 GET 请求中一样，你可以使用 `$select` 查询参数以仅指定获取最佳性能所需的属性。始终返回 *id* 属性。
- 对`$filter`以下项的支持有限:
  - 唯一支持的 `$filter` 表达式用于跟踪对特定对象 `$filter=id+eq+{value}` 的更改。 可以筛选多个对象。 例如，`https://graph.microsoft.com/beta/users/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`。 筛选对象不能超出 50 个。

## <a name="request-headers"></a>请求标头
| 名称       | 说明|
|:---------------|:----------|
| Authorization  | 持有者&lt;令牌&gt;|
| Content-Type  | application/json |
| Prefer | return = 最小 <br><br>如果使用使用 a 的`deltaLink`请求指定此标头, 则将仅返回自上一轮后已更改的对象属性。 可选。 |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

### <a name="response"></a>响应

如果成功，此方法的响应正文返回`200 OK`响应代码和[用户](../resources/user.md)集合对象。 该响应还包括`nextLink` url 或`deltaLink` url。

- 如果返回`nextLink` URL:
  - 这表示在会话中有要检索的其他数据页。 应用程序将继续使用`nextLink` URL 发出请求, 直到`deltaLink`响应中包含 url 为止。
  - 响应包含与初始 delta 查询请求中相同的属性集。 这使您可以在启动增量循环时捕获对象的完整当前状态。

- 如果返回`deltaLink` URL:
  - 这表示没有更多有关要返回的资源的现有状态的数据。 保存并使用`deltaLink` URL, 了解下一轮中对资源的更改。
  - 您可以选择指定`Prefer:return=minimal`标头, 以便仅将自发出以来`deltaLink`发生更改的属性的响应值包括在响应值中。

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a>默认值: 返回与初始 delta 请求相同的属性

默认情况下, 请求使用`deltaLink`或`nextLink`返回在初始 delta 查询中以下列方式选择的相同属性:

- 如果属性已更改, 则新值将包含在响应中。 这包括设置为 null 值的属性。
- 如果该属性未更改, 则响应中将包含旧值。
- 如果从未设置该属性, 则根本不会将其包含在响应中。


> **注意:** 在这种情况下, 通过查看响应, 无法判断属性是否正在更改。 此外, 由于增量响应包含所有属性值 (如下面的[第二个示例](#request-2)所示), 因此它们会变大。

#### <a name="alternative-return-only-the-changed-properties"></a>替代方法: 仅返回更改的属性

添加可选请求标头- `prefer:return=minimal` -导致以下行为:

- 如果属性已更改, 则新值将包含在响应中。 这包括设置为 null 值的属性。
- 如果该属性未更改, 则该属性根本不包含在响应中。 (与默认行为不同。)

> **注意:** 可以在增量循环中的任何`deltaLink`时间点将标头添加到请求中。 标头只会影响响应中包含的一组属性, 而不会影响增量查询的执行方式。 请参阅下面的[第三个示例](#request-3)。

### <a name="example"></a>示例

#### <a name="request-1"></a>请求 1

下面是一个请求示例。 没有`$select`参数, 因此会跟踪并返回默认的属性集。
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/beta/users/delta
```

#### <a name="response-1"></a>响应 1

以下是使用`deltaLink`从查询初始化获取的响应的示例。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。 所有属性都将通过实际调用返回。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/beta/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "businessPhones": [
          "businessPhones-value"
      ],
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "jobTitle": "jobTitle-value",
      "mail": "mail-value",
      "mobilePhone": "mobilePhone-value",
      "officeLocation": "officeLocation-value",
      "preferredLanguage": "preferredLanguage-value",
      "surname": "surname-value",
      "userPrincipalName": "userPrincipalName-value",
      "id": "id-value"
    }
  ]
}
```

#### <a name="request-2"></a>请求 2

下一个示例显示了使用默认响应行为选择3个属性进行更改跟踪的初始请求:
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/beta/users/delta?$select=displayName,jobTitle,mobilePhone
```

#### <a name="response-2"></a>响应 2

以下是使用`deltaLink`从查询初始化获取的响应的示例。 请注意, 所有3个属性都包含在响应中, 并且不知道是在获取之后`deltaLink`更改的。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/beta/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "jobTitle": "jobTitle-value",
      "mobilePhone": null
    }
  ]
}
```

#### <a name="request-3"></a>请求 3

下一个示例显示了使用替代最小响应行为选择3个更改跟踪属性的初始请求:
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/beta/users/delta?$select=displayName,jobTitle,mobilePhone
Prefer: return=minimal
```

#### <a name="response-3"></a>响应 3

以下是使用`deltaLink`从查询初始化获取的响应的示例。 请注意, `mobilePhone`该属性不包括在内, 这意味着自上次增量查询以来它尚未发生更改;`displayName`并`jobTitle`将其包括在内, 这意味着它们的值已更改。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/beta/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "jobTitle": null
    }
  ]
}
```

- [使用 delta 查询跟踪 Microsoft Graph 数据中的更改](/graph/delta-query-overview)。
- [获取用户的增量更改](/graph/delta-query-users)。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-delta.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
