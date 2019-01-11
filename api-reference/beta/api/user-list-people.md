---
title: 列出人员
description: 检索按其与用户，这由用户的通信和协作模式和业务关系的相关性排序的 person 对象的列表。
author: simonhult
localization_priority: Normal
ms.openlocfilehash: 3bd9c8cdd3737cbd8d96fd4f9b24f5382ce04793
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872777"
---
# <a name="list-people"></a>列出人员

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

检索按给[用户](../resources/user.md)，它由用户的通信和协作模式和业务关系其相关性排序的[person](../resources/person.md)对象的列表。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | People.Read    |
|委派（个人 Microsoft 帐户） | People.Read    |
|应用程序 | 不支持。 |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /me/people
GET /users/{id | userPrincipalName}/people
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持以下 OData 查询参数，以帮助自定义响应。

|名称|值|说明|
|:---------------|:--------|:-------|
|$filter|string|将响应限制为仅记录中包含指定条件的那些人员。|
|$orderby|string|默认情况下，按与查询的相关程度对响应中的人员进行排序。 可以使用 *$orderby* 参数更改响应中的人员排序。|
|$search|string|按姓名或别名搜索人员。 支持模糊匹配。 参数仅适用于不搜索已登录的用户相关人员搜索相关的其他用户的人员。 此外支持`topic`要查找人员关键字基于提取与此人的电子邮件对话的主题。 请参阅*Perform 模糊搜索*节[获取有关人员的相关信息](/graph/people-example#perform-a-fuzzy-search)的信息和示例。|
|$select|string|要在响应中添加的属性列表（以逗号分隔）。为获得最佳结果，请仅选择所需属性的子集。|
|$skip|整数|跳过前 n 个结果，可用于分页。使用 *$search* 时不支持此参数。|
|$top|整数|要返回的结果数。|

## <a name="request-headers"></a>请求标头

| 名称      |说明|
|:----------|:----------|
| Authorization  | Bearer {token}。必需。 |
| Accept | application/json |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法返回`200 OK`响应代码和响应正文中的[联系人](../resources/person.md)对象的集合。

## <a name="examples"></a>示例

### <a name="browse"></a>浏览

本节中的请求获得人员已登录的用户与最相关 (`/me`)、 基于通信、 协作和业务关系。

默认情况下，每个响应都会返回10条记录，但您可以 改变这点 使用 *$顶部* 参数。 这些请求需要 People.Read 的权限。

#### <a name="request"></a>请求

下面是请求的默认的示例。
<!-- {
  "blockType": "request",
  "name": "get_person_collection_beta"
}-->

```http
GET https://graph.microsoft.com/beta/me/people
```

#### <a name="response"></a>响应

下面展示了示例响应。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。

<!-- {
  "blockType": "response",
  "name": "get_person_collection_beta",
  "truncated": true,
  "@odata.type": "microsoft.graph.person",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1326

{
    "value": [
        {
            "id": "33b43a5b-87d6-41ec-91f8-a2610048105f",
            "displayName": "Marketing",
            "givenName": null,
            "surname": null,
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "title": null,
            "companyName": null,
            "yomiCompany": "",
            "department": null,
            "officeLocation": null,
            "profession": "",
            "mailboxType": "GroupMailbox",
            "personType": "ModernGroup",
            "userPrincipalName": "",
            "emailAddresses": [
                {
                    "address": "Marketing@contoso.com",
                    "rank": 30
                }
            ],
            "phones": [],
            "postalAddresses": [],
            "websites": [],
            "sources": [
                {
                    "type": "Directory"
                }
            ]
        },
        {
            "id": "e3d0513b-449e-4198-ba6f-bd97ae7cae85",
            "displayName": "Isaiah Langer",
            "givenName": "Isaiah",
            "surname": "Langer",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "title": "Web Marketing Manager",
            "companyName": null,
            "yomiCompany": "",
            "department": "Sales & Marketing",
            "officeLocation": "20/1101",
            "profession": "",
            "mailboxType": "Mailbox",
            "personType": "Person",
            "userPrincipalName": "IsaiahL@contoso.com",
            "emailAddresses": [
                {
                    "address": "IsaiahL@contoso.com",
                    "rank": 20
                }
            ],
            "phones": [
                {
                    "type": "business",
                    "number": "+1 918 555 0101"
                }
            ],
            "postalAddresses": [],
            "websites": [],
            "sources": [
                {
                    "type": "Directory"
                }
            ]
        }
    ]
}
```

#### <a name="requesting-a-subsequent-page-of-people"></a>请求人员的后续页面。

如果第一个响应未包含相关人员的完整列表，可以使用 *$top* 和 *$skip* 发出第二个请求，以请求其他信息页面。如果上一个请求包含其他信息，则下一个请求从服务器获取下一个人员页面。

```http
GET https://graph.microsoft.com/beta/me/people/?$top=10&$skip=10
```

#### <a name="sort-the-response"></a>对响应进行排序

默认情况下，按与查询的相关程度对响应中的人员进行排序。 可以使用 *$orderby* 参数更改响应中的人员排序。 此查询选择与您最相关的人员，按他们的显示名称对他们进行排序，然后返回排序列表中的前10个人。

```http
GET https://graph.microsoft.com/beta/me/people/?$orderby=DisplayName
```

#### <a name="changing-the-number-of-people-returned-and-the-fields-returned"></a>更改返回的人数和返回的字段

可以通过设置 *$top* 参数更改响应中返回的人员数。

下面的示例请求与最相关的 1,000 人员`/me`。 此外将请求限制后从服务器发送的请求只有的人员的显示名称的数据量。

```http
GET https://graph.microsoft.com/beta/me/people/?$top=1000&$select=DisplayName
```

#### <a name="selecting-the-fields-to-return"></a>选择要返回的字段

您可以限制从服务器返回通过使用 *$select*参数选择一个或多个字段的数据量。 该 *@ odata.id* 字段总会返回。

下面的示例限制对*DisplayName*和*电子邮件地址*的 10 个最相关人员的响应。

```http
GET https://graph.microsoft.com/beta/me/people/?$select=DisplayName,EmailAddresses
```

#### <a name="using-a-filter-to-limit-the-response"></a>使用过滤来限制响应

可以使用 *$filter* 参数将响应限制为记录中包含指定条件的那些人员。

下面的查询限制的响应人员与源"目录"。

```http
GET https://graph.microsoft.com/beta/me/people/?$filter=Sources/Any (source: source/Type  eq 'Directory')
```

#### <a name="selecting-the-fields-to-return-in-a-filtered-response"></a>选择要筛选的响应中返回的字段

可以结合 *$select* 和 *$filter* 参数创建自定义用户相关人员列表，并且只获取应用程序需要的字段。

下面的示例获取的*DisplayName*和其显示名称等于指定的名称的人员的*电子邮件地址*。 在本示例中，只返回显示名称等于“Nestor Kellum”的人。

```http
+GET https://graph.microsoft.com/beta/me/people/?$select=DisplayName,EmailAddresses&$filter=DisplayName eq 'Nestor Kellum'
```

### <a name="search-people"></a>搜索人员

本节中的请求也会获得人员最相关的已登录的用户 (`/me`)。 搜索请求需要 People.Read 的权限。

#### <a name="using-search-to-select-people"></a>使用搜索来选择的人员

使用 *$search* 参数选择符合某组特定条件的人员。

下面的搜索查询返回与相关人员`/me`其 GivenName 或姓字母开头"j"。

```http
GET https://graph.microsoft.com/beta/me/people/?$search=j
```

#### <a name="using-search-to-specify-a-relevant-topic"></a>使用搜索来指定相关主题

以下请求返回与相关人员`/me`名称中包含"ma"和谁具有关联"规划的功能。"

```http
GET https://graph.microsoft.com/beta/me/people/?$search="ma topic: feature planning"
```

#### <a name="performing-a-fuzzy-search"></a>执行模糊搜索

以下请求执行名为"Hermaini 大厅。"的人员搜索 因为没有名为"Herminia 轮廓"与已登录的用户相关的人员，则返回"Herminia 轮廓"的信息。

```http
GET https://graph.microsoft.com/beta/me/people/?$search="hermaini hall"
```

### <a name="related-people"></a>相关的人员

以下请求用户的组织中获取人员最相关的其他人。 该请求需要 User.ReadBasic.All People.Read.All 权限。 本示例中，显示 Nestor Kellum 相关人员。

```http
GET https://graph.microsoft.com/beta/users('nestork@contoso.com')/people/
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List people",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
