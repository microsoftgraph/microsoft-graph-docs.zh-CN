# <a name="get-person"></a><span data-ttu-id="db213-101">Get person</span><span class="sxs-lookup"><span data-stu-id="db213-101">Get person</span></span>

<span data-ttu-id="db213-102">检索 [person](../resources/person.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="db213-102">Retrieve the properties and relationships of a [person](../resources/person.md) object.</span></span>

<span data-ttu-id="db213-p101">可以通过 People API 获取此信息。有关示例，请参阅[示例](#examples)部分和[获取人员的相关信息](../../../concepts/people_example.md)一文。</span><span class="sxs-lookup"><span data-stu-id="db213-p101">You can get this information via the People API. For examples, see the [Examples](#examples) section and the article [Get relevant information about people](../../../concepts/people_example.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="db213-105">权限</span><span class="sxs-lookup"><span data-stu-id="db213-105">Permissions</span></span>
<span data-ttu-id="db213-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="db213-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>
 

|<span data-ttu-id="db213-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="db213-108">Permission type</span></span>      | <span data-ttu-id="db213-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="db213-109">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="db213-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="db213-110">Delegated (work or school account)</span></span> | <span data-ttu-id="db213-111">People.Read、People.Read.All</span><span class="sxs-lookup"><span data-stu-id="db213-111">People.Read, People.Read.All</span></span>    | 
|<span data-ttu-id="db213-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="db213-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db213-113">People.Read</span><span class="sxs-lookup"><span data-stu-id="db213-113">People.Read</span></span>    | 
|<span data-ttu-id="db213-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="db213-114">Application</span></span> | <span data-ttu-id="db213-115">People.Read.All</span><span class="sxs-lookup"><span data-stu-id="db213-115">People.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="db213-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="db213-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/people/?$search='{property_value}'
GET /me/people/?$filter={person_property} eq '{property_value}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="db213-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="db213-117">Optional query parameters</span></span>
|<span data-ttu-id="db213-118">Name</span><span class="sxs-lookup"><span data-stu-id="db213-118">Name</span></span>|<span data-ttu-id="db213-119">值</span><span class="sxs-lookup"><span data-stu-id="db213-119">Value</span></span>|<span data-ttu-id="db213-120">说明</span><span class="sxs-lookup"><span data-stu-id="db213-120">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="db213-121">$filter</span><span class="sxs-lookup"><span data-stu-id="db213-121">$filter</span></span>|<span data-ttu-id="db213-122">string</span><span class="sxs-lookup"><span data-stu-id="db213-122">string</span></span>|<span data-ttu-id="db213-123">将响应限制为仅记录中包含指定条件的那些人员。</span><span class="sxs-lookup"><span data-stu-id="db213-123">Limits the response to only those people whose record contains the specified criteria.</span></span>|
|<span data-ttu-id="db213-124">$orderby</span><span class="sxs-lookup"><span data-stu-id="db213-124">$orderby</span></span>|<span data-ttu-id="db213-125">string</span><span class="sxs-lookup"><span data-stu-id="db213-125">string</span></span>|<span data-ttu-id="db213-p103">默认情况下，按与查询的相关性对响应中的人员进行排序。可以使用 *$orderby* 参数更改响应中的人员的顺序。</span><span class="sxs-lookup"><span data-stu-id="db213-p103">By default, the people in the response are sorted by their relevance to your query. You can change the order of the people in the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="db213-128">$search</span><span class="sxs-lookup"><span data-stu-id="db213-128">$search</span></span>|<span data-ttu-id="db213-129">string</span><span class="sxs-lookup"><span data-stu-id="db213-129">string</span></span>|<span data-ttu-id="db213-p104">按名字或别名搜索人员。支持模糊匹配。</span><span class="sxs-lookup"><span data-stu-id="db213-p104">Search for people by name or alias. Supports fuzzy matching.</span></span>|
|<span data-ttu-id="db213-132">$select</span><span class="sxs-lookup"><span data-stu-id="db213-132">$select</span></span>|<span data-ttu-id="db213-133">string</span><span class="sxs-lookup"><span data-stu-id="db213-133">string</span></span>|<span data-ttu-id="db213-p105">要在响应中添加的属性列表（以逗号分隔）。为获得最佳结果，请仅选择所需属性的子集。</span><span class="sxs-lookup"><span data-stu-id="db213-p105">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>|
|<span data-ttu-id="db213-136">$skip</span><span class="sxs-lookup"><span data-stu-id="db213-136">$skip</span></span>|<span data-ttu-id="db213-137">int</span><span class="sxs-lookup"><span data-stu-id="db213-137">int</span></span>|<span data-ttu-id="db213-p106">跳过前 n 个结果，可用于分页。使用 *$search* 时不支持此参数。</span><span class="sxs-lookup"><span data-stu-id="db213-p106">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>|
|<span data-ttu-id="db213-140">$top</span><span class="sxs-lookup"><span data-stu-id="db213-140">$top</span></span>|<span data-ttu-id="db213-141">int</span><span class="sxs-lookup"><span data-stu-id="db213-141">int</span></span>|<span data-ttu-id="db213-142">要返回的结果数。</span><span class="sxs-lookup"><span data-stu-id="db213-142">Number of results to be returned.</span></span>|

## <a name="parameters"></a><span data-ttu-id="db213-143">参数</span><span class="sxs-lookup"><span data-stu-id="db213-143">Parameters</span></span>
| <span data-ttu-id="db213-144">参数</span><span class="sxs-lookup"><span data-stu-id="db213-144">Parameter</span></span> |<span data-ttu-id="db213-145">类型</span><span class="sxs-lookup"><span data-stu-id="db213-145">Type</span></span>       |<span data-ttu-id="db213-146">说明</span><span class="sxs-lookup"><span data-stu-id="db213-146">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="db213-147">property_value</span><span class="sxs-lookup"><span data-stu-id="db213-147">property_value</span></span>|<span data-ttu-id="db213-148">字符串</span><span class="sxs-lookup"><span data-stu-id="db213-148">String</span></span>     |<span data-ttu-id="db213-p107">要匹配的扩展属性的值。**HTTP 请求**部分中列出的必需的参数。</span><span class="sxs-lookup"><span data-stu-id="db213-p107">The value of the extended property to match. Required where listed in the **HTTP request** section.</span></span>|
|<span data-ttu-id="db213-151">person_property</span><span class="sxs-lookup"><span data-stu-id="db213-151">person_property</span></span>|<span data-ttu-id="db213-152">字符串</span><span class="sxs-lookup"><span data-stu-id="db213-152">String</span></span>    |<span data-ttu-id="db213-p108">要匹配的人员属性。**HTTP 请求**部分中列出的必需的参数。</span><span class="sxs-lookup"><span data-stu-id="db213-p108">The person property to match. Required where listed in the **HTTP request** section.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="db213-155">请求标头</span><span class="sxs-lookup"><span data-stu-id="db213-155">Request headers</span></span>
| <span data-ttu-id="db213-156">名称</span><span class="sxs-lookup"><span data-stu-id="db213-156">Name</span></span>      |<span data-ttu-id="db213-157">说明</span><span class="sxs-lookup"><span data-stu-id="db213-157">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="db213-158">Authorization</span><span class="sxs-lookup"><span data-stu-id="db213-158">Authorization</span></span>  | <span data-ttu-id="db213-p109">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="db213-p109">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="db213-161">请求正文</span><span class="sxs-lookup"><span data-stu-id="db213-161">Request body</span></span>
<span data-ttu-id="db213-162">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="db213-162">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="db213-163">响应</span><span class="sxs-lookup"><span data-stu-id="db213-163">Response</span></span>
<span data-ttu-id="db213-p110">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [person](../resources/person.md) 对象。响应可以包含一个人员实例或一个人员实例集合。</span><span class="sxs-lookup"><span data-stu-id="db213-p110">If successful, this method returns a `200 OK` response code and a [person](../resources/person.md) object in the response body. The response can contain one person instance or a collection of person instances.</span></span> 
## <a name="examples"></a><span data-ttu-id="db213-166">示例</span><span class="sxs-lookup"><span data-stu-id="db213-166">Examples</span></span>
### <a name="perform-a-search"></a><span data-ttu-id="db213-167">执行搜索</span><span class="sxs-lookup"><span data-stu-id="db213-167">Perform a search</span></span> 
<span data-ttu-id="db213-168">以下请求搜索名为“Irene McGowan”的人员。</span><span class="sxs-lookup"><span data-stu-id="db213-168">The following request does a search for a person named Irene McGowan.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_person"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="Irene McGowan"
```

<span data-ttu-id="db213-169">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="db213-169">The following example shows the response.</span></span> 

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
### <a name="select-the-fields-to-return-in-a-filtered-response"></a><span data-ttu-id="db213-170">选择要在经过筛选的响应中返回的字段</span><span class="sxs-lookup"><span data-stu-id="db213-170">Select the fields to return in a filtered response</span></span> 
<span data-ttu-id="db213-171">可以结合 *$select* 和 *$filter* 参数创建自定义用户相关人员列表，并且只获取应用程序需要的字段。</span><span class="sxs-lookup"><span data-stu-id="db213-171">You can combine the *$select* and *$filter* parameters to create a custom list of people relevant to the user and get only the fields that your application needs.</span></span> 

<span data-ttu-id="db213-p111">以下示例获取显示名称等于指定名称的人员的 **displayName** 和 **scoredEmailAddresses**。在本示例中，只返回显示名称等于“Lorrie Frye”的人员。</span><span class="sxs-lookup"><span data-stu-id="db213-p111">The following example gets the **displayName** and **scoredEmailAddresses** of people whose display name equals the specified name. In this example, only people whose display name equals "Lorrie Frye" are returned.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_person"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/people/?$select=displayName,scoredEmailAddresses&$filter=displayName eq 'Lorrie Frye'
```

<span data-ttu-id="db213-174">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="db213-174">The following example shows the response.</span></span> 

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
