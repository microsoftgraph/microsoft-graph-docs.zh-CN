---
title: 'group: delta'
description: 获取新创建、更新或删除的组，包括组成员身份更改，而无需执行整个组集合的完整读取。 有关详细信息，请参阅使用增量查询。
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: e5fabcc982c676ba322d92e5abf6d1fb40944a13
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52681793"
---
# <a name="group-delta"></a>group: delta

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取新创建、更新或删除的组，包括组成员身份更改，而无需执行整个组集合的完整读取。 有关详细信息 [，请参阅使用增量](/graph/delta-query-overview) 查询。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | GroupMember.Read.All、Group.Read.All、Directory.Read.All、Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All  |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

为开始跟踪更改，请在组资源上发出包含 delta 函数的请求。

<!-- { "blockType": "ignored" } -->

```http
GET /groups/delta
```

## <a name="query-parameters"></a>查询参数

跟踪组中的更改会触发一个或多个 **delta** 函数调用。如果使用任何查询参数（而不是 `$deltatoken` 和 `$skiptoken`），必须在初始 **delta** 请求中指定它。Microsoft Graph 会自动将任何指定参数编码为响应中返回的 `nextLink` 或 `deltaLink` URL 的令牌部分。

只需预先指定所需的任何查询参数一次。

在后续请求中，可以复制并应用之前响应中返回的 `nextLink` 或 `deltaLink` URL，因为此 URL 已包含所需的编码参数。

| 查询参数 | 类型  |说明|
|:---------------|:--------|:----------|
| $deltatoken | string | 对同一个组集合之前的 **delta** 函数调用的 `deltaLink` URL 中返回的 [状态令牌](/graph/delta-query-overview)，指示该组更改跟踪的完成状态。将此令牌包含在对该集合的下一组更改追踪的首次请求中，并保存和应用整个 `deltaLink` URL。|
| $skiptoken | string | 对之前的 **delta** 函数调用的 `nextLink` URL 中返回的 [状态令牌](/graph/delta-query-overview)，指示同一个组集合中有进一步的更改需要追踪。 |

### <a name="odata-query-parameters"></a>OData 查询参数

此方法支持可选的 OData 查询参数来帮助自定义响应。

