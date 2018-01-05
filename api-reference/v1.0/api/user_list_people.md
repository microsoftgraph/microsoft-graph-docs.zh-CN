# <a name="list-people"></a><span data-ttu-id="952fc-101">列出人员</span><span class="sxs-lookup"><span data-stu-id="952fc-101">List people</span></span>

<span data-ttu-id="952fc-102">检索一组 [person](../resources/person.md) 对象，这些对象按与 [user](../resources/user.md) 的相关程度进行排序，相关程度由用户的通信和协作模式以及业务关系决定。</span><span class="sxs-lookup"><span data-stu-id="952fc-102">Retrieve a collection of [person](../resources/person.md) objects ordered by their relevance to the [user](../resources/user.md), which is determined by the user's communication and collaboration patterns and business relationships.</span></span>

<span data-ttu-id="952fc-p101">可以通过 People API 获取此信息。有关示例，请参阅[示例](#examples)部分和[获取人员的相关信息](../../../concepts/people_example.md)一文。</span><span class="sxs-lookup"><span data-stu-id="952fc-p101">You can get this information via the People API. For examples, see the [Examples](#examples) section and the article [Get relevant information about people](../../../concepts/people_example.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="952fc-105">权限</span><span class="sxs-lookup"><span data-stu-id="952fc-105">Permissions</span></span>
<span data-ttu-id="952fc-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="952fc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="952fc-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="952fc-108">Permission type</span></span>      | <span data-ttu-id="952fc-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="952fc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="952fc-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="952fc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="952fc-111">People.Read、People.Read.All</span><span class="sxs-lookup"><span data-stu-id="952fc-111">People.Read, People.Read.All</span></span>    |
|<span data-ttu-id="952fc-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="952fc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="952fc-113">People.Read</span><span class="sxs-lookup"><span data-stu-id="952fc-113">People.Read</span></span>    |
|<span data-ttu-id="952fc-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="952fc-114">Application</span></span> | <span data-ttu-id="952fc-115">People.Read.All</span><span class="sxs-lookup"><span data-stu-id="952fc-115">People.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="952fc-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="952fc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/people
GET /users/{id | userPrincipalName}/people
```

## <a name="optional-query-parameters"></a><span data-ttu-id="952fc-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="952fc-117">Optional query parameters</span></span>
<span data-ttu-id="952fc-118">此方法支持使用 [OData 查询参数](../../../concepts/query_parameters.md)自定义响应，如[获取人员的相关信息](../../../concepts/people_example.md)一文中的示例所示。</span><span class="sxs-lookup"><span data-stu-id="952fc-118">This method supports the [OData query parameters](../../../concepts/query_parameters.md) to help customize the response, as shown in the examples in the article [Get relevant information about people](../../../concepts/people_example.md).</span></span>

|<span data-ttu-id="952fc-119">名称</span><span class="sxs-lookup"><span data-stu-id="952fc-119">Name</span></span>|<span data-ttu-id="952fc-120">值</span><span class="sxs-lookup"><span data-stu-id="952fc-120">Value</span></span>|<span data-ttu-id="952fc-121">说明</span><span class="sxs-lookup"><span data-stu-id="952fc-121">Description</span></span>| 
|:---------------|:--------|:-------| 
|<span data-ttu-id="952fc-122">$filter</span><span class="sxs-lookup"><span data-stu-id="952fc-122">$filter</span></span>|<span data-ttu-id="952fc-123">string</span><span class="sxs-lookup"><span data-stu-id="952fc-123">string</span></span>|<span data-ttu-id="952fc-124">将响应限制为仅记录中包含指定条件的那些人员。</span><span class="sxs-lookup"><span data-stu-id="952fc-124">Limits the response to only those people whose record contains the specified criteria.</span></span>| 
|<span data-ttu-id="952fc-125">$orderby</span><span class="sxs-lookup"><span data-stu-id="952fc-125">$orderby</span></span>|<span data-ttu-id="952fc-126">string</span><span class="sxs-lookup"><span data-stu-id="952fc-126">string</span></span>|<span data-ttu-id="952fc-127">默认情况下，按与查询的相关程度对响应中的人员进行排序。</span><span class="sxs-lookup"><span data-stu-id="952fc-127">By default, the people in the response are sorted by their relevance to your query. You can change the order of the people in the response using the $orderby parameter.</span></span> <span data-ttu-id="952fc-128">可以使用 *$orderby* 参数更改响应中的人员排序。</span><span class="sxs-lookup"><span data-stu-id="952fc-128">By default, the people in the response are sorted by their relevance to your query. You can change the order of the people in the response using the *$orderby* parameter.</span></span>| 
|<span data-ttu-id="952fc-129">$search</span><span class="sxs-lookup"><span data-stu-id="952fc-129">$search</span></span>|<span data-ttu-id="952fc-130">string</span><span class="sxs-lookup"><span data-stu-id="952fc-130">string</span></span>|<span data-ttu-id="952fc-131">按姓名或别名搜索人员。</span><span class="sxs-lookup"><span data-stu-id="952fc-131">Search for people by name or alias. Supports fuzzy matching.</span></span> <span data-ttu-id="952fc-132">支持模糊匹配。</span><span class="sxs-lookup"><span data-stu-id="952fc-132">Supports Fuzzy matching.</span></span>| 
|<span data-ttu-id="952fc-133">$select</span><span class="sxs-lookup"><span data-stu-id="952fc-133">$select</span></span>|<span data-ttu-id="952fc-134">string</span><span class="sxs-lookup"><span data-stu-id="952fc-134">string</span></span>|<span data-ttu-id="952fc-p105">要在响应中添加的属性列表（以逗号分隔）。为获得最佳结果，请仅选择所需属性的子集。</span><span class="sxs-lookup"><span data-stu-id="952fc-p105">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>| 
|<span data-ttu-id="952fc-137">$skip</span><span class="sxs-lookup"><span data-stu-id="952fc-137">$skip</span></span>|<span data-ttu-id="952fc-138">int</span><span class="sxs-lookup"><span data-stu-id="952fc-138">int</span></span>|<span data-ttu-id="952fc-p106">跳过前 n 个结果，可用于分页。使用 *$search* 时不支持此参数。</span><span class="sxs-lookup"><span data-stu-id="952fc-p106">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>| 
|<span data-ttu-id="952fc-141">$top</span><span class="sxs-lookup"><span data-stu-id="952fc-141">$top</span></span>|<span data-ttu-id="952fc-142">int</span><span class="sxs-lookup"><span data-stu-id="952fc-142">int</span></span>|<span data-ttu-id="952fc-143">要返回的结果数。</span><span class="sxs-lookup"><span data-stu-id="952fc-143">Number of results to be returned.</span></span>| 

## <a name="request-headers"></a><span data-ttu-id="952fc-144">请求标头</span><span class="sxs-lookup"><span data-stu-id="952fc-144">Request headers</span></span>
| <span data-ttu-id="952fc-145">名称</span><span class="sxs-lookup"><span data-stu-id="952fc-145">Name</span></span>      |<span data-ttu-id="952fc-146">说明</span><span class="sxs-lookup"><span data-stu-id="952fc-146">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="952fc-147">Authorization</span><span class="sxs-lookup"><span data-stu-id="952fc-147">Authorization</span></span>  | <span data-ttu-id="952fc-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="952fc-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="952fc-150">接受</span><span class="sxs-lookup"><span data-stu-id="952fc-150">Accept</span></span> | <span data-ttu-id="952fc-151">application/json</span><span class="sxs-lookup"><span data-stu-id="952fc-151">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="952fc-152">请求正文</span><span class="sxs-lookup"><span data-stu-id="952fc-152">Request body</span></span>
<span data-ttu-id="952fc-153">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="952fc-153">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="952fc-154">响应</span><span class="sxs-lookup"><span data-stu-id="952fc-154">Response</span></span>
<span data-ttu-id="952fc-p108">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [person](../resources/person.md) 对象集合。响应可以包含一个人员对象或一个人员对象集合。</span><span class="sxs-lookup"><span data-stu-id="952fc-p108">If successful, this method returns a `200 OK` response code and a collection of [person](../resources/person.md) objects in the response body. The response can contain one person object or a collection of person objects.</span></span>

## <a name="examples"></a><span data-ttu-id="952fc-157">示例</span><span class="sxs-lookup"><span data-stu-id="952fc-157">Examples</span></span>
#### <a name="request"></a><span data-ttu-id="952fc-158">请求</span><span class="sxs-lookup"><span data-stu-id="952fc-158">Request</span></span>
<span data-ttu-id="952fc-159">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="952fc-159">The following is an example of the request body.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_person_collection"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/people
```

#### <a name="response"></a><span data-ttu-id="952fc-160">响应</span><span class="sxs-lookup"><span data-stu-id="952fc-160">Response</span></span>
<span data-ttu-id="952fc-161">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="952fc-161">Here is an example of the response.</span></span>

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
Content-length: 1370

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

<span data-ttu-id="952fc-162">有关更多示例，请参阅[获取人员的相关信息](../../../concepts/people_example.md)一文。</span><span class="sxs-lookup"><span data-stu-id="952fc-162">For more examples, see the article [Get relevant information about people](../../../concepts/people_example.md).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List people",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
