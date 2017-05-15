# <a name="microsoft-graph-optional-query-parameters"></a>Microsoft Graph 可选的查询参数
Microsoft Graph 提供多个可选查询参数，您可以用来指定和控制响应中返回的数据量。Microsoft Graph 支持以下查询选项。 

|名称|值|说明|
|:---------------|:--------|:-------|
|$search|string|由冒号分隔的属性和值对。 | 
|$select|string|要在响应中添加的属性（以逗号分隔的列表）。|
|$expand|string|要在响应中扩展和添加的关系（以逗号分隔的列表）。  |
|$orderby|string|用于在响应集合中对项目进行排序的属性（以逗号分隔的列表）。|
|$filter|string|根据一组条件筛选响应。|
|$top|int|要在结果集中返回的项目数。|
|$skip|int|在结果集中跳过的项目数。|
|$skipToken|string|给用于获取下一个结果集的令牌进行分页。|
|$count|none|一个集合以及集合中的项目数。|

这些参数均与 [OData V4 查询语言](http://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752356) 兼容。

>  **注意**：在 Microsoft Graph **beta** 终结点中，可以省略 **$** 前缀，以获得更简单的体验。例如，作为 **$expand** 的替代，可以使用 **expand**。有关更多详细信息和示例，请参阅 [在 Microsoft Graph 中支持没有 $ 前缀的查询参数](http://dev.office.com/queryparametersinMicrosoftGraph)。  

**编码的查询参数**

- 如果您尝试在 [Microsoft Graph 资源管理器](https://graph.microsoft.io/en-us/graph-explorer#)中查询参数，您可以只复制和粘贴以下示例，无需将任何 URL 编码应用到查询字符串。以下示例在 Graph 资源管理器中运行正常，无需对空格和引号字符进行编码：
```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=from/emailAddress/address eq 'jon@contoso.com'
``` 
- 一般情况下，在应用中指定查询参数时，请确保相应的编码字符[保留 URI 中的特殊含义](https://tools.ietf.org/html/rfc3986#section-2.2)。例如，在最后一个示例中对空格和引号字符进行编码，如下所示：
```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=from/emailAddress/address%20eq%20%27jon@contoso.com%27
```


### <a name="search"></a>$search
若要限制匹配搜索条件的请求结果，则使用 **$search** 查询参数。 

>  **注意**：目前可以对[邮件](../api-reference/v1.0/resources/message.md)和[人员](../api-reference/beta/resources/person.md)的集合使用 **$search**，但不可以对[联系人](../api-reference/v1.0/resources/contact.md)或[事件](../api-reference/v1.0/resources/event.md)集合使用。**$search** 请求可返回多达 250 个结果。不能在 **$search** 请求中使用 **$filter** 或 **$orderby**。

搜索条件使用高级查询语法 (AQS) 表示。 

**对邮件应用 $search**

搜索结果按发送邮件的日期和时间排序。

可以在 **$search** 条件中指定**邮件**的以下属性：**attachments**、 **bccRecipients**、 **body**、 **category**、 **ccRecipients**、 **content**、 **from**、 **hasAttachments**、 **participants**、 **receivedDateTime**、 **sender**、 **subject**、 **toRecipients**

如果对邮件进行搜索且仅指定了一个值，则基于默认的搜索属性 **from**、**subject** 和 **body** 进行搜索。

以下示例返回已登录用户收件箱中的所有邮件，且用户收件箱在三个默认搜索属性的任意一个中包含“pizza”： 

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="pizza"
```

下一个示例搜索用户收件箱中从指定电子邮件地址发送的所有邮件：

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="from:help@contoso.com"
```



### <a name="select"></a>$select
若要指定返回一组不同于 Graph 提供的默认集的属性集，请使用 **$select** 查询选项。**$Select** 选项允许选择返回的默认集的子集或超集。例如，在检索邮件时，可能希望选择仅返回邮件的 **发件人** 和 **主题** 属性。

```http
GET https://graph.microsoft.com/v1.0/me/messages?$select=from,subject
```

<!--For example, when retrieving the children of an item on a drive, you want to select that only the **name** and **size** properties of items are returned.

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

## <a name="expand"></a>$expand

在 Microsoft Graph API 请求中，对参考项目的对象或集合的导航不会自动扩展。这是有意为之，因为这样可以减少网络流量以及从服务生成响应所需的时间。不过，在某些情况下，您可能希望在响应中添加这些结果。

可以使用 **$expand** 查询字符串参数，指示 API 扩展子对象或集合，并添加这些结果。

例如，若要检索根驱动器信息和驱动器中的顶级子项目，请使用 **$expand** 参数。此示例还使用 **$select** 声明，以便仅返回子项的 ID 和 name 属性。

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children($select=id,name)
```

>  **注意**：请求最多可扩展 20 个对象。 

> 此外，如果您要查询[用户](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/user)资源，您可以使用 **$expand**，一次仅可获取一个子对象 或集合的属性。 

以下示例获取**用户**对象时，每个在 **directReports** 扩展集合中都有多达 20 个 **directReport** 对象：
```http
GET https://graph.microsoft.com/v1.0/users?$expand=directReports
```
某些其他资源可能也会存在限制，因此务必检查可能存在的错误。


<!---The following shows a sample result that is returned in the response body.-->


## <a name="orderby"></a>$orderby

若要指定从 Microsoft Graph API 返回的项目的排序顺序，请使用 **$orderby** 查询选项。 

例如，若要返回组织中的用户，并按显示名称进行排序，请使用以下语法：

```http
GET https://graph.microsoft.com/v1.0/users?$orderby=displayName
``` 

你还可以按复杂的类型实体进行排序。以下示例获取邮件并按“**发件人**”属性（属于复杂类型 **emailAddress**）中的“**地址**”字段对这些邮件进行排序：

```http
GET https://graph.microsoft.com/v1.0/me/messages?$orderby=from/emailAddress/address
``` 

若要以升序或降序排列结果，请在字段名称中附上 `asc` 或 `desc`（用空格隔开），例如，`?$orderby=name%20desc`

 >  **注意**：如果在 [user](../api-reference/v1.0/resources/user.md) 资源中查询，则 **$orderby** 不能与 filter 表达式结合使用。

## <a name="filter"></a>$filter
若要根据一组条件筛选响应数据，请使用 **$filter** 查询选项。例如，若要返回组织中的用户，并筛选出以“Garth”开头的显示名称，请使用以下语法。

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'Garth')
```

还可以按复杂的类型实体进行筛选。以下示例将返回**发件人**属性的**地址**字段为“jon@contoso.com”的邮件。**发件人**属性属于复杂的类型 **emailAddress**。

```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=from/emailAddress/address eq 'jon@contoso.com'
``` 

## <a name="top"></a>$top
若要指定要在结果集中返回的最大项目数，请使用 **$top** 查询选项。**$top** 查询选项用于确定集合中的子集。此子集通过以下方式形成：仅选择集合的前 N 个项目，其中 N 是此查询选项指定的正整数。例如，若要返回用户邮箱中的前 5 封邮件，请使用以下语法：

```http
GET https://graph.microsoft.com/v1.0/me/messages?$top=5
```

## <a name="skip"></a>$skip
若要在检索集合中的项目之前，设置要跳过的项目数，请使用 **$skip** 查询选项。例如，若要返回按创建日期排序的事件，并从第 21 个事件开始返回，请使用以下语法。

```http
GET  https://graph.microsoft.com/v1.0/me/events?$orderby=createdDateTime&$skip=20
```

## <a name="skiptoken"></a>$skipToken
若要请求 Graph 数据的第二页和后续页，请使用 **$skipToken** 查询选项。当 Graph 已返回结果的部分子集时，**$SkipToken** 查询选项是从 Graph 返回的 URL 中提供的一个选项，这通常是由于服务器端分页造成的。它标识集合中服务器完成发送结果的点，并将其传递回 Graph 以标识其应继续发送结果的位置。例如，**$skipToken** 查询选项的值可以标识集合中的第十项，也可以标识包含 50 个项目的集合中的第 20 项，亦可标识集合中的其他任何位置。

在一些响应中，会看到 `@odata.nextLink` 值。其中一些也包括 **$skipToken** 值。**$skipToken** 值就像是一个标记，可指示服务在何处继续返回下一组结果。以下是一个响应中的 `@odata.nextLink` 值的示例，其中请求的用户按 `displayName` 排序： 

```
"@odata.nextLink": "https://graph.microsoft.com/v1.0/users?$orderby=displayName&$skiptoken=X%2783630372100000000000000000000%27"
```

若要返回组织中的下一页用户，则语法如下所示。

```http
GET  https://graph.microsoft.com/v1.0/users?$orderby=displayName&$skiptoken=X%2783630372100000000000000000000%27
```

## <a name="count"></a>$count
使用 **$count** 作为查询参数，以包含集合中项目总数的计数以及从 Graph 返回的数据值页，如以下示例所示：
```http
GET  https://graph.microsoft.com/v1.0/me/contacts?$count=true
```
这将同时返回**联系人**集合和 `@odata.count` 属性中**联系人**集合中的项目数。

>
  **注意：**[directoryObject](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/directoryobject) 集合对此不支持。
