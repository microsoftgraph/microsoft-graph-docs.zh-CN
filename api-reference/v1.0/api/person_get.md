# <a name="get-person"></a><span data-ttu-id="5a99b-101">Get person</span><span class="sxs-lookup"><span data-stu-id="5a99b-101">Get person</span></span>

<span data-ttu-id="5a99b-102">检索 [person](../resources/person.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5a99b-102">Retrieve the properties and relationships of [plannerAssignedToTaskBoardTaskFormat](../resources/person.md) object.</span></span>

<span data-ttu-id="5a99b-p101">可以通过 People API 获取此信息。有关示例，请参阅[示例](#examples)部分和[获取人员的相关信息](../../../concepts/people_example.md)一文。</span><span class="sxs-lookup"><span data-stu-id="5a99b-p101">You can get this information via the People API. For examples, see the [Examples](#examples) section and the article [Get relevant information about people](../../../concepts/people_example.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5a99b-105">先决条件</span><span class="sxs-lookup"><span data-stu-id="5a99b-105">Prerequisites</span></span>
<span data-ttu-id="5a99b-106">执行此部分 API 需要以下**权限**：*People.Read*；*People.Read.All*</span><span class="sxs-lookup"><span data-stu-id="5a99b-106">The following **permissions** are required to execute portions of this API: *People.Read*; *People.Read.All*</span></span>
 
## <a name="http-request"></a><span data-ttu-id="5a99b-107">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5a99b-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/people/?$search='{property_value}'
GET /me/people/?$filter={person_property} eq '{property_value}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5a99b-108">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5a99b-108">Optional query parameters</span></span>
|<span data-ttu-id="5a99b-109">Name</span><span class="sxs-lookup"><span data-stu-id="5a99b-109">Name</span></span>|<span data-ttu-id="5a99b-110">值</span><span class="sxs-lookup"><span data-stu-id="5a99b-110">Value</span></span>|<span data-ttu-id="5a99b-111">说明</span><span class="sxs-lookup"><span data-stu-id="5a99b-111">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="5a99b-112">$filter</span><span class="sxs-lookup"><span data-stu-id="5a99b-112">$filter</span></span>|<span data-ttu-id="5a99b-113">string</span><span class="sxs-lookup"><span data-stu-id="5a99b-113">string</span></span>|<span data-ttu-id="5a99b-114">将响应限制为仅记录中包含指定条件的那些人员。</span><span class="sxs-lookup"><span data-stu-id="5a99b-114">Limits the response to only those people whose record contains the specified criteria.</span></span>|
|<span data-ttu-id="5a99b-115">$orderby</span><span class="sxs-lookup"><span data-stu-id="5a99b-115">$orderby</span></span>|<span data-ttu-id="5a99b-116">string</span><span class="sxs-lookup"><span data-stu-id="5a99b-116">string</span></span>|<span data-ttu-id="5a99b-p102">默认情况下，按与查询的相关性对响应中的人员进行排序。可以使用 *$orderby* 参数更改响应中的人员的顺序。</span><span class="sxs-lookup"><span data-stu-id="5a99b-p102">By default, the people in the response are sorted by their relevance to your query. You can change the order of the people in the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="5a99b-119">$search</span><span class="sxs-lookup"><span data-stu-id="5a99b-119">$search</span></span>|<span data-ttu-id="5a99b-120">string</span><span class="sxs-lookup"><span data-stu-id="5a99b-120">string</span></span>|<span data-ttu-id="5a99b-p103">按名字或别名搜索人员。支持模糊匹配。</span><span class="sxs-lookup"><span data-stu-id="5a99b-p103">Search for people by name or alias. Supports fuzzy matching.</span></span>|
|<span data-ttu-id="5a99b-123">$select</span><span class="sxs-lookup"><span data-stu-id="5a99b-123">$select</span></span>|<span data-ttu-id="5a99b-124">string</span><span class="sxs-lookup"><span data-stu-id="5a99b-124">string</span></span>|<span data-ttu-id="5a99b-p104">要在响应中添加的属性列表（以逗号分隔）。为获得最佳结果，请仅选择所需属性的子集。</span><span class="sxs-lookup"><span data-stu-id="5a99b-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>|
|<span data-ttu-id="5a99b-127">$skip</span><span class="sxs-lookup"><span data-stu-id="5a99b-127">$skip</span></span>|<span data-ttu-id="5a99b-128">int</span><span class="sxs-lookup"><span data-stu-id="5a99b-128">int</span></span>|<span data-ttu-id="5a99b-p105">跳过前 n 个结果，可用于分页。使用 *$search* 时不支持此参数。</span><span class="sxs-lookup"><span data-stu-id="5a99b-p105">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>|
|<span data-ttu-id="5a99b-131">$top</span><span class="sxs-lookup"><span data-stu-id="5a99b-131">$top</span></span>|<span data-ttu-id="5a99b-132">int</span><span class="sxs-lookup"><span data-stu-id="5a99b-132">int</span></span>|<span data-ttu-id="5a99b-133">要返回的结果数。</span><span class="sxs-lookup"><span data-stu-id="5a99b-133">Number of results to be returned.</span></span>|

## <a name="parameters"></a><span data-ttu-id="5a99b-134">参数</span><span class="sxs-lookup"><span data-stu-id="5a99b-134">Parameters</span></span>
| <span data-ttu-id="5a99b-135">参数</span><span class="sxs-lookup"><span data-stu-id="5a99b-135">Parameter</span></span> |<span data-ttu-id="5a99b-136">类型</span><span class="sxs-lookup"><span data-stu-id="5a99b-136">Type</span></span>       |<span data-ttu-id="5a99b-137">说明</span><span class="sxs-lookup"><span data-stu-id="5a99b-137">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="5a99b-138">property_value</span><span class="sxs-lookup"><span data-stu-id="5a99b-138">property_value</span></span>|<span data-ttu-id="5a99b-139">String</span><span class="sxs-lookup"><span data-stu-id="5a99b-139">String</span></span>     |<span data-ttu-id="5a99b-p106">要匹配的扩展属性的值。**HTTP 请求**部分中列出的必需的参数。</span><span class="sxs-lookup"><span data-stu-id="5a99b-p106">The value of the extended property to match. Required where listed in the HTTP request section above.</span></span>|
|<span data-ttu-id="5a99b-142">person_property</span><span class="sxs-lookup"><span data-stu-id="5a99b-142">person_property</span></span>|<span data-ttu-id="5a99b-143">String</span><span class="sxs-lookup"><span data-stu-id="5a99b-143">String</span></span>    |<span data-ttu-id="5a99b-p107">要匹配的人员属性。**HTTP 请求**部分中列出的必需的参数。</span><span class="sxs-lookup"><span data-stu-id="5a99b-p107">The value of the extended property to match. Required where listed in the HTTP request section above.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="5a99b-146">请求标头</span><span class="sxs-lookup"><span data-stu-id="5a99b-146">Request headers</span></span>
| <span data-ttu-id="5a99b-147">名称</span><span class="sxs-lookup"><span data-stu-id="5a99b-147">Name</span></span>      |<span data-ttu-id="5a99b-148">说明</span><span class="sxs-lookup"><span data-stu-id="5a99b-148">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5a99b-149">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a99b-149">Authorization</span></span>  | <span data-ttu-id="5a99b-p108">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5a99b-p108">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5a99b-152">请求正文</span><span class="sxs-lookup"><span data-stu-id="5a99b-152">Request body</span></span>
<span data-ttu-id="5a99b-153">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5a99b-153">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="5a99b-154">响应</span><span class="sxs-lookup"><span data-stu-id="5a99b-154">Response</span></span>
<span data-ttu-id="5a99b-p109">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [person](../resources/person.md) 对象。响应可以包含一个人员实例或一个人员实例集合。</span><span class="sxs-lookup"><span data-stu-id="5a99b-p109">If successful, this method returns a `200 OK` response code and a [person](../resources/person.md) object in the response body. The response can contain one person instance or a collection of person instances.</span></span> 
## <a name="examples"></a><span data-ttu-id="5a99b-157">示例</span><span class="sxs-lookup"><span data-stu-id="5a99b-157">Examples</span></span>
### <a name="perform-a-search"></a><span data-ttu-id="5a99b-158">执行搜索</span><span class="sxs-lookup"><span data-stu-id="5a99b-158">Perform a search for Reseller entity instances.</span></span> 
<span data-ttu-id="5a99b-159">以下请求搜索名为“Irene McGowan”的人员。</span><span class="sxs-lookup"><span data-stu-id="5a99b-159">The following request does a search for a person named Irene McGowan.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_person"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="Irene McGowan"
```

<span data-ttu-id="5a99b-160">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="5a99b-160">The following example shows the response.</span></span> 

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
### <a name="select-the-fields-to-return-in-a-filtered-response"></a><span data-ttu-id="5a99b-161">选择要在经过筛选的响应中返回的字段</span><span class="sxs-lookup"><span data-stu-id="5a99b-161">Select the fields to return in a filtered response</span></span> 
<span data-ttu-id="5a99b-162">可以结合 *$select* 和 *$filter* 参数创建自定义用户相关人员列表，并且只获取应用程序需要的字段。</span><span class="sxs-lookup"><span data-stu-id="5a99b-162">You can combine the *$select* and *$filter* parameters to create a custom list of people relevant to the user and get only the fields that your application needs.</span></span> 

<span data-ttu-id="5a99b-p110">以下示例获取显示名称等于指定名称的人员的 **displayName** 和 **scoredEmailAddresses**。在本示例中，只返回显示名称等于“Lorrie Frye”的人员。</span><span class="sxs-lookup"><span data-stu-id="5a99b-p110">The following example gets the **displayName** and **scoredEmailAddresses** of people whose display name equals the specified name. In this example, only people whose display name equals "Lorrie Frye" are returned.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_person"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/people/?$select=displayName,scoredEmailAddresses&$filter=displayName eq 'Lorrie Frye'
```

<span data-ttu-id="5a99b-165">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="5a99b-165">The following example shows the response.</span></span> 

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
            "scoredEmailAddresses": [
                {
                    "address": "Lorrief@contoso.onmicrosoft.com",
                    "relevanceScore": 8
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
