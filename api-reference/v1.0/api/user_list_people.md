# <a name="list-people"></a><span data-ttu-id="08828-101">列出人员</span><span class="sxs-lookup"><span data-stu-id="08828-101">List people</span></span>

<span data-ttu-id="08828-102">检索按与[用户](../resources/user.md)的相关性排序的 [person](../resources/person.md) 对象集合，相关性由用户的通信和协作模式和业务关系决定。</span><span class="sxs-lookup"><span data-stu-id="08828-102">Retrieve a collection of [person](../resources/person.md) objects ordered by their relevance to the [user](../resources/user.md), which is determined by the user's communication and collaboration patterns and business relationships.</span></span>

<span data-ttu-id="08828-p101">可以通过 People API 获取此信息。有关示例，请参阅[示例](#examples)部分和[获取人员的相关信息](../../../concepts/people_example.md)一文。</span><span class="sxs-lookup"><span data-stu-id="08828-p101">You can get this information via the People API. For examples, see the [Examples](#examples) section and the article [Get relevant information about people](../../../concepts/people_example.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08828-105">先决条件</span><span class="sxs-lookup"><span data-stu-id="08828-105">Prerequisites</span></span>
<span data-ttu-id="08828-106">若要执行此 API，必须有以下**范围**：*People.Read* *People.Read.All*</span><span class="sxs-lookup"><span data-stu-id="08828-106">The following **scopes** are required to execute this API: *People.Read* *People.Read.All*</span></span>
 
## <a name="http-request"></a><span data-ttu-id="08828-107">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="08828-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/people
GET /users/{id | userPrincipalName}/people
```
## <a name="optional-query-parameters"></a><span data-ttu-id="08828-108">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="08828-108">Optional query parameters</span></span>
|<span data-ttu-id="08828-109">Name</span><span class="sxs-lookup"><span data-stu-id="08828-109">Name</span></span>|<span data-ttu-id="08828-110">值</span><span class="sxs-lookup"><span data-stu-id="08828-110">Value</span></span>|<span data-ttu-id="08828-111">说明</span><span class="sxs-lookup"><span data-stu-id="08828-111">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="08828-112">$filter</span><span class="sxs-lookup"><span data-stu-id="08828-112">$filter</span></span>|<span data-ttu-id="08828-113">string</span><span class="sxs-lookup"><span data-stu-id="08828-113">string</span></span>|<span data-ttu-id="08828-114">将响应限制为仅记录中包含指定条件的那些人员。</span><span class="sxs-lookup"><span data-stu-id="08828-114">Limits the response to only those people whose record contains the specified criteria.</span></span>|
|<span data-ttu-id="08828-115">$orderby</span><span class="sxs-lookup"><span data-stu-id="08828-115">$orderby</span></span>|<span data-ttu-id="08828-116">string</span><span class="sxs-lookup"><span data-stu-id="08828-116">string</span></span>|<span data-ttu-id="08828-p102">默认情况下，按与查询的相关性对响应中的人员进行排序。可以使用 *$orderby* 参数更改响应中的人员的顺序。</span><span class="sxs-lookup"><span data-stu-id="08828-p102">By default, the people in the response are sorted by their relevance to your query. You can change the order of the people in the response by using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="08828-119">$search</span><span class="sxs-lookup"><span data-stu-id="08828-119">$search</span></span>|<span data-ttu-id="08828-120">string</span><span class="sxs-lookup"><span data-stu-id="08828-120">string</span></span>|<span data-ttu-id="08828-p103">按名字或别名搜索人员。支持模糊匹配。</span><span class="sxs-lookup"><span data-stu-id="08828-p103">Search for people by name or alias. Supports fuzzy matching.</span></span>|
|<span data-ttu-id="08828-123">$select</span><span class="sxs-lookup"><span data-stu-id="08828-123">$select</span></span>|<span data-ttu-id="08828-124">string</span><span class="sxs-lookup"><span data-stu-id="08828-124">string</span></span>|<span data-ttu-id="08828-p104">要在响应中添加的属性列表（以逗号分隔）。为获得最佳结果，请仅选择所需属性的子集。</span><span class="sxs-lookup"><span data-stu-id="08828-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>|
|<span data-ttu-id="08828-127">$skip</span><span class="sxs-lookup"><span data-stu-id="08828-127">$skip</span></span>|<span data-ttu-id="08828-128">int</span><span class="sxs-lookup"><span data-stu-id="08828-128">int</span></span>|<span data-ttu-id="08828-p105">跳过前 n 个结果，可用于分页。使用 *$search* 时不支持此参数。</span><span class="sxs-lookup"><span data-stu-id="08828-p105">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>|
|<span data-ttu-id="08828-131">$top</span><span class="sxs-lookup"><span data-stu-id="08828-131">$top</span></span>|<span data-ttu-id="08828-132">int</span><span class="sxs-lookup"><span data-stu-id="08828-132">int</span></span>|<span data-ttu-id="08828-133">要返回的结果数。</span><span class="sxs-lookup"><span data-stu-id="08828-133">Number of results to be returned.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="08828-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="08828-134">Request headers</span></span>
| <span data-ttu-id="08828-135">名称</span><span class="sxs-lookup"><span data-stu-id="08828-135">Name</span></span>      |<span data-ttu-id="08828-136">说明</span><span class="sxs-lookup"><span data-stu-id="08828-136">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="08828-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="08828-137">Authorization</span></span>  | <span data-ttu-id="08828-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="08828-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="08828-140">接受</span><span class="sxs-lookup"><span data-stu-id="08828-140">Accept</span></span> | <span data-ttu-id="08828-141">application/json</span><span class="sxs-lookup"><span data-stu-id="08828-141">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="08828-142">请求正文</span><span class="sxs-lookup"><span data-stu-id="08828-142">Request body</span></span>
<span data-ttu-id="08828-143">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="08828-143">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="08828-144">响应</span><span class="sxs-lookup"><span data-stu-id="08828-144">Response</span></span>
<span data-ttu-id="08828-p107">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [person](../resources/person.md) 对象集合。响应可以包含一个人员对象或一个人员对象集合。</span><span class="sxs-lookup"><span data-stu-id="08828-p107">If successful, this method returns a `200 OK` response code and a collection of [person](../resources/person.md) objects in the response body. The response can contain one person object or a collection of person objects.</span></span> 
## <a name="examples"></a><span data-ttu-id="08828-147">示例</span><span class="sxs-lookup"><span data-stu-id="08828-147">Examples</span></span>

### <a name="get-a-collection-of-relevant-people"></a><span data-ttu-id="08828-148">获取相关人员集合。</span><span class="sxs-lookup"><span data-stu-id="08828-148">Get a collection of relevant people</span></span> 

<span data-ttu-id="08828-149">以下请求根据通信和协作模式及业务关系获取与登录用户 (`/me`) 相关度最高的人员。</span><span class="sxs-lookup"><span data-stu-id="08828-149">The following request gets the people most relevant to the signed-in user (`/me`), based on communication and collaboration patterns and business relationships.</span></span> 
<!-- {
  "blockType": "request",
  "name": "get_person"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/people/
```

<span data-ttu-id="08828-p108">以下示例显示了相应的响应。默认情况下，每个响应返回 10 个记录。可以使用 *$top* 查询参数更改此设置。本示例使用 *$top* 将响应限制为三个记录。</span><span class="sxs-lookup"><span data-stu-id="08828-p108">The following example shows the response. By default, each response returns 10 records. You can change this by using the *$top* query parameter. This example uses *$top* to limit the response to three records.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.person"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "8CE6E1DE-CB84-4BF5-971D-D3ECF452E2B5",
            "displayName": "Lorrie Frye",
            "givenName": "Lorrie",
            "surname": "Frye",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "Paralegal",
            "companyName": null,
            "yomiCompany": "",
            "department": "Legal",
            "officeLocation": "20/1109",
            "profession": "",
            "userPrincipalName": "Lorrief@contoso.onmicrosoft.com",
            "imAddress": "sip:Lorrief@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Lorrief@contoso.onmicrosoft.com",
                    "relevanceScore": 8
                }
            ],
            "phones": [
                {
                    "type": "Business",
                    "number": "+1 980 555 0101"
                }
            ],
            "postalAddresses": [],
            "websites": [],
            "personType": {
                "class": "Person",
                "subclass": "OrganizationUser"
            }
        },
        {
            "id": "5767393D-42BA-4E5C-BEE4-52BB25639CF4",
            "displayName": "Maynard Denman",
            "givenName": "Maynard",
            "surname": "Denman",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "Web Marketing Manager",
            "companyName": null,
            "yomiCompany": "",
            "department": "Sales & Marketing",
            "officeLocation": "20/1101",
            "profession": "",
            "userPrincipalName": "Maynardd@contoso.onmicrosoft.com",
            "imAddress": "sip:Maynardd@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Maynardd@contoso.onmicrosoft.com",
                    "relevanceScore": 8
                }
            ],
            "phones": [
                {
                    "type": "Business",
                    "number": "+1 918 555 0101"
                }
            ],
            "postalAddresses": [],
            "websites": [],
            "personType": {
                "class": "Person",
                "subclass": "OrganizationUser"
            }
        },
        {
            "id": "914B5191-11FA-4C0B-A354-0FA8C8EFD585",
            "displayName": "Darrel Halsey",
            "givenName": "Darrel",
            "surname": "Halsey",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "Attorney",
            "companyName": null,
            "yomiCompany": "",
            "department": "Legal",
            "officeLocation": "14/1102",
            "profession": "",
            "userPrincipalName": "Darrelh@contoso.onmicrosoft.com",
            "imAddress": "sip:Darrelh@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Darrelh@contoso.onmicrosoft.com",
                    "relevanceScore": 8
                }
            ],
            "phones": [
                {
                    "type": "Business",
                    "number": "+1 205 555 0103"
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
### <a name="search-other-users-relevant-people"></a><span data-ttu-id="08828-154">搜索其他用户的相关人员</span><span class="sxs-lookup"><span data-stu-id="08828-154">Search other user’s relevant people</span></span>

<span data-ttu-id="08828-p109">以下请求获取与登录用户组织中的其他人员相关度最高的人员。此请求需要具有 People.Read.All 权限。在本示例中显示了 Roscoe Seidel 的相关人员。</span><span class="sxs-lookup"><span data-stu-id="08828-p109">The following request gets the people most relevant to another person in the signed-in user's organization. This request requires the People.Read.All permission. In this example, Roscoe Seidel's relevant people are displayed.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_person"
}-->

```http
GET https://graph.microsoft.com/v1.0/users('roscoes@contoso.com')/people/
```

<span data-ttu-id="08828-p110">以下示例显示了相应的响应。默认情况下，每个响应返回 10 个记录。可以使用 *$top* 参数更改此设置。本示例使用 *$top* 将响应限制为三个记录。</span><span class="sxs-lookup"><span data-stu-id="08828-p110">The following example shows the response. By default, each response returns 10 records. You can change this by using the *$top* parameter. This example uses *$top* to limit the response to three records.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.person"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
     "value": [
        {
            "id": "56155636-703F-47F2-B657-C83F01F49BBC",
            "displayName": "Clifton Clemente",
            "givenName": "Clifton",
            "surname": "Clemente",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "Director",
            "companyName": null,
            "yomiCompany": "",
            "department": "Legal",
            "officeLocation": "19/2106",
            "profession": "",
            "userPrincipalName": "Cliftonc@contoso.onmicrosoft.com",
            "imAddress": "sip:Cliftonc@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Cliftonc@contoso.onmicrosoft.com",
                    "relevanceScore": 20
                }
            ],
            "phones": [
                {
                    "type": "Business",
                    "number": "+1 309 555 0101"
                }
            ],
            "postalAddresses": [],
            "websites": [],
            "personType": {
                "class": "Person",
                "subclass": "OrganizationUser"
            }
        },
        {
            "id": "6BF27D5A-AB4F-4C43-BED0-7DAD9EB0C1C4",
            "displayName": "Sheree Mitchell",
            "givenName": "Sheree",
            "surname": "Mitchell",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "Product Manager",
            "companyName": null,
            "yomiCompany": "",
            "department": "Sales & Marketing",
            "officeLocation": "20/2107",
            "profession": "",
            "userPrincipalName": "Shereem@contoso.onmicrosoft.com",
            "imAddress": "sip:shereem@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Shereem@contoso.onmicrosoft.com",
                    "relevanceScore": 10
                }
            ],
            "phones": [
                {
                    "type": "Business",
                    "number": "+1 918 555 0107"
                }
            ],
            "postalAddresses": [],
            "websites": [],
            "personType": {
                "class": "Person",
                "subclass": "OrganizationUser"
            }
        },
        {
            "id": "B3E5302D-EAF0-4E8B-8C6C-A2AE64B4B163",
            "displayName": "Vincent Matney",
            "givenName": "Vincent",
            "surname": "Matney",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "CVP Engineering",
            "companyName": null,
            "yomiCompany": "",
            "department": "Engineering",
            "officeLocation": "23/2102",
            "profession": "",
            "userPrincipalName": "Vincentm@contoso.onmicrosoft.com",
            "imAddress": "sip:vincentm@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Vincentm@contoso.onmicrosoft.com",
                    "relevanceScore": 10
                }
            ],
            "phones": [
                {
                    "type": "Business",
                    "number": "+1 502 555 0102"
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List people",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
