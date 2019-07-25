---
title: 列出人员
description: 检索按其与用户的相关性排序的人员对象列表, 该列表由用户的通信和协作模式以及业务关系决定。
author: dkershaw10
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: d3b7f815fb75b17f88db234cae4fdea626d34bfb
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867134"
---
# <a name="list-people"></a>列出人员

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检索按其与[用户](../resources/user.md)的相关性排序的[人员](../resources/person.md)对象列表, 该列表由用户的通信和协作模式以及业务关系决定。

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

此方法支持以下 OData 查询参数来帮助自定义响应。

|名称|值|说明|
|:---------------|:--------|:-------|
|$filter|string|将响应限制为仅记录中包含指定条件的那些人员。|
|$orderby|string|默认情况下，按与查询的相关程度对响应中的人员进行排序。 可以使用 *$orderby* 参数更改响应中的人员排序。|
|$search|string|按姓名或别名搜索人员。 支持模糊匹配。 参数仅适用于搜索已登录用户的相关人员，而不适用于搜索与其他用户相关的人员。 此外还支持 `topic` 关键字，以根据从与此人的电子邮件对话中提取的主题查找人员。 有关信息和示例，请参阅“[获取相关人员的信息](/graph/people-example#perform-a-fuzzy-search)”的“*执行模糊搜索*”部分。|
|$select|string|要在响应中添加的属性列表（以逗号分隔）。为获得最佳结果，请仅选择所需属性的子集。|
|$skip|int|跳过前 n 个结果，可用于分页。使用 *$search* 时不支持此参数。|
|$top|int|要返回的结果数。|

## <a name="request-headers"></a>请求标头

| 名称      |说明|
|:----------|:----------|
| Authorization  | Bearer {token}。必需。 |
| 接受 | application/json |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功, 此方法在响应`200 OK`正文中返回响应代码和[person](../resources/person.md)对象集合。

## <a name="examples"></a>示例

### <a name="browse"></a>定位

本节中的请求将根据通信、协作和业务关系获取与登录用户最`/me`相关的人员 ()。

默认情况下，每个响应都会返回10条记录，但您可以 改变这点 使用 *$顶部* 参数。 这些请求需要人员读取权限。

#### <a name="request"></a>请求

以下是默认请求的示例。

# <a name="httptabhttp"></a>[HTTP.SYS](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_person_collection_beta"
}-->

```http
GET https://graph.microsoft.com/beta/me/people
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-person-collection-beta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-person-collection-beta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目标-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-person-collection-beta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-person-collection-beta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


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

下面的示例请求与最相关的1000人`/me`。 请求还通过仅请求用户的显示名称来限制从服务器发送回的数据量。

```http
GET https://graph.microsoft.com/beta/me/people/?$top=1000&$select=DisplayName
```

#### <a name="selecting-the-fields-to-return"></a>选择要返回的字段

您可以通过使用 *$select*参数选择一个或多个字段来限制从服务器返回的数据量。 该 *@ odata.id* 字段总会返回。

下面的示例将响应限制为10个最相关人员的*DisplayName*和*EmailAddress* 。

```http
GET https://graph.microsoft.com/beta/me/people/?$select=DisplayName,EmailAddresses
```

#### <a name="using-a-filter-to-limit-the-response"></a>使用过滤来限制响应

可以使用 *$filter* 参数将响应限制为记录中包含指定条件的那些人员。

以下查询将响应限制为对源 "Directory" 的人员的响应。

```http
GET https://graph.microsoft.com/beta/me/people/?$filter=Sources/Any (source: source/Type  eq 'Directory')
```

#### <a name="selecting-the-fields-to-return-in-a-filtered-response"></a>在筛选的响应中选择要返回的字段

可以结合 *$select* 和 *$filter* 参数创建自定义用户相关人员列表，并且只获取应用程序需要的字段。

下面的示例获取其显示名称等于指定名称的用户的*DisplayName*和*EmailAddress* 。 在本示例中，只返回显示名称等于“Nestor Kellum”的人。

```http
+GET https://graph.microsoft.com/beta/me/people/?$select=DisplayName,EmailAddresses&$filter=DisplayName eq 'Nestor Kellum'
```

### <a name="search-people"></a>搜索人员

此部分中的请求还可以获取与登录用户最相关的人员 (`/me`)。 搜索请求需要人员读取权限。

#### <a name="using-search-to-select-people"></a>使用 "搜索" 选择人员

使用 *$search* 参数选择符合某组特定条件的人员。

下面的搜索查询返回与`/me`其 GivenName 或姓以字母 "j" 开头的人员相关的人员。

```http
GET https://graph.microsoft.com/beta/me/people/?$search=j
```

#### <a name="using-search-to-specify-a-relevant-topic"></a>使用搜索来指定相关主题

以下请求返回相关人员, `/me`其名称包含 "ma", 以及与 "功能计划" 有关联的人员。

```http
GET https://graph.microsoft.com/beta/me/people/?$search="ma topic: feature planning"
```

#### <a name="performing-a-fuzzy-search"></a>执行模糊搜索

下面的请求搜索名为 "Hermaini 厅" 的人。 由于存在与登录用户相关的名为 "所以凸" 的人员, 因此返回 "所以凸" 的信息。

```http
GET https://graph.microsoft.com/beta/me/people/?$search="hermaini hall"
```

### <a name="related-people"></a>相关人员

以下请求获取与用户组织中的其他人最相关的人员。 此请求需要 User.readbasic.all 的所有人。读取。 All 权限。 在此示例中, 将显示 Nestor Kellum 的相关人员。

```http
GET https://graph.microsoft.com/beta/users('nestork@contoso.com')/people/
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List people",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
