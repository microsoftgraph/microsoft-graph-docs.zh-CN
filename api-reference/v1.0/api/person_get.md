# <a name="get-person"></a>Get person

检索 [person](../resources/person.md) 对象的属性和关系。

可以通过 People API 获取此信息。有关示例，请参阅[示例](#examples)部分和[获取人员的相关信息](../../../concepts/people_example.md)一文。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。
 

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | People.Read、People.Read.All    |
|委派（个人 Microsoft 帐户） | People.Read    |
|应用程序 | People.Read.All |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->

```http
GET /me/people/?$search='{property_value}'
GET /me/people/?$filter={person_property} eq '{property_value}'
```

## <a name="optional-query-parameters"></a>可选的查询参数
|Name|值|说明|
|:---------------|:--------|:-------|
|$filter|string|将响应限制为仅记录中包含指定条件的那些人员。|
|$orderby|string|默认情况下，按与查询的相关性对响应中的人员进行排序。可以使用 *$orderby* 参数更改响应中的人员的顺序。|
|$search|string|按名字或别名搜索人员。支持模糊匹配。|
|$select|string|要在响应中添加的属性列表（以逗号分隔）。为获得最佳结果，请仅选择所需属性的子集。|
|$skip|int|跳过前 n 个结果，可用于分页。使用 *$search* 时不支持此参数。|
|$top|int|要返回的结果数。|

## <a name="parameters"></a>参数
| 参数 |类型       |说明|
|:----------|:----------|:----------|
|property_value|字符串     |要匹配的扩展属性的值。**HTTP 请求**部分中列出的必需的参数。|
|person_property|字符串    |要匹配的人员属性。**HTTP 请求**部分中列出的必需的参数。|

## <a name="request-headers"></a>请求标头
| 名称      |说明|
|:----------|:----------|
| Authorization  | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。
## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [person](../resources/person.md) 对象。响应可以包含一个人员实例或一个人员实例集合。 
## <a name="examples"></a>示例
### <a name="perform-a-search"></a>执行搜索 
以下请求搜索名为“Irene McGowan”的人员。 

<!-- {
  "blockType": "request",
  "name": "get_person"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="Irene McGowan"
```

以下示例显示了相应的响应。 

<!-- {
  "blockType": "response",
  "name": "get_person",
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
           "personType": [
               {
                    "class": "Person",
                    "subclass": "OrganizationUser"
                }
            ]
       }
   ]
}
```
### <a name="select-the-fields-to-return-in-a-filtered-response"></a>选择要在经过筛选的响应中返回的字段 
可以结合 *$select* 和 *$filter* 参数创建自定义用户相关人员列表，并且只获取应用程序需要的字段。 

以下示例获取显示名称等于指定名称的人员的 **displayName** 和 **scoredEmailAddresses**。在本示例中，只返回显示名称等于“Lorrie Frye”的人员。

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/v1.0/me/people/?$select=displayName,scoredEmailAddresses&$filter=displayName eq 'Lorrie Frye'
```

下面是示例请求的正确编码 URL。

<!-- {
  "blockType": "request",
  "name": "get_person_select_and_filter"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/people/?$select=displayName,scoredEmailAddresses&$filter=displayName%20eq%20'Lorrie Frye'
```

下面展示了示例响应。 

<!-- {
  "blockType": "response",
  "name": "get_person_select_and_filter",
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
            "id": "8CE6E1DE-CB84-4BF5-971D-D3ECF452E2B5",
            "displayName": "Lorrie Frye",
            "scoredEmailAddresses": [
                {
                    "address": "Lorrief@contoso.onmicrosoft.com",
                    "relevanceScore": 8.0
                }
            ]
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get person",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
