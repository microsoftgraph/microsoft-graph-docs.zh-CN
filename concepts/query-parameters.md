---
title: 使用查询参数自定义响应
description: Microsoft Graph 提供可选的查询参数，可用于指定和控制响应中返回的数据量。
author: mumbi-o
localization_priority: Priority
ms.custom: graphiamtop20, scenarios:getting-started
ms.openlocfilehash: 51bf43360c3580011ab39e2c385b4c23d3bfc5a1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962411"
---
# <a name="use-query-parameters-to-customize-responses"></a>使用查询参数自定义响应

Microsoft Graph 支持可选的查询参数，可用于指定和控制响应中返回的数据量。 对准确查询参数的支持因 API 操作不同而不同，并且可能会在 v1.0 和数据终结点之间不同，具体取决于 API。 

> [!TIP] 
> 在 beta 终结点上，`$` 前缀是可选的。 例如，可使用 `filter` 来代替 `$filter`。 在 v1 终结点上, `$`前缀仅对 API 的一个子集是可选的。 为简单起见, 如果使用 v1 终结点, 请始终包含`$`。

查询参数可以是 OData 系统查询选项，也可以是其他查询参数。 

> [!VIDEO https://www.youtube-nocookie.com/embed/7BuFv3yETi4]

## <a name="odata-system-query-options"></a>OData 系统查询选项
Microsoft Graph API 操作可以支持以下一个或多个 OData 系统查询选项。 这些查询选项与 [OData V4 查询语言][odata-query]兼容。

>**注意：** OData 4.0 仅在 GET 操作中支持系统查询选项。

单击示例可以在 [Graph 浏览器][graph-explorer]中试调用它们。

| 名称                     | 说明 | 示例
|:-------------------------|:------------|:---------|
| [$count](#count-parameter)         | 检索匹配资源的总数。 | [`/me/messages?$top=2&$count=true`][count-example]
| [$expand](#expand-parameter)       | 检索相关资源。|[`/groups?$expand=members`][expand-example]
| [$filter](#filter-parameter)       | 筛选结果（行）。|[`/users?$filter=startswith(givenName,'J')`][filter-example]
| [$format](#format-parameter)       | 返回指定媒体格式的结果。|[`/users?$format=json`][format-example]
| [$orderby](#orderby-parameter)     | 对结果进行排序。|[`/users?$orderby=displayName desc`][orderby-example]
| [$search](#search-parameter)       | 返回基于搜索条件的结果。 |[`/me/messages?$search=pizza`][search-example]
| [$select](#select-parameter)       | 筛选属性（列）。|[`/users?$select=givenName,surname`][select-example]
| [$skip](#skip-parameter)           | 对结果集建立索引。一些 API 也使用它来实现分页，并且可以与 `$top` 一起使用来手动对结果分页。 | [`/me/messages?$skip=11`][skip-example]
| [$top](#top-parameter)             | 设置结果的页面大小。 |[`/users?$top=2`][top-example]


## <a name="other-query-parameters"></a>其他查询参数

| 名称                     | 说明 | 示例
|:-------------------------|:------------|:---------|
| [$skipToken](#skiptoken-parameter) | 从跨多页的结果集中检索下一页结果。（但某些 API 改为使用 `$skip`。） | `/users?$skiptoken=X%274453707402000100000017...`|

## <a name="other-odata-url-capabilities"></a>其他 OData URL 功能

下列 OData 4.0 功能是 URL 区段，不是查询参数。

| 名称                     | 说明 | 示例 
|:-------------------------|:------------|:---------|
| [$ref](/graph/api/group-post-members) | 更新实体成员身份至集合。 | `POST /groups/{id}/members/$ref` |
| [$value](/graph/api/profilephoto-get) | 检索或更新项的二进制值。 | `GET /me/photo/$value` |

## <a name="encoding-query-parameters"></a>对查询参数进行编码

应对查询参数的值进行百分比编码。 许多 HTTP 客户端、浏览器和工具（如 [Graph 浏览器][graph-explorer]）将在这方面帮助你。 如果查询失败，可能原因之一是未正确编码查询参数值。

未编码的 URL 如下所示：

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName, 'J')
```

正确解码的 URL 如下所示：

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName%2C+'J')
```

### <a name="escaping-single-quotes"></a>转义单引号

对于使用单引号的请求，如果任何参数值也包含单引号，则必须进行双转义；否则，由于语法无效，请求将失败。 在示例中，字符串值 `let''s meet for lunch?` 进行了单引号转义。

```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=subject eq 'let''s meet for lunch?'
```

## <a name="count-parameter"></a>count 参数

使用 `$count` 查询参数以包括集合中项总数的计数，以及从 Microsoft Graph 返回的数据值页。 

例如，下面的请求返回当前用户的 **contact** 集合，以及 `@odata.count` 属性中 **contact** 集合内的项数。

```http
GET  https://graph.microsoft.com/v1.0/me/contacts?$count=true
```

[在 Graph 浏览器中试调用](https://developer.microsoft.com/graph/graph-explorer?request=me/contacts?$count=true&method=GET&version=v1.0)


`$count`查询参数支持这些资源集合和它们的关系派生[自directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta&preserve-view=true)：
- [application](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true)
- [orgContact](/graph/api/resources/orgcontact?view=graph-rest-beta&preserve-view=true)
- [设备](/graph/api/resources/device?view=graph-rest-beta&preserve-view=true)
- [组](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true)
- [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true)
- [用户](/graph/api/resources/user?view=graph-rest-beta&preserve-view=true)。

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

[在 Graph 浏览器中试调用][expand-example]

> **注意：** 并不是所有关系和资源都支持 `$expand` 查询参数。例如，可以扩展用户的 **directReports**、**manager** 和 **memberOf** 关系，但无法扩展其 **events**、**messages** 或 **photo** 关系。并非所有资源或关系都支持对扩展项使用 `$select`。 
> 
> 使用从 [directoryObject](/graph/api/resources/directoryobject) 派生的 Azure AD 资源（如[user](/graph/api/resources/user) 和 [group](/graph/api/resources/group)），`$expand` 仅支持 `beta`，并且通常最多为扩展关系返回 20 个项。

## <a name="filter-parameter"></a>filter 参数

使用 `$filter` 查询参数，以仅检索集合的子集。 `$filter`查询参数还可以用于检索关系，例如members、memberOf、transitiveMembers和transitiveMemberOf。 例如，获取我所属的所有安全组。

以下例子可用于查找显示名称以子母“J”开头的用户，请使用 `startsWith`。

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startsWith(displayName,'J')
```

[在 Graph 浏览器中试调用][filter-example]

对 `$filter` 运算符的支持因 Microsoft Graph API 不同而异。 通常支持下列逻辑运算符：

- 等于 `eq`/不等于 `ne`
- 小于 `lt`/大于 `gt`
- 小于或等于 `le`/大于或等于 `ge`
- 和 `and`/或 `or`
- 属于 `in`
- 否定式 `not`
- l匿名函数运算符 any `any`
- l匿名函数运算符 all `all`
- 开头为 `startsWith`
- 结尾为 `endsWith`

> **注意：** 对这些运算符的支持因实体而异。 有关详细信息，请参阅特定实体文档。 
>
> 所有 Microsoft Graph 资源目前均不支持 `contains` 字符串运算符。

有关一些用法示例的信息，请参阅下表。 如需了解 `$filter` 语法的更多详情，请参阅 [OData 协议][odata-filter]。  
下表展示了一些使用 `$filter` 查询参数的示例。

> **注意：** 单击示例可以在 [Graph 浏览器][graph-explorer]中试调用。

| 说明 | 示例
|:------------|:--------|
| 跨多个属性获取名为 Mary 的用户。 | [`https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'mary') or startswith(givenName,'mary') or startswith(surname,'mary') or startswith(mail,'mary') or startswith(userPrincipalName,'mary')`](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(displayName,'mary')+or+startswith(givenName,'mary')+or+startswith(surname,'mary')+or+startswith(mail,'mary')+or+startswith(userPrincipalName,'mary')&method=GET&version=v1.0) |
| 获取邮件域等于“hotmail.com”的所有用户 | [`https://graph.microsoft.com/v1.0/users?$count=true&$filter=endsWith(mail,'@hotmail.com')`](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24count%3Dtrue%26%24filter%3DendsWith(mail%2C'%40hotmail.com')%26%24select%3Did%2CdisplayName%2Cmail&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) |
| 获取 2017 年 7 月 1 日之后开始的所有登录用户的事件。 | [`https://graph.microsoft.com/v1.0/me/events?$filter=start/dateTime ge '2017-07-01T08:00'`](https://developer.microsoft.com/graph/graph-explorer?request=me/events?$filter=start/dateTime+ge+'2017-07-01T08:00'&method=GET&version=v1.0) |
| 获取登录用户收到的来自特定地址的所有电子邮件。 | [`https://graph.microsoft.com/v1.0/me/messages?$filter=from/emailAddress/address eq 'someuser@example.com'`](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=from/emailAddress/address+eq+'someuser@.com'&method=GET&version=v1.0) |
| 获取登录用户在 2017 年 4 月收到的所有电子邮件。 | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=ReceivedDateTime ge 2017-04-01 and receivedDateTime lt 2017-05-01`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=ReceivedDateTime+ge+2017-04-01+and+receivedDateTime+lt+2017-05-01&method=GET&version=v1.0) |
| 获取登录用户收件箱中的所有未读邮件。 | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=isRead eq false`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=isRead+eq+false&method=GET&version=v1.0) |
| 列出组织中的所有 Microsoft 365 组。 | [`https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')`](https://developer.microsoft.com/graph/graph-explorer?request=groups?$filter=groupTypes/any(c:c+eq+'Unified')&method=GET&version=v1.0) |
| 使用 OData 转换可实现显示名称以“ a”开头（包括返回的对象数）的组中的临时成员资格。 | [`https://graph.microsoft.com/beta/me/transitiveMemberOf/microsoft.graph.group?$count=true&$filter=startswith(displayName, 'a')`](https://developer.microsoft.com/graph/graph-explorer?request=me/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName,'a')&method=GET&version=v1.0) |

## <a name="format-parameter"></a>format 参数

使用 `$format` 查询参数，指定 Microsoft Graph 返回的项的媒体格式。

例如，下面的请求以 json 格式返回组织中的用户：

```http
GET https://graph.microsoft.com/v1.0/users?$format=json
```

[在 Graph 浏览器中试调用][format-example]

> **注意：**`$format` 查询参数支持许多格式（例如，atom、xml 和 json），但可能无法返回所有格式的结果。

## <a name="orderby-parameter"></a>orderby 参数

使用 `$orderby` 查询参数指定从 Microsoft Graph 返回的项的排序顺序。

例如，以下请求返回按用户显示名称进行排序的组织中的用户：

```http
GET https://graph.microsoft.com/v1.0/users?$orderby=displayName
```
[在 Graph 浏览器中试调用][orderby-example]

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

> **注意：** 如果指定 $filter，服务器会推断结果的排序顺序。 如果同时使用 `$orderby` 和 `$filter` 获取消息，因为服务器始终会推断 `$filter` 结果的排序顺序，必须[以特定的方式指定属性](/graph/api/user-list-messages#using-filter-and-orderby-in-the-same-query)。


下面的示例展示了如何按 **subject** 和 **importance** 属性筛选查询，再按 **subject**、**importance** 和 **receivedDateTime** 属性进行降序排序。

```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=Subject eq 'welcome' and importance eq 'normal'&$orderby=subject,importance,receivedDateTime desc
```

[在 Graph 浏览器中试调用](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=subject%20eq%20%27welcome%27%20and%20importance%20eq%20%27normal%27%20&$orderby=subject,importance,receivedDateTime%20desc&method=GET&version=v1.0)

> **注意：** 对于以下 AD 资源及其从 [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta&preserve-view=true) 派生的关系，在 Beta 终结点上支持组合 `$orderby` 和 `$filter` 查询参数：
>
>- [application](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true)
>- [orgContact](/graph/api/resources/orgcontact?view=graph-rest-beta&preserve-view=true)
>- [设备](/graph/api/resources/device?view=graph-rest-beta&preserve-view=true)
>- [组](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true)
>- [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true)
>- [用户](/graph/api/resources/user?view=graph-rest-beta&preserve-view=true)
>
> 若要将`$orderby``$filter`、或`$filter`与`endsWith`一，则需要：
>
> - 将 `$count=true` 添加到查询参数
> - 添加 `ConsistencyLevel: eventual` 请求标题
>
> 有关更多信息，请参见[可选用户查询参数](/graph/api/user-list?view=graph-rest-beta&preserve-view=true#optional-query-parameters)。

## <a name="search-parameter"></a>search 参数

使用 `$search` 查询参数限制与搜索条件匹配的请求结果。

### <a name="using-search-on-message-collections"></a>对 message 集合使用 $search

可根据特定邮件属性值搜索邮件。 搜索结果按邮件发送日期和时间进行排序。 `$search` 请求最多可返回 250 个结果。

如果确实要搜索邮件，且仅指定值，而未指定特定邮件属性，搜索依据为默认搜索属性 **from**、**subject** 和 **body**。

下面的示例返回登录用户收件箱中三个默认搜索属性中有任意一个包含“pizza”的所有邮件：

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="pizza"
```

[在 Graph 浏览器中试调用][search-example]

也可以指定下表中的邮件属性名来搜索邮件，这些属性名可由关键字查询语言 (KQL) 语法识别。 这些属性名对应于 Microsoft Graph **message** 实体中定义的属性。 Outlook 和其他 Microsoft 365 应用程序（如 SharePoint）支持 KQL 语法，从而为数据存储提供了方便使用的公共发现域。


| 可搜索的电子邮件属性                | 说明 | 示例 
|:-------------------------|:------------|:---------|
| **attachment**           | 电子邮件附件的文件名。|[`me/messages?$search="attachment:api-catalog.md"`][search-att-example]
| **bcc**           | 电子邮件的 **bcc** 字段，可指定为 SMTP 地址、显示名称或别名。|[`me/messages?$search="bcc:samanthab@contoso.com"&$select=subject,bccRecipients`][search-bcc-example]
| **body**           | 电子邮件正文。|[`me/messages?$search="body:excitement"`][search-body-example]
| **cc**           | 电子邮件的 **cc** 字段，可指定为 SMTP 地址、显示名称或别名。|[`me/messages?$search="cc:danas"&$select=subject,ccRecipients`][search-cc-example]
| **from**           | 电子邮件的发件人，可指定为 SMTP 地址、显示名称或别名。|[`me/messages?$search="from:randiw"&$select=subject,from`][search-from-example]
| **hasAttachment** | 如果电子邮件附件不是内联附件，则为 true；否则，为 false。 |[`me/messages?$search="hasAttachments:true"`][search-from-example]
| **importance**           | 发件人在发送邮件时可以指定的电子邮件重要性。 可取值包括 `low`、`medium` 或 `high`。|[`me/messages?$search="importance:high"&$select=subject,importance`][search-imp-example]
| **Kind**           | 邮件类型。 可取值包括 `contacts`、`docs`、`email`、`faxes`、`im`、`journals`、`meetings`、`notes`、`posts`、`rssfeeds`、`tasks` 或 `voicemail`。|[`me/messages?$search="kind:voicemail"`][search-kind-example]
| **participants**           | 电子邮件的 **from**、**to**、**cc** 和 **bcc** 字段，可指定为 SMTP 地址、显示名称或别名。|[`me/messages?$search="participants:danas"`][search-part-example]
| **received**           | 收件人接收电子邮件的日期。|[`me/messages?$search="received:07/23/2018"&$select=subject,receivedDateTime`][search-rcvd-example]
| **recipients**           | 电子邮件的 **to**、**cc** 和 **bcc** 字段，可指定为 SMTP 地址、显示名称或别名。|[`me/messages?$search="recipients:randiq"&$select=subject,toRecipients,ccRecipients,bccRecipients`][search-rcpts-example]
| **sent**           | 发件人发送电子邮件的日期。|[`me/messages?$search="sent:07/23/2018"&$select=subject,sentDateTime`][search-sent-example]
| **size**           | 邮件大小（以字节为单位）。|[`me/messages?$search="size:1..500000"`][search-size-example]
| **subject**           | 电子邮件主题行中的文本。 .|[`me/messages?$search="subject:has"&$select=subject`][search-sbj-example]
| **to**           | 电子邮件的 **to** 字段，可指定为 SMTP 地址、显示名称或别名。|[`me/messages?$search="to:randiw"&$select=subject,toRecipients`][search-to-example]


若要详细了解 可搜索的电子邮件属性、KQL 语法、受支持的运算符和搜索技巧，请参阅以下文章：

- [Exchange 中的可搜索属性](/Exchange/policy-and-compliance/ediscovery/message-properties-and-search-operators#searchable-properties-in-exchange)。

- [关键字查询语言 (KQL) 语法参考](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference)

- [Exchange 2016 中的就地电子数据展示的邮件属性和搜索运算符](/Exchange/policy-and-compliance/ediscovery/message-properties-and-search-operators)

### <a name="using-search-on-person-collections"></a>对 person 集合使用 $search

可以使用 Microsoft Graph People API 检索与用户相关度最高的人员。 相关性由用户的通信和协作模式及业务关系决定。 People API 支持 `$search` 查询参数。 `$search` 请求最多可返回 250 个结果。

人员搜索就是按 [person](/graph/api/resources/person) 资源的 **displayName** 和 **emailAddress** 属性进行搜索。

以下请求在已登录用户的 **人员** 集合中的每个人员的 **displayName** 和 **emailAddress** 属性中，为名为“Irene McGowen”的人员执行搜索。 由于一个名为“Irene McGowan”的人员与登录用户相关，因此返回了“Irene McGowan”的信息。

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="Irene McGowen"
```

以下示例显示了相应的响应。 

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
       {
           "id": "C0BD1BA1-A84E-4796-9C65-F8A0293741D1",
           "displayName": "Irene McGowan",
           "givenName": "Irene",
           "surname": "McGowan",
           "birthday": "",
           "personNotes": "",
           "isFavorite": false,
           "jobTitle": "Auditor",
           "companyName": null,
           "yomiCompany": "",
           "department": "Finance",
           "officeLocation": "12/1110",
           "profession": "",
           "userPrincipalName": "irenem@contoso.onmicrosoft.com",
           "imAddress": "sip:irenem@contoso.onmicrosoft.com",
           "scoredEmailAddresses": [
               {
                   "address": "irenem@contoso.onmicrosoft.com",
                   "relevanceScore": -16.446060612802224
               }
           ],
           "phones": [
               {
                   "type": "Business",
                   "number": "+1 412 555 0109"
               }
           ],
           "postalAddresses": [],
           "websites": [],
           "personType": {
               "class": "Person",
               "subclass": "OrganizationUser"
           }
       }
   ]
}
```

若要了解有关 People API 的详细信息，请参阅[获取相关人员的信息](./people-example.md#search-people)。  

### <a name="using-search-on-directory-object-collections"></a>在目录对象集合上使用 $search

可使用 `$search` 查询参数来使用标记筛选结果。 标记化搜索的工作原理是提取输入和输出字符串中的单词，并使用空格、数字、不同的大小写和符号分隔这些词，如下所示：

* **空格**：`hello world` => `hello`、 `world`
* **不同的大小写**⁽¹⁾：`HelloWorld` 或 `helloWORLD` => `hello`、`world`
* **符号**⁽⁾：`hello.world` => `hello`、`.`、`world`， `helloworld`
* **数字**：`hello123world` => `hello`、`123`、 `world`

⁽¹⁾ 目前，标记化仅在大小写从小写转换为大写时才有效，因此 `HELLOworld` 被视为一个标记：`helloworld`，`HelloWORld` 是两个标记：`hello`、`world`。 ⁽²⁾ 标记化逻辑还会合并仅由符号分隔的单词；例如，搜索 `helloworld` 将找到 `hello-world` 和 `hello.world`。

> **注意**：标记化后，标记将独立于原始大小写进行匹配，并且将以任何顺序匹配。
> `$search` 目录对象集合上的查询参数 **需要** 特殊的请求标头：`ConsistencyLevel: eventual`。

标记化搜索支持仅适用于 **displayName** 和 **description** 字段。 任何字段都可以放入 `$search`；非 **displayName** 和 **description** 的字段默认为 `$filter` startswith 行为。 例如：

`https://graph.microsoft.com/beta/groups/?$search="displayName:OneVideo"`

这将查找显示名称看起来像 "OneVideo" 的所有组。 也可与`$search`配合使用`$filter`。 例如：

`https://graph.microsoft.com/beta/groups/?$filter=mailEnabled eq true&$search="displayName:OneVideo"`

这将查找显示名称类似于“OneVideo”的所有启用邮件的组。 结果是根据逻辑结合（"AND"）和`$filter`整个查询`$search`来限制。 搜索文本基于大小写进行标记，但是匹配以不区分大小写的方式执行。 例如，“OneVideo”将被分割成两个输入标记“one”和“video”，但是匹配不区分大小写的属性。

搜索的语法遵循以下规则：

* 通用格式：$search="clause1" \[AND \| OR\] "\[clauseX\]"\.
* 支持任何子句。 支持适用于优先级的括号。
* 每个子句的语法是："\<property>:\<text to search>"。
* 必须在子句中指定属性名称。 可以在中使用的任何属性`$filter`也可以在内使用 `$search`。 根据属性的不同，如果属性不支持搜索，那么搜索行为要么是“search”，要么是“start with”。
* 必须将完整子句部分置于双引号内。
* 必须将逻辑运算符 "AND" 和 "OR" 置于双引号之外。 它们必须处于大写形式。
* 考虑到整个子句部分需要放在双引号内，如果包含双引号和反斜杠，则需要使用反斜杠对其进行转义。 无需转义其他字符。

下表显示了一些示例。

| 对象类 | 说明 | 示例 |
| ------------ | ----------- | ------- |
| 用户 | 通讯簿显示用户的名称。 | `https://graph.microsoft.com/beta/users?$search="displayName:Guthr"` |
| 用户 | 通讯簿显示用户的名称或邮件。 | `https://graph.microsoft.com/beta/users?$search="displayName:Guthr" OR "mail:Guthr"` |
| Group | 通讯簿显群组的名称或说明。 | `https://graph.microsoft.com/beta/groups?$search="description:One" AND ("displayName:Video" OR "displayName:Drive")` |
| Group | 通讯簿在启用邮件组上显示名称。 | `https://graph.microsoft.com/beta/groups?$filter=mailEnabled eq true&$search="displayName:OneVideo"` |

你在 `$search` 中提供的字符串输入以及可搜索属性都按空格、不同的大小写和字符类型（数字和特殊字符）划分为多个部分。

## <a name="select-parameter"></a>select 参数

使用 `$select` 查询参数返回一组不同于单个资源的默认集或资源集合的属性。 使用 $select，可以指定默认属性的子集或超集。

例如，检索登录用户的邮件时，可以指定仅返回 **from** 和 **subject** 属性：

```http
GET https://graph.microsoft.com/v1.0/me/messages?$select=from,subject
```

[在 Graph 浏览器中试调用][select-example]

> **重要说明：** 一般来说，建议使用 `$select` 将查询返回的属性限制为应用所需的属性。 这对于可能返回大型结果集的查询尤为有用。 限制每行返回的属性将减少网络负载并帮助提升应用的性能。
>
> 在 `v1.0` 中，从 [directoryObject](/graph/api/resources/directoryobject) 派生的一些 Azure AD 资源（如 [user](/graph/api/resources/user) 和 [group](/graph/api/resources/group)）在读取时返回受限的默认属性子集。对于这些资源，必须使用 `$select` 将属性返回到默认集之外。  

## <a name="skip-parameter"></a>skip 参数

使用 `$skip` 查询参数设置要在集合开头跳过的项数。例如，以下请求返回按照创建日期排序的用户的事件，从集合中的第 21 个事件开始：

```http
GET  https://graph.microsoft.com/v1.0/me/events?$orderby=createdDateTime&$skip=20
```
[在 Graph 浏览器中试调用][skip-example]

> **注意：** 一些 Microsoft Graph API 使用 `$skip` 实现分页，如 Outlook 邮件和日历（**message**、**event** 和 **calendar**）。 当查询结果跨多个页面时，这些 API 会返回 `@odata:nextLink` 属性，具有包含 `$skip` 参数的 URL。 可以使用此 URL 返回下一页结果。 若要了解详细信息，请参阅[分页](./paging.md)。

## <a name="skiptoken-parameter"></a>skipToken 参数

由于服务器端分页或由于使用 [`$top`](#top-parameter) 参数来限制响应的页面大小，致使一些请求返回多页数据。 许多 Microsoft Graph API 使用 `skipToken` 查询参数来引用结果的后续页面。  
`$skiptoken` 参数包含引用下一页结果的不透明令牌，并在响应的 `@odata.nextLink` 属性中提供的 URL 中返回。 若要了解详细信息，请参阅[分页](./paging.md)。
> **注意**：如果你使用的是 OData 计数（在查询字符串中添加 `$count=true`），则 `@odata.count` 属性将仅在第一页中出现。

## <a name="top-parameter"></a>top 参数

使用 `$top` 查询参数指定结果集的页面大小。 

如果结果集中还剩余多个项目，则响应正文将包含 `@odata.nextLink` 参数。 此参数包含可用于获取下一页结果的 URL。 若要了解详细信息，请参阅[分页](./paging.md)。 

最小值为 $top 1，最大值取决于相应的 API。  

例如，以下列表 [请求](/graph/api/user-list-messages) 返回用户邮箱中的前五条消息：

```http
GET https://graph.microsoft.com/v1.0/me/messages?$top=5
```

[在 Graph 浏览器中试调用][top-example]


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
[odata-filter]: https://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752358
[odata-query]: https://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752356
[count-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$top=2%26$count=true&method=GET&version=v1.0
[expand-example]: https://developer.microsoft.com/graph/graph-explorer?request=groups?$expand=members&method=GET&version=v1.0
[filter-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(givenName,'J')&method=GET&version=v1.0
[format-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$format=json&method=GET&version=v1.0
[orderby-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$orderby=displayName%20DESC&method=GET&version=v1.0
[search-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=pizza&method=GET&version=v1.0
[select-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$select=givenName,surname&method=GET&version=v1.0
[skip-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$skip=11&method=GET&version=v1.0
[top-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$top=2&method=GET&version=v1.0

[search-att-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22attachment%3Aapi-catalog%2Emd%22&method=GET&version=v1.0
[search-bcc-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22bcc%3Asamanthab%40contoso%2Ecom%22%26$select=subject,bccRecipients&method=GET&version=v1.0
[search-body-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22body%3Aexcitement%22&method=GET&version=v1.0
[search-cc-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22cc%3Adanas%22%26$select=subject,ccRecipients&method=GET&version=v1.0
[search-from-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22from%3Arandiw%22%26$select=subject,from&method=GET&version=v1.0
[search-hasatt-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22hasAttachments=true%22&method=GET&version=v1.0
[search-imp-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22importance%3Ahigh%22%26$select=subject,importance&method=GET&version=v1.0
[search-kind-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22kind%3Avoicemail%22&method=GET&version=v1.0
[search-part-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22participants%3Adanas%22&method=GET&version=v1.0

[search-rcvd-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22received%3A07/23/2018%22%26$select=subject,receivedDateTime&method=GET&version=v1.0

[search-rcpts-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22recipients%3Arandiw%22%26$select=subject,toRecipients,ccRecipients,bccRecipients&method=GET&version=v1.0
[search-sent-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22sent%3A07/23/2018%22%26$select=subject,sentDateTime&method=GET&version=v1.0
[search-size-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22size%3A1%2E%2E500000%22&method=GET&version=v1.0

[search-sbj-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22subject%3Ahas%22%26$select=subject&method=GET&version=v1.0
[search-to-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22to%3Arandiw%22%26$select=subject,toRecipients&method=GET&version=v1.0



## <a name="see-also"></a>另请参阅

- [查询参数限制](known-issues.md#query-parameter-limitations)
