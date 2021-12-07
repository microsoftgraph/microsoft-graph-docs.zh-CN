---
title: 列出人员
description: 检索一组 person 对象，这些对象按与 user 的相关程度进行排序，相关程度由用户的通信和协作模式以及业务关系决定。
author: anthona
ms.localizationpriority: high
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 9910a5fe6853f9baf9bd7005fb1b242e68f652aa
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322168"
---
# <a name="list-people"></a>列出人员

命名空间：microsoft.graph

检索一组 [person](../resources/person.md) 对象，这些对象按与 [user](../resources/user.md) 的相关程度进行排序，相关程度由用户的通信和协作模式以及业务关系决定。

可以通过 People API 获取此信息。有关示例，请参阅[示例](#examples)部分和[获取人员的相关信息](/graph/people-example)一文。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | People.Read、People.Read.All    |
|委派（个人 Microsoft 帐户） | People.Read    |
|应用程序 | People.Read.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /me/people
GET /users/{id | userPrincipalName}/people
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持使用 [OData 查询参数](/graph/query-parameters)自定义响应，如[获取人员的相关信息](/graph/people-example)一文中的示例所示。

|名称|值|说明|
|:---------------|:--------|:-------|
|$filter|string|将响应限制为仅记录中包含指定条件的那些人员。|
|$orderby|string|默认情况下，按与查询的相关程度对响应中的人员进行排序。可以使用 *$orderby* 参数更改响应中的人员排序。|
|$search|string|按姓名或别名搜索人员。 支持模糊匹配。 参数仅适用于搜索已登录用户的相关人员，而不适用于搜索与其他用户相关的人员。 此外还支持 `topic` 关键字，以根据从与此人的电子邮件对话中提取的主题查找人员。 有关信息和示例，请参阅“[获取相关人员的信息](/graph/people-example#perform-a-fuzzy-search)”的“*执行模糊搜索*”部分。 |
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

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [person](../resources/person.md) 对象集合。响应可以包含一个人员对象或一个人员对象集合。

## <a name="examples"></a>示例

#### <a name="request"></a>请求

下面展示了示例请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_person_collection"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/people
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-person-collection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-person-collection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-person-collection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-person-collection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-person-collection-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "name": "get_person_collection",
  "truncated": true,
  "@odata.type": "microsoft.graph.person",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

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
            "jobTitle": null,
            "companyName": null,
            "yomiCompany": "",
            "department": null,
            "officeLocation": null,
            "profession": "",
            "userPrincipalName": "",
            "imAddress": null,
            "scoredEmailAddresses": [
                {
                    "address": "Marketing@contoso.com",
                    "relevanceScore": 30.0
                }
            ],
            "phones": [],
            "postalAddresses": [],
            "websites": [],
            "personType": {
                "class": "Group",
                "subclass": "UnifiedGroup"
            }
        },
        {
            "id": "e3d0513b-449e-4198-ba6f-bd97ae7cae85",
            "displayName": "Isaiah Langer",
            "givenName": "Isaiah",
            "surname": "Langer",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "Web Marketing Manager",
            "companyName": null,
            "yomiCompany": "",
            "department": "Sales & Marketing",
            "officeLocation": "20/1101",
            "profession": "",
            "userPrincipalName": "IsaiahL@contoso.com",
            "imAddress": "sip:isaiahl@contoso.com",
            "scoredEmailAddresses": [
                {
                    "address": "IsaiahL@contoso.com",
                    "relevanceScore": 20.0
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
            "personType": {
                "class": "Person",
                "subclass": "OrganizationUser"
            }
        }
    ]
}
```

有关更多示例，请参阅[获取人员的相关信息](/graph/people-example)一文。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List people",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

