# <a name="list-people"></a><span data-ttu-id="7f888-101">列出人员</span><span class="sxs-lookup"><span data-stu-id="7f888-101">List people</span></span>

<span data-ttu-id="7f888-102">检索按与[用户](../resources/user.md)的相关性排序的 [person](../resources/person.md) 对象集合，相关性由用户的通信和协作模式和业务关系决定。</span><span class="sxs-lookup"><span data-stu-id="7f888-102">Retrieve a collection of [person](../resources/person.md) objects ordered by their relevance to the [user](../resources/user.md), which is determined by the user's communication and collaboration patterns and business relationships.</span></span>

<span data-ttu-id="7f888-p101">可以通过 People API 获取此信息。有关示例，请参阅[示例](#examples)部分和[获取人员的相关信息](../../../concepts/people_example.md)一文。</span><span class="sxs-lookup"><span data-stu-id="7f888-p101">You can get this information via the People API. For examples, see the [Examples](#examples) section and the article [Get relevant information about people](../../../concepts/people_example.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7f888-105">权限</span><span class="sxs-lookup"><span data-stu-id="7f888-105">Permissions</span></span>
<span data-ttu-id="7f888-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="7f888-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>
 

|<span data-ttu-id="7f888-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="7f888-108">Permission type</span></span>      | <span data-ttu-id="7f888-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7f888-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f888-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7f888-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7f888-111">People.Read、People.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f888-111">People.Read, People.Read.All</span></span>    |
|<span data-ttu-id="7f888-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7f888-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f888-113">People.Read</span><span class="sxs-lookup"><span data-stu-id="7f888-113">People.Read</span></span>    |
|<span data-ttu-id="7f888-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="7f888-114">Application</span></span> | <span data-ttu-id="7f888-115">People.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f888-115">People.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f888-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7f888-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/people
GET /users/{id | userPrincipalName}/people
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7f888-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7f888-117">Optional query parameters</span></span>
|<span data-ttu-id="7f888-118">Name</span><span class="sxs-lookup"><span data-stu-id="7f888-118">Name</span></span>|<span data-ttu-id="7f888-119">值</span><span class="sxs-lookup"><span data-stu-id="7f888-119">Value</span></span>|<span data-ttu-id="7f888-120">说明</span><span class="sxs-lookup"><span data-stu-id="7f888-120">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="7f888-121">$filter</span><span class="sxs-lookup"><span data-stu-id="7f888-121">$filter</span></span>|<span data-ttu-id="7f888-122">string</span><span class="sxs-lookup"><span data-stu-id="7f888-122">string</span></span>|<span data-ttu-id="7f888-123">将响应限制为仅记录中包含指定条件的那些人员。</span><span class="sxs-lookup"><span data-stu-id="7f888-123">Limits the response to only those people whose record contains the specified criteria.</span></span>|
|<span data-ttu-id="7f888-124">$orderby</span><span class="sxs-lookup"><span data-stu-id="7f888-124">$orderby</span></span>|<span data-ttu-id="7f888-125">string</span><span class="sxs-lookup"><span data-stu-id="7f888-125">string</span></span>|<span data-ttu-id="7f888-p103">默认情况下，按与查询的相关性对响应中的人员进行排序。可以使用 *$orderby* 参数更改响应中的人员的顺序。</span><span class="sxs-lookup"><span data-stu-id="7f888-p103">By default, the people in the response are sorted by their relevance to your query. You can change the order of the people in the response by using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="7f888-128">$search</span><span class="sxs-lookup"><span data-stu-id="7f888-128">$search</span></span>|<span data-ttu-id="7f888-129">string</span><span class="sxs-lookup"><span data-stu-id="7f888-129">string</span></span>|<span data-ttu-id="7f888-p104">按名字或别名搜索人员。支持模糊匹配。</span><span class="sxs-lookup"><span data-stu-id="7f888-p104">Search for people by name or alias. Supports fuzzy matching.</span></span>|
|<span data-ttu-id="7f888-132">$select</span><span class="sxs-lookup"><span data-stu-id="7f888-132">$select</span></span>|<span data-ttu-id="7f888-133">string</span><span class="sxs-lookup"><span data-stu-id="7f888-133">string</span></span>|<span data-ttu-id="7f888-p105">要在响应中添加的属性列表（以逗号分隔）。为获得最佳结果，请仅选择所需属性的子集。</span><span class="sxs-lookup"><span data-stu-id="7f888-p105">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>|
|<span data-ttu-id="7f888-136">$skip</span><span class="sxs-lookup"><span data-stu-id="7f888-136">$skip</span></span>|<span data-ttu-id="7f888-137">int</span><span class="sxs-lookup"><span data-stu-id="7f888-137">int</span></span>|<span data-ttu-id="7f888-p106">跳过前 n 个结果，可用于分页。使用 *$search* 时不支持此参数。</span><span class="sxs-lookup"><span data-stu-id="7f888-p106">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>|
|<span data-ttu-id="7f888-140">$top</span><span class="sxs-lookup"><span data-stu-id="7f888-140">$top</span></span>|<span data-ttu-id="7f888-141">int</span><span class="sxs-lookup"><span data-stu-id="7f888-141">int</span></span>|<span data-ttu-id="7f888-142">要返回的结果数。</span><span class="sxs-lookup"><span data-stu-id="7f888-142">Number of results to be returned.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="7f888-143">请求标头</span><span class="sxs-lookup"><span data-stu-id="7f888-143">Request headers</span></span>
| <span data-ttu-id="7f888-144">名称</span><span class="sxs-lookup"><span data-stu-id="7f888-144">Name</span></span>      |<span data-ttu-id="7f888-145">说明</span><span class="sxs-lookup"><span data-stu-id="7f888-145">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7f888-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f888-146">Authorization</span></span>  | <span data-ttu-id="7f888-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7f888-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7f888-149">接受</span><span class="sxs-lookup"><span data-stu-id="7f888-149">Accept</span></span> | <span data-ttu-id="7f888-150">application/json</span><span class="sxs-lookup"><span data-stu-id="7f888-150">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="7f888-151">请求正文</span><span class="sxs-lookup"><span data-stu-id="7f888-151">Request body</span></span>
<span data-ttu-id="7f888-152">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7f888-152">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="7f888-153">响应</span><span class="sxs-lookup"><span data-stu-id="7f888-153">Response</span></span>
<span data-ttu-id="7f888-p108">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [person](../resources/person.md) 对象集合。响应可以包含一个人员对象或一个人员对象集合。</span><span class="sxs-lookup"><span data-stu-id="7f888-p108">If successful, this method returns a `200 OK` response code and a collection of [person](../resources/person.md) objects in the response body. The response can contain one person object or a collection of person objects.</span></span> 
## <a name="examples"></a><span data-ttu-id="7f888-156">示例</span><span class="sxs-lookup"><span data-stu-id="7f888-156">Examples</span></span>

### <a name="get-a-collection-of-relevant-people"></a><span data-ttu-id="7f888-157">获取相关人员集合。</span><span class="sxs-lookup"><span data-stu-id="7f888-157">Get a collection of relevant people</span></span> 

<span data-ttu-id="7f888-158">以下请求根据通信和协作模式及业务关系获取与登录用户 (`/me`) 相关度最高的人员。</span><span class="sxs-lookup"><span data-stu-id="7f888-158">The following request gets the people most relevant to the signed-in user (`/me`), based on communication and collaboration patterns and business relationships.</span></span> 
<!-- {
  "blockType": "request",
  "name": "get_person_collection"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/people/
```

<span data-ttu-id="7f888-p109">以下示例显示了相应的响应。默认情况下，每个响应返回 10 个记录。可以使用 *$top* 查询参数更改此设置。本示例使用 *$top* 将响应限制为三个记录。</span><span class="sxs-lookup"><span data-stu-id="7f888-p109">The following example shows the response. By default, each response returns 10 records. You can change this by using the *$top* query parameter. This example uses *$top* to limit the response to three records.</span></span>
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
                    "relevanceScore": 8.0
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
            "personType": [
                {
                    "class": "Person",
                    "subclass": "OrganizationUser"
                }
            ]
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
                    "relevanceScore": 8.0
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
            "personType": [
                {
                    "class": "Person",
                    "subclass": "OrganizationUser"
                }
            ]
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
                    "relevanceScore": 8.0
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
### <a name="search-other-users-relevant-people"></a><span data-ttu-id="7f888-163">搜索其他用户的相关人员</span><span class="sxs-lookup"><span data-stu-id="7f888-163">Search other user’s relevant people</span></span>

<span data-ttu-id="7f888-p110">以下请求获取与登录用户组织中的其他人员相关度最高的人员。此请求需要具有 People.Read.All 权限。在本示例中显示了 Roscoe Seidel 的相关人员。</span><span class="sxs-lookup"><span data-stu-id="7f888-p110">The following request gets the people most relevant to another person in the signed-in user's organization. This request requires the People.Read.All permission. In this example, Roscoe Seidel's relevant people are displayed.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_other_person"
}-->

```http
GET https://graph.microsoft.com/v1.0/users('roscoes@contoso.com')/people/
```

<span data-ttu-id="7f888-p111">以下示例显示了相应的响应。默认情况下，每个响应返回 10 个记录。可以使用 *$top* 参数更改此设置。本示例使用 *$top* 将响应限制为三个记录。</span><span class="sxs-lookup"><span data-stu-id="7f888-p111">The following example shows the response. By default, each response returns 10 records. You can change this by using the *$top* parameter. This example uses *$top* to limit the response to three records.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_other_person",
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
                    "relevanceScore": 20.0
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
            "personType": [
                {
                    "class": "Person",
                    "subclass": "OrganizationUser"
                }
            ]
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
                    "relevanceScore": 10.0
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
            "personType": [
                {
                    "class": "Person",
                    "subclass": "OrganizationUser"
                }
            ]
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
                    "relevanceScore": 10.0
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List people",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
