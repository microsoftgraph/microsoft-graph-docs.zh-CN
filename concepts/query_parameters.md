<a id="use-query-parameters-to-customize-responses" class="xliff"></a>

# 使用查询参数自定义响应

Microsoft Graph 提供可选的查询参数，可用于指定和控制响应中返回的数据量。支持以下查询参数。

|名称|说明|示例（单击示例可在 [Graph 浏览器][graph-explorer]中试调用）
|:---------------|:--------|:-------|
|[$filter](#filter)|筛选结果（行）。|[`/users?$filter=startswith(givenName,'J')`](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users?$filter=startswith(givenName,'J')&method=GET&version=v1.0)
|[$select](#select)|筛选属性（列）。|[`/users?$select=givenName,surname`](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users?$select=givenName,surname&method=GET&version=v1.0)
|[$expand](#expand)|检索相关资源。|[`/groups/{id}?$expand=members`](https://developer.microsoft.com/en-us/graph/graph-explorer?request=groups/22be6ccb-15a5-459f-94ac-d1393bdd9e66?$expand=members&method=GET&version=v1.0)
|[$orderby](#orderby)|对结果进行排序。|[`/users?$orderby=displayName,userPrincipalName desc`](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users?$orderby=displayName,userPrincipalName%20DESC&method=GET&version=v1.0)
|[$top](#top)|限制结果。通常与 `$skipToken` 配合使用。|[`/users?$top=2`](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users?$top=2&method=GET&version=v1.0)
|[$skipToken](#skiptoken)|与 `$top` 配合使用可以检索结果页。|有关示例，请参阅 $top 查询中的 `nextLink`。
|[$count](#count)|检索匹配资源的总数。|[`/me/messages?$top=2&$count=true`](https://developer.microsoft.com/en-us/graph/graph-explorer?request=me/messages?$top=2%26$count=true&method=GET&version=v1.0)
<!-- TODO: figure out whether $search is actually used
|[`$search`](#search)|A property and value pair separated by a colon.|
-->

这些参数与 [OData V4 查询语言][odata-query]兼容。

> **注意：**在 `beta` 终结点上，`$` 前缀是可选的。例如，可使用 `filter` 来代替 `$filter`。有关更多详细信息和示例，请参阅 [Microsoft Graph 中支持不含 $ 前缀的查询参数](http://dev.office.com/queryparametersinMicrosoftGraph)。

**编码查询参数：**

应对查询参数的值进行百分比编码。许多 HTTP 客户端、浏览器和工具（例如，[Graph 浏览器][graph-explorer]）都可以帮助你完成此操作。如果查询失败，可能原因之一是未正确编码查询参数的值。

未编码的 URL 如下所示：

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName, 'J')
```

正确解码的 URL 如下所示：

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName%2C+'J')
```

<a id="filter" class="xliff"></a>

## filter

`$filter` 可用于仅检索集合的一部分内容。例如，若要查找显示名称以 `J` 开头的用户，请使用 `startswith`。

[在 Graph 浏览器中试调用](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users?$filter=startswith(givenName,'J')&method=GET&version=v1.0)

**请求：**

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'J')
```

**响应：**

```json
{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users",
    "value": [
        {
            "id": "e013b9f3-a1ab-48d1-907b-e716c39d6363",
            "businessPhones": [
                "4255550100"
            ],
            "displayName": "Jan Madden",
            "givenName": "Jan",
            "jobTitle": null,
            "mail": "demo32@a830edad9050849NDA1.onmicrosoft.com",
            "mobilePhone": null,
            "officeLocation": null,
            "preferredLanguage": null,
            "surname": "Madden",
            "userPrincipalName": "demo32@a830edad9050849NDA1.onmicrosoft.com"
        },
        {
            "id": "89efe8ed-d141-4151-a3e4-570a70022dff",
            "businessPhones": [
                "+1 425 555 0109"
            ],
            "displayName": "Janet Schorr",
            "givenName": "Janet",
            "jobTitle": "Product Marketing Manager",
            "mail": "janets@a830edad9050849NDA1.onmicrosoft.com",
            "mobilePhone": null,
            "officeLocation": "18/2111",
            "preferredLanguage": null,
            "surname": "Schorr",
            "userPrincipalName": "janets@a830edad9050849NDA1.onmicrosoft.com"
        },
        ...
    ]
}
```

`$filter` 的语法非常丰富且富于表现力，其中可内置许多运算符。逻辑运算符包括等于 (`eq`)、不等于 (`ne`)、大于 (`gt`)、大于或等于 (`gte`)、且 (`and`)、或 (`or`)、非 (`not`) 等。算术运算符包括加 (`add`)、减 (`sub`) 等。字符串运算符包括包含 (`contains`)，开头为 (`startswith`) 等。lambda 运算符包括任意 (`any`) 和所有 (`all`)。有关 `$filter` 语法的其他详细信息，请参阅 [OData 协议][odata-filter]。


<a id="select" class="xliff"></a>

## select

在集合或单个实体中，若要指定返回不同于默认集的属性集，请使用 `$select` 查询参数。使用 `$select` 参数，可以选择返回的默认集的子集或超集。例如，检索邮件时，不妨选择仅返回邮件的 `from` 和 `subject` 属性。

```http
GET https://graph.microsoft.com/v1.0/me/messages?$select=from,subject
```

<!--For example, when retrieving the children of an item on a drive, you want to select that only the `name` and `size` properties of items are returned.

```http
GET https://graph.microsoft.com/v1.0/me/drive/root/children?$select=name,size
```

By submitting the request with the `$select=name,size` query string, the objects
in the response will only have those property values included.

```json
{
  "value": [
    {
      "id": "13140a9sd9aba",
      "name": "Documents",
      "size": 1024
    },
    {
      "id": "123901909124a",
      "name": "Pictures",
      "size": 1012010210
    }
  ]
}
```-->

<a id="expand" class="xliff"></a>

## expand

在 Microsoft Graph API 请求中，对参考项目的对象或集合的导航不会自动扩展。这是有意为之，因为这样可以减少网络流量以及从服务生成响应所需的时间。不过，在某些情况下，您可能希望在响应中添加这些结果。

`$expand` 查询字符串参数可用于指示 API 扩展子对象或集合，并添加这些结果。

例如，若要检索根驱动器信息和驱动器中的顶级子项，请使用 `$expand` 参数。此示例还使用 [`$select`](#select) 声明，以便仅返回子项的 `id` 和 `name` 属性。

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children($select=id,name)
```

> **注意：**最多可为请求扩展 20 个对象。此外，如果查询 [`user`](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/user) 资源，可以使用 `$expand`，一次仅获取一个子对象或集合的属性。下面的示例便是获取 `user` 对象，每个请求在 `directReports` 集合中最多扩展 20 个 `directReport` 对象：

```http
GET https://graph.microsoft.com/v1.0/users?$expand=directReports
```

其他一些资源可能也有限制，因此，请务必检查是否可能有错。

<a id="orderby" class="xliff"></a>

## orderby

若要指定从 Microsoft Graph API 返回的项的排序顺序，请使用 `$orderby` 查询参数。

例如，若要返回组织中的用户，并按显示名称进行排序，请使用以下语法：

```http
GET https://graph.microsoft.com/v1.0/users?$orderby=displayName
```

还可以按复杂类型实体进行排序。下面的示例获取邮件，然后按 `from` 属性的 `address` 字段（属于复杂类型 `emailAddress`）对这些邮件进行排序：

```http
GET https://graph.microsoft.com/v1.0/me/messages?$orderby=from/emailAddress/address
```

若要以升序或降序对结果进行排序，请向字段名称追加 `asc` 或 `desc`，并用空格隔开。例如，`?$orderby=name%20desc`。

 > **注意：**如果查询 [`user`](../api-reference/v1.0/resources/user.md) 资源，不能将 `$orderby` 与 filter 表达式结合使用。

<a id="top" class="xliff"></a>

## top

若要指定结果集中返回的项数上限，请使用 `$top` 查询参数。`$top` 查询参数可确定集合的子集。这个子集是通过仅选择集合的前 N 项而形成，其中 N 是此查询参数指定的正整数。例如，若要返回用户邮箱中的前 5 封邮件，请使用以下语法：

```http
GET https://graph.microsoft.com/v1.0/me/messages?$top=5
```

<a id="skip" class="xliff"></a>

## skip

若要设置在检索集合中的项之前要跳过的项数，请使用 `$skip` 查询参数。例如，若要返回按创建日期排序的事件，并从第 21 个事件开始返回，请使用以下语法。

```http
GET  https://graph.microsoft.com/v1.0/me/events?$orderby=createdDateTime&$skip=20
```

<a id="skiptoken" class="xliff"></a>

## skipToken

若要请求第二个和后续 Graph 数据页，请使用 `$skipToken` 查询参数。当 Graph 返回部分结果时（通常是由于服务器端分页所致），Graph 返回的 URL 中会提供 `$skipToken` 查询参数。它在集合中标识了服务器发送完结果的点，并会传递回 Graph 以指明应从哪里继续发送结果。例如，`$skipToken` 查询参数的值可以标识集合中的第 10 项，也可以标识包含 50 项的集合中的第 20 项，亦可标识集合中的其他任何位置。

一些响应中会有 `@odata.nextLink` 值。其中一些包括 `$skipToken` 值。`$skipToken` 值就像是一个标记，用于指示服务从哪里继续返回下一组结果。下面的示例展示了用户请求按 `displayName` 进行排序的响应中的 `@odata.nextLink` 值：

```json
"@odata.nextLink": "https://graph.microsoft.com/v1.0/users?$orderby=displayName&$skiptoken=X%2783630372100000000000000000000%27"
```

若要返回下一页的组织用户，请使用以下语法。

```http
GET  https://graph.microsoft.com/v1.0/users?$orderby=displayName&$skiptoken=X%2783630372100000000000000000000%27
```

<a id="count" class="xliff"></a>

## count

`$count` 查询参数可用于添加集合中的项总数，以及从 Graph 返回的数据值页，如下面的示例所示：

```http
GET  https://graph.microsoft.com/v1.0/me/contacts?$count=true
```

这将同时返回 `contacts` 集合和 `@odata.count` 属性中 `contacts` 集合中的项数。

>**注意：**[`directoryObject`](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/directoryobject) 集合不支持此查询参数。

<a id="search" class="xliff"></a>

## search

若要限制与搜索条件匹配的请求结果，请使用 `$search` 查询参数。

> **注意：**目前**只**能搜索 [message](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/message) 和 [person](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/person) 集合。`$search` 请求最多可返回 250 个结果。不能在搜索请求中使用 [`$filter`](#filter) 或 [`$orderby`](#orderby)。

搜索条件使用高级查询语法 (AQS) 进行表示。结果按邮件发送日期和时间进行排序。

可以在 `$search` 条件中对 `message` 指定下列属性：`attachments`、`bccRecipients`、`body`、`category`、`ccRecipients`、`content`、`from`、`hasAttachments`、`participants`、`receivedDateTime`、`sender`、`subject`、`toRecipients`

如果要搜索邮件并且仅指定了一个值，那么会根据默认搜索属性 `from`、`subject` 和 `body` 进行搜索。

下面的示例返回登录用户收件箱中在三个默认搜索属性的任意一个中包含“pizza”的的所有邮件：

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="pizza"
```

下一个示例在用户收件箱中搜索从指定电子邮件地址发送的所有邮件：

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="from:help@contoso.com"
```

[graph-explorer]: https://graph.microsoft.io/en-us/graph-explorer
[odata-filter]: http://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752358
[odata-query]: http://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752356