- 像在任何 GET 请求中一样，你可以使用 `$select` 查询参数以仅指定获取最佳性能所需的属性。始终返回 *id* 属性。
- 可以使用 获取 `$select=members` 成员身份更改。 您还可以通过选择 **directoryObject** 集合类型的任何 [](../resources/group.md#relationships)组关系来跟踪其他更改（如所有权等）。
- 提供对 `$filter` 的有限支持：
  - 唯一支持的 `$filter` 表达式用于跟踪对特定对象 `$filter=id+eq+{value}` 的更改。 可以筛选多个对象。 例如，`https://graph.microsoft.com/beta/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`。 筛选对象不能超出 50 个。

## <a name="request-headers"></a>请求标头

| 名称       | 说明|
|:---------------|:----------|
| Authorization  | 持有者&lt;令牌&gt;|
| Content-Type  | application/json |
| Prefer | return=minimal <br><br>在使用 `deltaLink` 的请求中执行此标头将仅返回自上一轮之后发生更改的对象属性。 可选。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

### <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和[组](../resources/group.md)集合对象。 该响应还包括一个状态令牌，即 `nextLink` URL 或 `deltaLink` URL。

- 如果返回 `nextLink`URL：
  - 这表示绘画中存在要检索的其他数据页面。 应用程序继续使用 `nextLink` URL 发出请求，直到响应中包含 `deltaLink` URL。
  - 响应包含与初始 Delta 查询请求相同的属性集。 这使你能够在发起 Delta 循环时捕获对象当前的完整状态。

- 如果返回 `deltaLink`URL：
  - 这表示未返回关于资源现有状态的更多数据。 保存并使用 `deltaLink` URL 来了解下一轮资源更改。
  - 只有对于在签发 `deltaLink` 之后更改的属性，你才可以选择指定 `Prefer:return=minimal` 标头以包含在响应值中。

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a>默认：返回与初始 Delta 请求相同的属性

默认情况下，使用 `deltaLink` 或 `nextLink` 的请求将通过以下方式返回与初始 Delta 查询中选择的相同属性：

- 如果属性已更改，则新值将包括在响应中。 这包括设为 Null 值的属性。
- 如果属性未更改，则旧值将包括在响应中。
- 如果之前从未设置属性，则它不会包括在响应中。


> **注意：** 如果出现此行为，那么通过查看响应无法区分属性是否已更改。 此外，Delta 响应往往过大，因为它们包含所有属性值，如下面的[第二个示例](#request-2)所示。

#### <a name="alternative-return-only-the-changed-properties"></a>备用：仅返回更改的属性

添加可选请求标头 - `prefer:return=minimal` - 将导致出现以下行为：

- 如果属性已更改，则新值将包括在响应中。 这包括设为 Null 值的属性。
- 如果尚未更改属性，则该属性不会包括在响应中。（不同于默认行为。）

> **注意：** 可以在 Delta 循环中的任何时间点将标头添加到 `deltaLink` 请求中。 标头仅影响响应中包含的属性集，它不会影响执行 Delta 查询的方式。 请参阅下面的[第三个示例](#request-3)。

### <a name="example"></a>示例

#### <a name="request-1"></a>请求 1

下面展示了示例请求。 没有 `$select` 参数，因为将跟踪并返回默认的属性集。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/delta
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response-1"></a>响应 1

以下示例所示为使用从查询初始化获得的 `deltaLink` 时的响应。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
>
> 请注意存在包含 *members@delta* 成员对象的 ID 的 members@delta 属性。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups","@odata.nextLink":"https://graph.microsoft.com/beta/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvY1FSSc_",
  "value":[
    {
      "classification": "classification-value",
      "createdDateTime":"datetime-value",
      "description":"Test group 1",
      "displayName":"TestGroup1",
      "groupTypes": [
        "groupTypes-value"
      ],
      "mail": "mail-value",
      "members@delta": [
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "693acd06-2877-4339-8ade-b704261fe7a0"
               },
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "49320844-be99-4164-8167-87ff5d047ace"
               }
      ]
    }
  ]
}
```

#### <a name="request-2"></a>请求 2

下一个示例所示为通过默认响应行为选择 3 种更改跟踪属性时的初始请求：

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_delta_with_selelct"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/delta?$select=displayName,description,mailNickname
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-delta-with-selelct-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-delta-with-selelct-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-delta-with-selelct-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-delta-with-selelct-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response-2"></a>响应 2

以下示例所示为使用从查询初始化获得的 `deltaLink` 时的响应。 请注意，所有 3 种属性将包括在响应中，并且无法知道在获得 `deltaLink` 之后发生更改的属性。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/beta/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "description": null,
      "mailNickname": "mailNickname-value"
    }
  ]
}
```

#### <a name="request-3"></a>请求 3

下一个示例所示为通过备用最小响应行为选择 3 种更改跟踪属性时的初始请求：

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_delta_minimal"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/delta?$select=displayName,description,mailNickname
Prefer: return=minimal
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-delta-minimal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-delta-minimal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-delta-minimal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-delta-minimal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response-3"></a>响应 3

以下示例所示为使用从查询初始化获得的 `deltaLink` 时的响应。 请注意，`mailNickname` 属性不包括在内，这意味着它在上一轮 Delta 查询之后未发生更改；并且 `displayName` 和 `description` 将包括在内，这意味着其值已发生更改。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/beta/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "description": null
    }
  ]
}
```

## <a name="see-also"></a>另请参阅

- [使用 Delta 查询跟踪 Microsoft Graph 数据更改](/graph/delta-query-overview)。
- [获取组的增量更改](/graph/delta-query-groups)。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "group: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


