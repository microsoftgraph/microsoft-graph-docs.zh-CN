---
title: 使用查询参数自定义响应
description: Microsoft Graph 提供可选的查询参数，可用于指定和控制响应中返回的数据量。
author: mumbi-o
ms.localizationpriority: high
ms.custom: graphiamtop20, scenarios:getting-started
ms.openlocfilehash: e0af0692e89f0ea099fb480ecd57cd60e54bd798
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461371"
---
# <a name="use-query-parameters-to-customize-responses"></a>使用查询参数自定义响应

Microsoft Graph 支持可选的查询参数，可用于指定和控制响应中返回的数据量。 对准确查询参数的支持因 API 操作不同而不同，并且可能会在 v1.0 和数据终结点之间不同，具体取决于 API。

> [!TIP] 
> 在 beta 终结点上，`$` 前缀是可选的。 例如，可使用 `filter` 来代替 `$filter`。 在 v1 终结点上, `$`前缀仅对 API 的一个子集是可选的。 为简单起见, 如果使用 v1 终结点, 请始终包含`$`。

查询参数可以是 [OData 系统查询选项](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part2-url-conventions.html#_Toc31360955)，也可以是其他查询参数。

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

若要了解 API 及其属性支持的 OData 系统查询选项，请参阅资源页中的 **属性** 表，以及 API 的 LIST 和 GET 操作部分 **可选查询参数**。

## <a name="other-query-parameters"></a>其他查询参数

| 名称                     | 说明 | 示例
|:-------------------------|:------------|:---------|
| [$skipToken](#skiptoken-parameter) | 从跨多页的结果集中检索下一页结果。（但某些 API 改为使用 `$skip`。） | `/users?$skiptoken=X%274453707402000100000017...`|

## <a name="other-odata-url-capabilities"></a>其他 OData URL 功能

下列 OData 4.0 功能是 URL 区段，不是查询参数。

| 名称                     | 说明 | 示例 
|:-------------------------|:------------|:---------|
| [$count](/graph/api/user-list#example-3-get-only-a-count-of-users)| 检索集合的整数总计。 | `GET /users/$count` <br> `GET /groups/{id}/members/$count`|
| [$ref](/graph/api/group-post-members) | 更新实体成员身份至集合。 | `POST /groups/{id}/members/$ref` |
| [$value](/graph/api/profilephoto-get) | 检索或更新项的二进制值。 | `GET /me/photo/$value` |
| [$batch](/graph/json-batching) | 将多个 HTTP 请求合并到批处理请求中。 | `POST /$batch` |

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

对于使用单引号的请求，如果任何参数值也包含单引号，则必须进行双转义；否则，由于语法无效，请求将失败。在该示例中，字符串值 `let''s meet for lunch?` 具有转义单引号。

```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=subject eq 'let''s meet for lunch?'
```

## <a name="count-parameter"></a>count 参数

使用 `$count` 查询参数检索集合中的项总数或与表达式匹配的项总数。 可以通过以下方式使用 `$count`：

1. 作为具有语法 `$count=true` 的查询字符串参数，用于在从 Microsoft Graph 返回的数据值页面旁边包含集合中的项总数。例如，`users?$count=true`。
2. 作为 [URL 段](#other-odata-url-capabilities)，仅检索集合的整数总计。 例如，`users/$count`。
3. 在具有等式运算符的 `$filter` 表达式中，检索筛选属性为空集合的数据集合。 请参阅[以下示例](#examples-using-the-filter-query-operator)。

> [!NOTE]
> 1. 在派生自 [directoryObject](/graph/api/resources/directoryobject) 的资源上，仅在高级查询中支持 `$count`。 请参阅[Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。
> 2. Azure AD B2C 租户不支持使用`$count`。

例如，下面的请求返回当前用户的 **contact** 集合，以及 `@odata.count` 属性中 **contact** 集合内的项数。

```msgraph-interactive
GET  https://graph.microsoft.com/v1.0/me/contacts?$count=true
```

`$count`查询参数支持以下常用资源集合和派生自[directoryObject](/graph/api/resources/directoryobject)的关系，而且仅在[高级查询](/graph/aad-advanced-queries)中支持：
- [administrativeUnit](/graph/api/resources/administrativeunit)
- [application](/graph/api/resources/application)
- [orgContact](/graph/api/resources/orgcontact)
- [设备](/graph/api/resources/device)
- [组](/graph/api/resources/group)
- [servicePrincipal](/graph/api/resources/serviceprincipal)
- [用户](/graph/api/resources/user)

## <a name="expand-parameter"></a>expand 参数

许多 Microsoft Graph 资源都会公开资源的已声明属性以及与其他资源的关系。 这些关系也称为引用属性或导航属性，它们可以引用单个资源或资源集合。 例如，用户的邮件文件夹、管理者和直接下属都将作为关系公开。 

通常情况下，可以在单个请求中查询资源属性或其关系之一，但不能同时查询。可以使用 `$expand` 查询字符串参数以包含结果中单个关系（导航属性）引用的扩展资源或集合。一个请求中只能扩展一个关系。

以下示例在驱动器中获取根驱动器信息以及顶级子项：

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children
```


使用一些资源集合，还可以添加 `$select` 参数，指定要在扩展资源中返回的属性。下面的示例执行与上一示例几乎相同的查询，不同之处在于使用 [`$select`](#select-parameter) 语句将为扩展子项返回的属性限制为 **id** 和 **name** 属性。

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children($select=id,name)
```

> [!NOTE]
> + 并不是所有关系和资源都支持 `$expand` 查询参数。例如，可以扩展用户的 **directReports**、**manager** 和 **memberOf** 关系，但无法扩展其 **events**、**messages** 或 **photo** 关系。并非所有资源或关系都支持对扩展项使用 `$select`。 
> 
> + 对于派生自 [directoryObject](/graph/api/resources/directoryobject) 的 Azure AD 资源，例如，[user](/graph/api/resources/user) 和 [group](/graph/api/resources/group)，`$expand` 通常最多为扩展关系返回 20 个项，并且没有 [@odata.nextLink](./paging.md)。查看更多[已知问题](known-issues.md#query-parameters)。
>
> + [高级查询](/graph/aad-advanced-queries)当前不支持`$expand`。

## <a name="filter-parameter"></a>filter 参数

使用 `$filter` 查询参数，以仅检索集合的子集。 `$filter`查询参数还可以用于检索关系，例如members、memberOf、transitiveMembers和transitiveMemberOf。 例如，获取我所属的所有安全组。

以下示例查找显示名称以字母“J”开头的用户:

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=startsWith(displayName,'J')
```

对 `$filter` 运算符的支持因 Microsoft Graph API 不同而异。 通常支持下列逻辑运算符：

| 运算符类型 | 运算符 |
| --- | --- |
| 相等运算符 | <ul><li> 等于 (`eq`) </li><li> 不等于 (`ne`)</li><li> 逻辑否定（`not`）</li><li> 在 (`in`) 中</li></ul> |
| 关系运算符 | <ul><li> 小于 (`lt`) </li><li> 大于 (`gt`)</li><li> 小于或等于 (`le`)</li><li> 大于或等于 (`ge`)</li></ul> |
| Lambda 运算符 | <ul><li> 任何 (`any`)  </li><li> 全部 (`all`)</li></ul>|
| 条件运算符 | <ul><li> 以及 (`and`) </li><li> 或 (`or`)</li> |
| 函数 | <ul><li> 开头为 （`startsWith`） </li><li> 结尾为 （`endsWith`）</li><li> 包含 (`contains`)</li></ul>|


> **注意:** 对这些运算符的支持因实体而异，某些属性仅在 [高级查询](/graph/aad-advanced-queries)中支持`$filter`。有关详细信息，请参阅特定实体文档。

### <a name="filter-using-lambda-operators"></a>使用 lambda 运算符进行筛选

OData 定义 `any` 和 `all` 运算符以评估多值属性的匹配项，即基元值(如字符串 类型或实体集合)的集合。

#### <a name="any-operator"></a>`any` 运算符

`any` 运算符以迭代方式将布尔表达式应用于集合的每个成员，如果集合的 *任何成员* 的表达式为 `true`，则返回 `true`;否则返回 `false`。下面是 `any` 运算符的语法：

```http
$filter=param/any(var:var/subparam eq 'value-to-match')
```

其中
+ *param* 是包含值集合或实体集合的属性。
+ *var:var* 是一个范围变量，用于在迭代期间保存集合的当前元素。 此变量几乎可以被命名为任何内容，例如， *adele:adele* 或 *x:x*。
+ 当查询应用于实体集合时，*subparam* 是必需的。 它表示正在匹配其值的复杂类型的属性。
+ *value-to-match* 表示要与之匹配的集合的成员。

例如，用户资源的 **imAddresses** 属性包含基元类型 String 的集合。 以下查询仅检索 imAddress 为 `admin@contoso.com`的用户。

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=imAddresses/any(s:s eq 'admin@contoso.com')
```

用户资源的 **assignedLicenses** 属性包含 **assignedLicense** 对象的集合，一个包含两个属性 **skuId** 和 **disabledPlans** 的复杂类型。 以下查询仅检索具有由 **skuId** `184efa21-98c3-4e5d-95ab-d07053a96e67`标识的已分配许可证的用户。

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=assignedLicenses/any(s:s/skuId eq 184efa21-98c3-4e5d-95ab-d07053a96e67)
```

若要对 `any` 子句内表达式的结果求反，请使用 `not` 运算符，而不是 `ne` 运算符。 例如，以下查询仅检索未分配 `admin@contoso.com` 的 **imAddress** 的用户。
>**注意:** 对于像用户这样的目录对象，`not` 和 `ne` 运算符仅在 [高级查询](/graph/aad-advanced-queries) 中受支持。

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=NOT(imAddresses/any(s:s eq 'admin@contoso.com'))&$count=true
ConsistencyLevel: eventual
```

#### <a name="all-operator"></a>`all` 运算符

`all`运算符以迭代方式将布尔表达式应用于集合的每个成员，如果集合的 *所有成员* 的表达式为`true`，则返回`true`;否则返回`false`。它不受任何属性支持。

### <a name="examples-using-the-filter-query-operator"></a>使用筛选器查询运算符的示例

下表展示了一些使用 `$filter` 查询参数的示例。 如需了解 `$filter` 语法的更多详情，请参阅 [OData 协议][odata-filter]。

> **注意：** 单击示例可以在 [Graph 浏览器][graph-explorer]中试调用。

| 说明 | 示例
|:------------|:--------|
| 跨多个属性获取名为 Mary 的用户。 | [GET](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(displayName,'mary')+or+startswith(givenName,'mary')+or+startswith(surname,'mary')+or+startswith(mail,'mary')+or+startswith(userPrincipalName,'mary')&method=GET&version=v1.0) `../users?$filter=startswith(displayName,'mary') or startswith(givenName,'mary') or startswith(surname,'mary') or startswith(mail,'mary') or startswith(userPrincipalName,'mary')` |
| 获取邮件域等于“hotmail.com”的所有用户 | [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24count%3Dtrue%26%24filter%3DendsWith(mail%2C'%40hotmail.com')%26%24select%3Did%2CdisplayName%2Cmail&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d)`../users?$count=true&$filter=endsWith(mail,'@hotmail.com')`。这是一个[高级查询](/graph/aad-advanced-queries)。 |
| 获取所有未分配许可证的用户 | [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24filter%3DassignedLicenses%2F%24count%2Bne%2B0%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d)`../users?$filter=assignedLicenses/$count eq 0&$count=true`。这是一个[高级查询](/graph/aad-advanced-queries)。 |
| 获取 2017 年 7 月 1 日之后开始的所有登录用户的事件。 | 
  [GET](https://developer.microsoft.com/graph/graph-explorer?request=me/events?$filter=start/dateTime+ge+'2017-07-01T08:00'&method=GET&version=v1.0) `../me/events?$filter=start/dateTime ge '2017-07-01T08:00'`。 <br/>**注意：****dateTime** 属性为字符串类型。 |
| 获取登录用户收到的来自特定地址的所有电子邮件。 | [GET](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=from/emailAddress/address+eq+'someuser@.com'&method=GET&version=v1.0) `../me/messages?$filter=from/emailAddress/address eq 'someuser@example.com'` |
| 获取登录用户在 2017 年 4 月收到的所有电子邮件。 | [GET](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=ReceivedDateTime+ge+2017-04-01+and+receivedDateTime+lt+2017-05-01&method=GET&version=v1.0) `../me/mailFolders/inbox/messages?$filter=ReceivedDateTime ge 2017-04-01 and receivedDateTime lt 2017-05-01` |
| 获取登录用户收件箱中的所有未读邮件。 | [GET](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=isRead+eq+false&method=GET&version=v1.0) `../me/mailFolders/inbox/messages?$filter=isRead eq false` |
| 获取零售和销售部门中的所有用户。 | 
  [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24filter%3Ddepartment%20in%20('Retail'%2C%20'Sales')&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com) `../users?$filter=department in ('Retail', 'Sales')`| 
| 列出具有处于挂起状态的特定服务计划的用户。 | [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24filter%3DassignedPlans%2Fany(a%3Aa%2FservicePlanId%20eq%202e2ddb96-6af9-4b1d-a3f0-d6ecfd22edb2%20and%20a%2FcapabilityStatus%20eq%20'Suspended')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d)`../users?$filter=assignedPlans/any(a:a/servicePlanId eq 2e2ddb96-6af9-4b1d-a3f0-d6ecfd22edb2 and a/capabilityStatus eq 'Suspended')&$count=true`。这是一个[高级查询](/graph/aad-advanced-queries)。 |
| 列出组织中的所有非 Microsoft 365 组。 | [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=groups%3F%24filter%3DNOT%20groupTypes%2Fany(c%3Ac%20eq%20'Unified')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d)`../groups?$filter=NOT groupTypes/any(c:c eq 'Unified')&$count=true`。这是一个[高级查询](/graph/aad-advanced-queries)。 |
| 列出其公司名称不是未定义(即，不是 `null` 值)或 Microsoft 的所有用户。 | [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24filter%3DcompanyName%20ne%20null%20and%20NOT(companyName%20eq%20'Microsoft')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d)`../users?$filter=companyName ne null and NOT(companyName eq 'Microsoft')&$count=true`。这是一个[高级查询](/graph/aad-advanced-queries)。 |
| 列出其公司名称是未定义或 Microsoft 的所有用户。 | [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24filter%3DcompanyName%20in%20(null%2C%20'Microsoft')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d)`../users?$filter=companyName in (null, 'Microsoft')&$count=true`。这是一个[高级查询](/graph/aad-advanced-queries)。 |
| 使用 OData 转换可实现显示名称以“ a”开头(包括返回的对象数)的组中的临时成员资格。 | [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=me%2FtransitiveMemberOf%2Fmicrosoft.graph.group%3F%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d)`../me/transitiveMemberOf/microsoft.graph.group?$count=true&$filter=startswith(displayName, 'a')`。这是一个[高级查询](/graph/aad-advanced-queries)。 |

## <a name="format-parameter"></a>format 参数

使用 `$format` 查询参数，指定 Microsoft Graph 返回的项的媒体格式。

例如，下面的请求以 json 格式返回组织中的用户：

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$format=json
```


> **注意：**`$format` 查询参数支持许多格式（例如，atom、xml 和 json），但可能无法返回所有格式的结果。

## <a name="orderby-parameter"></a>orderby 参数

使用 `$orderby` 查询参数指定从 Microsoft Graph 返回的项的排序顺序。默认顺序为升序。

例如，以下请求返回按用户显示名称进行排序的组织中的用户：

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$orderby=displayName
```

还可以按复杂类型实体进行排序。下面的请求获取邮件，并按 **from** 属性的 **address** 字段（复杂类型为 **emailAddress**）进行排序：

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages?$orderby=from/emailAddress/address
```

若要以升序或降序对结果进行排序，请向字段名称追加 `asc` 或 `desc`，并用空格隔开。例如，`?$orderby=name%20desc`。 如果未指定排序顺序，则推断默认值(升序)。

通过一些 API，可以对多个属性的结果进行排序。例如，以下请求首先按发件人名称以降序(Z 到 A)排序用户收件箱中的邮件，然后按主题以升序(默认)排序邮件。

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailFolders/Inbox/messages?$orderby=from/emailAddress/name desc,subject
```

> **注意:** 如果指定 `$filter`，服务器会推断结果的排序顺序。 如果同时使用 `$orderby` 和 `$filter` 获取消息，因为服务器始终会推断 `$filter` 结果的排序顺序，必须[以特定的方式指定属性](/graph/api/user-list-messages#using-filter-and-orderby-in-the-same-query)。


下面的示例展示了如何按 **subject** 和 **importance** 属性筛选查询，再按 **subject**、**importance** 和 **receivedDateTime** 属性进行降序排序。

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages?$filter=Subject eq 'welcome' and importance eq 'normal'&$orderby=subject,importance,receivedDateTime desc
```


> [!NOTE] 
> 目录对象支持组合 `$orderby` 和 `$filter` 查询参数。 请参阅[Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。

## <a name="search-parameter"></a>search 参数

使用 `$search` 查询参数限制与搜索条件匹配的请求结果。 它的语法和行为因 API 操作而异。 若要查看不同资源之间 `$search` 的语法，请参阅 [使用$search查询参数匹配搜索条件](/graph/search-query-parameter)。

## <a name="select-parameter"></a>select 参数

使用 `$select` 查询参数返回一组不同于单个资源的默认集或资源集合的属性。 使用 `$select`，可以指定默认属性的子集或超集。

例如，检索登录用户的邮件时，可以指定仅返回 **from** 和 **subject** 属性：

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages?$select=from,subject
```


> **重要说明：** 一般来说，建议使用 `$select` 将查询返回的属性限制为应用所需的属性。 这对于可能返回大型结果集的查询尤为有用。 限制每行返回的属性将减少网络负载并帮助提升应用的性能。
>
> 在 `v1.0` 中，从 [directoryObject](/graph/api/resources/directoryobject) 派生的一些 Azure AD 资源（如 [user](/graph/api/resources/user) 和 [group](/graph/api/resources/group)）在读取时返回受限的默认属性子集。对于这些资源，必须使用 `$select` 将属性返回到默认集之外。  

## <a name="skip-parameter"></a>skip 参数

使用 `$skip` 查询参数设置要在集合开头跳过的项数。例如，以下请求返回按照创建日期排序的用户的事件，从集合中的第 21 个事件开始：

```msgraph-interactive
GET  https://graph.microsoft.com/v1.0/me/events?$orderby=createdDateTime&$skip=20
```


> **注意：** 一些 Microsoft Graph API 使用 `$skip` 实现分页，如 Outlook 邮件和日历（**message**、**event** 和 **calendar**）。 当查询结果跨多个页面时，这些 API 会返回 `@odata:nextLink` 属性，具有包含 `$skip` 参数的 URL。 可以使用此 URL 返回下一页结果。 若要了解详细信息，请参阅[分页](./paging.md)。
>
> 默认情况下，针对目录对象的高级查询所需的 **ConsistencyLevel** 标头不包含在后续页面请求中。必须在后续页面中显式设置它。

## <a name="skiptoken-parameter"></a>skipToken 参数

由于服务器端分页或由于使用 [`$top`](#top-parameter) 参数来限制响应的页面大小，致使一些请求返回多页数据。许多 Microsoft Graph API 使用 `skipToken` 查询参数来引用结果的后续页面。   
`$skiptoken` 参数包含引用下一页结果的不透明令牌，并在响应的 `@odata.nextLink` 属性中提供的 URL 中返回。若要了解详细信息，请参阅[分页](./paging.md)。
> **注意**:如果对目录对象的查询使用 OData 计数(在查询字符串中添加 `$count=true`)，则 `@odata.count` 属性将仅在第一页中出现。
>
> 默认情况下，针对目录对象的高级查询所需的 **ConsistencyLevel** 标头不包含在后续页面请求中。必须在后续页面中显式设置它。

## <a name="top-parameter"></a>top 参数

使用 `$top` 查询参数指定结果集的页面大小。 

如果结果集中还剩余多个项目，则响应正文将包含 `@odata.nextLink` 参数。 此参数包含可用于获取下一页结果的 URL。 若要了解详细信息，请参阅[分页](./paging.md)。 

最小值为 $top 1，最大值取决于相应的 API。  

例如，以下列表 [请求](/graph/api/user-list-messages) 返回用户邮箱中的前五条消息：

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages?$top=5
```


> 默认情况下，针对目录对象的高级查询所需的 **ConsistencyLevel** 标头不包含在后续页面请求中。必须在后续页面中显式设置它。

## <a name="error-handling-for-query-parameters"></a>查询参数的错误处理

如果不支持指定的查询参数，某些请求将返回错误消息。例如，不能对 `user/photo` 关系使用 `$expand`。 

```http
https://graph.microsoft.com/v1.0/me?$expand=photo
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

## <a name="see-also"></a>另请参阅

- [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)
- [使用$search查询参数匹配搜索条件](/graph/search-query-parameter)
- [查询参数限制](known-issues.md#query-parameters)
