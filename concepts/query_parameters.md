# <a name="use-query-parameters-to-customize-responses"></a>使用查询参数自定义响应

Microsoft Graph 提供可选的查询参数，可用于指定和控制响应中返回的数据量。支持以下查询参数。

>**注意：**单击示例以在 [Graph 浏览器][graph-explorer]中试调用。

| 名称                     | 说明 | 示例
|:-------------------------|:------------|:---------|
| [$count](#count-parameter)         | 检索匹配资源的总数。 | [`/me/messages?$top=2&$count=true`][count-example]
| [$expand](#expand-parameter)       | 检索相关资源。|[`/groups?$expand=members`][expand-example]
| [$filter](#filter-parameter)       | 筛选结果（行）。|[`/users?$filter=startswith(givenName,'J')`][filter-example]
| [$format](#format-parameter)       | 返回指定媒体格式的结果。|[`/users?$format=json`][format-example]
| [$orderby](#orderby-parameter)     | 对结果进行排序。|[`/users?$orderby=displayName desc`][orderby-example]
| [$search](#search-parameter)       | 根据搜索条件返回结果。目前支持用于 **messages** 和 **person** 集合。|[`/me/messages?$search=pizza`][search-example]
| [$select](#select-parameter)       | 筛选属性（列）。|[`/users?$select=givenName,surname`][select-example]
| [$skip](#skip-parameter)           | 对结果集建立索引。一些 API 也使用它来实现分页，并且可以与 `$top` 一起使用来手动对结果分页。 | [`/me/messages?$skip=11`][skip-example]
| [$skipToken](#skiptoken-parameter) | 从跨多页的结果集中检索下一页结果。（但某些 API 改为使用 `$skip`。） | `/users?$skiptoken=X%274453707402000100000017...`|
| [$top](#top-parameter)             | 设置结果的页面大小。 |[`/users?$top=2`][top-example]



这些参数与 [OData V4 查询语言][odata-query]兼容。 并非所有的 Microsoft Graph API 都支持所有参数，而对 `v1.0` 和 `beta` 终结点的支持可能会显著不同。 

> **注意：**在 `beta` 终结点上，`$` 前缀是可选的。例如，可使用 `filter` 来代替 `$filter`。有关更多详细信息和示例，请参阅 [Microsoft Graph 中支持不含 $ 前缀的查询参数](http://dev.office.com/queryparametersinMicrosoftGraph)。

## <a name="encoding-query-parameters"></a>编码的查询参数

应对查询参数的值进行百分比编码。 许多 HTTP 客户端、浏览器和工具（例如，[Graph 浏览器][graph-explorer]）都可以帮助用户完成此操作。 如果查询失败，可能原因之一是未正确编码查询参数值。

未编码的 URL 如下所示：

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName, 'J')
```

正确解码的 URL 如下所示：

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName%2C+'J')
```

## <a name="count-parameter"></a>count 参数

使用 `$count` 查询参数以包括集合中项总数的计数，以及从 Microsoft Graph 返回的数据值页。 

例如，下面的请求返回当前用户的 **contact** 集合，以及 `@odata.count` 属性中 **contact** 集合内的项数。

```http
GET  https://graph.microsoft.com/v1.0/me/contacts?$count=true
```

[在 Graph 浏览器中试调用](https://developer.microsoft.com/graph/graph-explorer?request=me/contacts?$count=true&method=GET&version=v1.0)


>**注意：**派生自 [directoryObject](../api-reference/v1.0/resources/directoryobject.md) 的资源集合（如 [user](../api-reference/v1.0/resources/user.md) 或 [group](../api-reference/v1.0/resources/group.md) 集合）不支持 `$count`。

## <a name="expand-parameter"></a>expand 参数

许多 Microsoft Graph 资源都会公开资源的已声明属性以及与其他资源的关系。 这些关系也称为引用属性或导航属性，它们可以引用单个资源或资源集合。 例如，用户的邮件文件夹、管理者和直接下属都将作为关系公开。 

通常情况下，可以在单个请求中查询资源属性或其关系之一，但不能同时查询。可以使用 `$expand` 查询字符串参数以包含结果中单个关系（导航属性）引用的扩展资源或集合。

以下示例在驱动器中获取根驱动器信息以及顶级子项：

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children
```

[在 Graph 浏览器中试调用](https://developer.microsoft.com/graph/graph-explorer?request=me/drive/root?$expand=children&method=GET&version=v1.0)

使用一些资源集合，还可以添加 `$select` 参数，指定要在扩展资源中返回的属性。下面的示例执行与上一示例几乎相同的查询，不同之处在于使用 [`$select`](#select-parameter) 语句将为扩展子项返回的属性限制为 **id** 和 **name** 属性。

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children($select=id,name)
```

[在 Graph 浏览器中试用][expand-example]

> **注意：**并不是所有关系和资源都支持 `$expand` 查询参数。例如，可以扩展用户的 **directReports**、**manager** 和 **memberOf** 关系，但无法扩展其 **events**、**messages** 或 **photo** 关系。并非所有资源或关系都支持对扩展项使用 `$select`。 
> 
> 使用从 [directoryObject](../api-reference/v1.0/resources/directoryobject.md) 派生的 Azure AD 资源（如[user](../api-reference/v1.0/resources/user.md) 和 [group](../api-reference/v1.0/resources/group.md)），`$expand` 仅支持 `beta`，并且通常最多为扩展关系返回 20 个项。

## <a name="filter-parameter"></a>filter 参数

使用 `$filter` 查询参数，以仅检索集合的子集。 

例如，若要查找显示名称以子母“J”开头的用户，请使用 `startswith`。

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'J')
```

[在 Graph 浏览器中试用][filter-example]

对 `$filter` 运算符的支持因 Microsoft Graph API 而异。 通常支持下列逻辑运算符： 

- 等于 (`eq`)
- 不等于 (`ne`)
- 大于 (`gt`)
- 大于或等于 (`ge`)
- 小于 (`lt`)，小于或等于 (`le`)
- 且 (`and`)
- 或 (`or`)
- 非 (`not`)
 
通常支持 `startswith` 字符串运算符。 某些 API 支持 `any` lambda 运算符。 有关一些用法示例的信息，请参阅下表。 有关 `$filter` 语法的其他详细信息，请参阅 [OData 协议][odata-filter]。  

下表显示使用 `$filter` 查询参数的一些示例。

> **注意：**单击示例以在 [Graph 浏览器][graph-explorer]中试调用。

| 说明 | 示例
|:------------|:--------|
| 跨多个属性搜索名为 Mary 的用户。 | [`https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'mary') or startswith(givenName,'mary') or startswith(surname,'mary') or startswith(mail,'mary') or startswith(userPrincipalName,'mary')`](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(displayName,'mary')+or+startswith(givenName,'mary')+or+startswith(surname,'mary')+or+startswith(mail,'mary')+or+startswith(userPrincipalName,'mary')&method=GET&version=v1.0) 
| 获取 2017 年 7 月 1 日之后开始的所有登录用户的事件。 | [`https://graph.microsoft.com/v1.0/me/events?$filter=start/dateTime ge '2017-07-01T08:00'`](https://developer.microsoft.com/graph/graph-explorer?request=me/events?$filter=start/dateTime+ge+'2017-07-01T08:00'&method=GET&version=v1.0) 
| 获取登录用户收到的来自特定地址的所有电子邮件。 | [`https://graph.microsoft.com/v1.0/me/messages?$filter=from/emailAddress/address eq 'someuser@example.com'`](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=from/emailAddress/address+eq+'someuser@.com'&method=GET&version=v1.0) 
| 获取登录用户在 2017 年 4 月收到的所有电子邮件。 | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=ReceivedDateTime ge 2017-04-01 and receivedDateTime lt 2017-05-01`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=ReceivedDateTime+ge+2017-04-01+and+receivedDateTime+lt+2017-05-01&method=GET&version=v1.0) 
| 获取登录用户收件箱中的所有未读邮件。 | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=isRead eq false`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=isRead+eq+false&method=GET&version=v1.0) 
| 列出组织中的所有 Office 365 组。 | [`https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')`](https://developer.microsoft.com/graph/graph-explorer?request=groups?$filter=groupTypes/any(c:c+eq+'Unified')&method=GET&version=v1.0) 

> **注意：**Azure AD 资源不支持以下 `$filter` 运算符：`ne`、`gt`、`ge`、`lt`、`le` 和 `not`。所有 Microsoft Graph 资源目前均不支持 `contains` 字符串运算符。

## <a name="format-parameter"></a>format 参数

使用 `$format` 查询参数，指定 Microsoft Graph 返回的项的媒体格式。

例如，下面的请求以 json 格式返回组织中的用户：

```http
GET https://graph.microsoft.com/v1.0/users?$format=json
```

[在 Graph 浏览器中试用][format-example]

> **注意：**`$format` 查询参数支持许多格式（例如，atom、xml 和 json），但可能无法返回所有格式的结果。

## <a name="orderby-parameter"></a>orderby 参数

使用 `$orderby` 查询参数指定从 Microsoft Graph 返回的项的排序顺序。

例如，以下请求返回按用户显示名称进行排序的组织中的用户：

```http
GET https://graph.microsoft.com/v1.0/users?$orderby=displayName
```
[在 Graph 浏览器中试用][orderby-example]

还可以按复杂类型实体进行排序。下面的请求获取邮件，并按 **from** 属性的 **address** 字段（复杂类型为 **emailAddress**）进行排序：

```http
GET https://graph.microsoft.com/v1.0/me/messages?$orderby=from/emailAddress/address
```
[在 Graph 浏览器中试调用](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/address&method=GET&version=v1.0)

若要以升序或降序对结果进行排序，请向字段名称追加 `asc` 或 `desc`，并用空格隔开。例如，`?$orderby=name%20desc`。

通过一些 API，可以对多个属性的结果进行排序。 例如，以下请求首先按发件人名称以降序（Z 到 A）排序用户收件箱中的邮件，然后按主题以升序（默认）排序邮件。

```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/Inbox/messages?$orderby=from/emailAddress/name desc,subject
```

[在 Graph 浏览器中试调用](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/name%20desc,subject&method=GET&version=v1.0)


 > **注意：**使用从 [directoryObject](../api-reference/v1.0/resources/directoryobject.md) 派生的 Azure AD 资源（如 [user](../api-reference/v1.0/resources/user.md) 和 [group](../api-reference/v1.0/resources/group.md)），则不能合并 `$orderby` 与 `$filter` 表达式。 

## <a name="search-parameter"></a>search 参数

使用 `$search` 查询参数限制与搜索条件匹配的请求结果。

> **注意：**目前**只**能搜索 [message](../api-reference/v1.0/resources/message.md) 和 [person](../api-reference/v1.0/resources/person.md) 集合。`$search` 请求最多可返回 250 个结果。不能在搜索请求中使用 [`$filter`](#filter-parameter) 或 [`$orderby`](#orderby-parameter)。

### <a name="using-search-on-message-collections"></a>对 message 集合使用 $search

Office 365 应用（如 Outlook 和 SharePoint）支持使用关键字查询语言 (KQL) 语法执行搜索。 这就方便常见发现域使用数据存储。 

搜索 message 集合时，结果按邮件发送日期和时间进行排序。 

可以在 `$search` 条件中对 **message** 指定下列属性：

- **attachments**
- **bccRecipients**
- **body**
- **category**
- **ccRecipients**
- **content**
- **from**
- **hasAttachments**
- **participants**
- **receivedDateTime**
- **sender**
- **subject**
- **toRecipients**

如果搜索邮件且仅指定值，将根据默认搜索属性 **from**、**subject** 和 **body** 进行搜索。

下面的示例返回登录用户收件箱中在三个默认搜索属性的任意一个中包含“pizza”的所有邮件：

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="pizza"
```

[在 Graph 浏览器中试用][search-example]

下一个示例在用户收件箱中搜索从指定电子邮件地址发送的所有邮件：

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="from:help@contoso.com"
```
若要详细了解 KQL（如语法、支持的运算符和搜索提示），请参阅以下文章：

- [关键字查询语言 (KQL) 语法参考](https://docs.microsoft.com/zh-CN/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference)

- 
  [Exchange 2016 中的就地电子数据展示的邮件属性和搜索运算符](https://technet.microsoft.com/en-us/library/dn774955(v=exchg.160).aspx)

### <a name="using-search-on-person-collections"></a>对 person 集合使用 $search

可以使用 Microsoft Graph People API 检索与用户相关度最高的人员。相关性由用户的通信和协作模式及业务关系决定。People API 支持 `$search` 查询参数。

人员搜索就是按 [person](../api-reference/v1.0/resources/person.md) 资源的 **displayName** 和 **emailAddress** 属性进行搜索。 搜索实现模糊匹配算法。 它们根据完全匹配以及搜索意图推断返回结果。 例如，假设用户显示名称为“Tyler Lee”，电子邮件地址为 tylerle@example.com，用户位于登录用户的 **people** 集合中。 所有以下搜索将返回包含 Tyler 的结果。

```http
GET https://graph.microsoft.com/v1.0/me/people?$search=tyler                //matches both Tyler's name and email
GET https://graph.microsoft.com/v1.0/me/people?$search=tylerle              //matches Tyler's email
GET https://graph.microsoft.com/v1.0/me/people?$search="tylerle@example.com"  //matches Tyler's email. Note the quotes to enclose '@'.
GET https://graph.microsoft.com/v1.0/me/people?$search=tiler                //fuzzy match with Tyler's name 
GET https://graph.microsoft.com/v1.0/me/people?$search="tyler lee"          //matches Tyler's name. Note the quotes to enclose the space.
```

还可以搜索对特定主题感兴趣的人员。基于从用户的邮件对话派生的推断来执行搜索。例如，以下搜索将返回与登录用户相关的人员集合，在与该用户进行通信时，他表现出了对披萨的兴趣。请注意，搜索短语用引号括起来。

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="topic:pizza"                
```

最后，可以通过组合两种类型的搜索表达式，在同一请求中合并人员搜索和主题搜索。

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="tyl topic:pizza"                
```

此请求主要进行两次搜索：对登录用户的相关人员的 **displayName** 和 **emailAddress** 属性进行模糊搜索，以及对用户的相关人员进行“pizza”主题搜索。 然后，对结果进行排名、排序并返回。 请注意，该搜索没有限制；可能会得到包含模糊匹配“tyl”的人员的结果和/或对“披萨”感兴趣的人员的结果。

若要了解有关 People API 的详细信息，请参阅[获取相关人员的信息](./people_example.md)。  

## <a name="select-parameter"></a>select 参数

使用 `$select` 查询参数返回一组不同于单个资源的默认集或资源集合的属性。 使用 $select，可以指定默认属性的子集或超集。

例如，检索登录用户的邮件时，可以指定仅返回 **from** 和 **subject** 属性：

```http
GET https://graph.microsoft.com/v1.0/me/messages?$select=from,subject
```

[在 Graph 浏览器中试用][select-example]

> **重要说明：**一般来说，建议使用 `$select` 将查询返回的属性限制为应用所需的属性。 这对于可能返回大型结果集的查询尤为有用。 限制每行返回的属性将减少网络负载并帮助提升应用的性能。
>
> 在 `v1.0` 中，从 [directoryObject](../api-reference/v1.0/resources/directoryobject.md) 派生的一些 Azure AD 资源（如 [user](../api-reference/v1.0/resources/user.md) 和 [group](../api-reference/v1.0/resources/group.md)）在读取时返回受限的默认属性子集。对于这些资源，必须使用 `$select` 将属性返回到默认集之外。  

## <a name="skip-parameter"></a>skip 参数

使用 `$skip` 查询参数设置要在集合开头跳过的项数。例如，以下请求返回按照创建日期排序的用户的事件，从集合中的第 21 个事件开始：

```http
GET  https://graph.microsoft.com/v1.0/me/events?$orderby=createdDateTime&$skip=20
```
[在 Graph 浏览器中试用][skip-example]

> **注意：**一些 Microsoft Graph API 使用 `$skip` 实现分页，如 Outlook 邮件和日历（**message**、**event** 和 **calendar**）。 当查询结果跨多个页面时，这些 API 会返回 `@odata:nextLink` 属性，具有包含 `$skip` 参数的 URL。 可以使用此 URL 返回下一页结果。 若要了解详细信息，请参阅[分页](./paging.md)。

## <a name="skiptoken-parameter"></a>skipToken 参数

由于服务器端分页或由于使用 [`$top`](#top-parameter) 参数来限制响应的页面大小，致使一些请求返回多页数据。许多 Microsoft Graph API 使用 `skipToken` 查询参数来引用结果的后续页面。`$skiptoken` 参数包含引用下一页结果的不透明令牌，并在响应的 `@odata.nextLink` 属性中提供的 URL 中返回。若要了解详细信息，请参阅[分页](./paging.md)。


## <a name="top-parameter"></a>top 参数

使用 `$top` 查询参数指定结果集的页面大小。 

如果结果集中还剩余多个项目，则响应正文将包含 `@odata.nextLink` 参数。 此参数包含可用于获取下一页结果的 URL。 若要了解详细信息，请参阅[分页](./paging.md)。 

例如，以下请求返回用户邮箱中的前 5 封邮件：

```http
GET https://graph.microsoft.com/v1.0/me/messages?$top=5
```

[在 Graph 浏览器中试用][top-example]


## <a name="error-handling-for-query-parameters"></a>查询参数的错误处理

如果不支持指定的查询参数，某些请求将返回错误消息。例如，不能对 `user/photo` 关系使用 `$expand`。 

```http
https://graph.microsoft.com/beta/me?$expand=photo
```

```json
{
    "error":{
        "code":"ExpandNotSupported",
        "message":"Expand is not allowed for property 'Photo' according to the entity schema.",
        "innerError":{
            "request-id":"1653fefd-bc31-484b-bb10-8dc33cb853ec",
            "date":"2017-07-31T20:55:01"
        }
    }
}
```

但是，值得注意的是请求中指定的查询参数可能会自行失败。 不支持的查询参数以及不支持的查询参数组合的情况就是如此。 在这些情况下，应检查请求返回的数据，以确定指定的查询参数是否具有所需的效果。 

[graph-explorer]: https://developer.microsoft.com/graph/graph-explorer
[odata-filter]: http://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752358
[odata-query]: http://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752356
[count-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$top=2%26$count=true&method=GET&version=v1.0
[expand-example]: https://developer.microsoft.com/graph/graph-explorer?request=groups$expand=members&method=GET&version=v1.0
[filter-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(givenName,'J')&method=GET&version=v1.0
[format-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$format=json&method=GET&version=v1.0
[orderby-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$orderby=displayName%20DESC&method=GET&version=v1.0
[search-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=pizza&method=GET&version=v1.0
[select-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$select=givenName,surname&method=GET&version=v1.0
[skip-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$skip=11&method=GET&version=v1.0
[top-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$top=2&method=GET&version=v1.0


