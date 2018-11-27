# <a name="user-delta"></a>user: delta

获取新创建、 更新或删除用户，而无需执行的整个用户集的完全读取。 有关详细信息，请参阅[修订](../../../concepts/delta_query_overview.md)。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。


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

跟踪中用户的更改会导致一个或多个**增量**函数调用的往返。 如果您使用任何查询参数 (以外的其他`$deltatoken`和`$skiptoken`)，则必须指定该初始**增量**请求中。 Microsoft Graph 自动将任何指定的参数编码为的令牌部分`nextLink`或`deltaLink`响应中提供的 URL。

只需预先指定所需的任何查询参数一次。

在后续请求中，可以复制并应用之前响应中返回的 `nextLink` 或 `deltaLink` URL，因为此 URL 已包含所需的编码参数。

| 查询参数      | 类型   |说明|
|:---------------|:--------|:----------|
| $deltatoken | string | 对同一个用户集合之前的 **delta** 函数调用的 `deltaLink` URL 中返回的[状态令牌](../../../concepts/delta_query_overview.md)，指示该组更改跟踪的完成状态。将此令牌包含在对该集合的下一组更改追踪的首次请求中，并保存和应用整个 `deltaLink` URL。|
| $skiptoken | string | 对之前的 **delta** 函数调用的 `nextLink` URL 中返回的[状态令牌](../../../concepts/delta_query_overview.md)，指示同一个用户集合中有进一步的更改需要追踪。 |

### <a name="odata-query-parameters"></a>OData 查询参数

此方法支持可选的 OData 查询参数，以帮助自定义响应。

- 像在任何 GET 请求中一样，你可以使用 `$select` 查询参数以仅指定获取最佳性能所需的属性。始终返回 *id* 属性。
- 支持是有限的`$filter`:
  - 唯一支持的 `$filter` 表达式用于跟踪对特定对象 `$filter=id+eq+{value}` 的更改。 可以筛选多个对象。 例如，`https://graph.microsoft.com/v1.0/users/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`。 筛选对象不能超出 50 个。

## <a name="request-headers"></a>请求标头
| 名称       | 说明|
|:---------------|:----------|
| Authorization  | 持有者&lt;令牌&gt;|
| Content-Type  | application/json |
| Prefer | 返回 = 最少 <br><br>指定与请求使用此标头`deltaLink`会返回自上次循环后已更改的对象属性。 可选。 |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

### <a name="response"></a>响应

如果成功，此方法返回`200 OK`响应正文中的响应代码和[用户](../resources/user.md)集合的对象。 响应还包括`nextLink`URL 或`deltaLink`URL。

- 如果`nextLink`返回 URL:
  - 这指示有会话中检索的数据的其他页面。 应用程序将继续进行请求使用`nextLink`直到 URL `deltaLink` URL 包含响应中。
  - 响应包含一组相同的属性，如初始增量查询请求中所示。 这样，您可以在启动增量周期捕获对象的完整当前状态。

- 如果`deltaLink`返回 URL:
  - 这表明没有更多有关要返回的资源的现有状态数据。 保存并使用`deltaLink`URL 以了解如何更改为下一轮中的资源。
  - 您可以选择指定`Prefer:return=minimal`标头，以响应时间以来已经更改的属性值中包括`deltaLink`颁发。

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a>默认值： 返回作为初始增量请求的同一属性

默认情况下，请求使用`deltaLink`或`nextLink`与选定初始增量查询中相同的属性返回以下方式：

- 如果该属性已更改的 JSON 响应中返回的属性。
- 如果设置了为空值的属性，返回属性值为 null。
- 如果具有未更改的属性，返回的值为 null。

> **注意：** 具有上述行为，它不能区分未更改的属性和一个已更改为`null`值。 请参阅下面的[第二个示例](#request-2)。 如果这是重要，我们建议使用下节所述的替代行为。

#### <a name="alternative-return-only-the-changed-properties"></a>可选： 仅返回已更改的属性

添加可选请求标头中的`prefer:return=minimal`-导致以下行为：

- 如果该属性已更改的 JSON 响应中返回的属性。
- 如果设置了为空值的属性，返回属性值为 null。
- 如果具有未更改的属性，不包括属性中的 JSON 响应。 （不同于默认行为。）

> **注意：** 标头可以添加到`deltaLink`任何时间点的增量周期中的请求。 头只影响的响应中包括的属性集，而不会影响如何执行增量查询。 请参阅下面的[第三个示例](#request-3)。

### <a name="example"></a>示例

#### <a name="request-1"></a>请求 1

下面展示了示例请求。 没有任何`$select`参数，以便跟踪和返回一组默认属性。
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/users/delta
```

#### <a name="response-1"></a>响应 1

以下是时使用的响应示例`deltaLink`获取从查询初始化。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
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

下面的示例演示选择 3 属性更改跟踪具有默认响应行为的初始请求：
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/users/delta?$select=displayName,jobTitle,mobilePhone
```

#### <a name="response-2"></a>响应 2

以下是时使用的响应示例`deltaLink`获取从查询初始化。 请注意，`jobTitle`和`mobilePhone`具有的值`null`这意味着它们可能已不发生更改或已设置为空值。

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "jobTitle": null,
      "mobilePhone": null
    }
  ]
}
```

#### <a name="request-3"></a>请求 3

下面的示例演示选择 3 属性更改跟踪具有最少的替代响应行为的初始请求：
<!-- {
  "blockType": "request",
  "name": "user_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/users/delta?$select=displayName,jobTitle,mobilePhone
Prefer: return=minimal
```

#### <a name="response-3"></a>响应 3

以下是时使用的响应示例`deltaLink`获取从查询初始化。 请注意，`mobilePhone`属性不包括在内，这意味着它未更改以来上一次增量查询;`displayName`和`jobTitle`是包含已更改其值的方法。

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "jobTitle": null
    }
  ]
}
```

- [使用增量查询来跟踪 Microsoft Graph 数据中的更改](../../../concepts/delta_query_overview.md)。
- [获取用户的增量更改](../../../concepts/delta_query_users.md)。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->