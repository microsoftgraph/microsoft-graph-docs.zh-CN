# <a name="get-person"></a><span data-ttu-id="b79ce-101">Get person</span><span class="sxs-lookup"><span data-stu-id="b79ce-101">Get person</span></span>

<span data-ttu-id="b79ce-102">检索 [person](../resources/person.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b79ce-102">Retrieve the properties and relationships of a [person](../resources/person.md) object.</span></span>

<span data-ttu-id="b79ce-p101">可以通过 People API 获取此信息。有关示例，请参阅[示例](#examples)部分和[获取人员的相关信息](../../../concepts/people_example.md)一文。</span><span class="sxs-lookup"><span data-stu-id="b79ce-p101">You can get this information via the People API. For examples, see the [Examples](#examples) section and the article [Get relevant information about people](../../../concepts/people_example.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b79ce-105">权限</span><span class="sxs-lookup"><span data-stu-id="b79ce-105">Permissions</span></span>
<span data-ttu-id="b79ce-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="b79ce-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>
 

|<span data-ttu-id="b79ce-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b79ce-108">Permission type</span></span>      | <span data-ttu-id="b79ce-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b79ce-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b79ce-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b79ce-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b79ce-111">People.Read、People.Read.All</span><span class="sxs-lookup"><span data-stu-id="b79ce-111">People.Read, People.Read.All</span></span>    |
|<span data-ttu-id="b79ce-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b79ce-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b79ce-113">People.Read</span><span class="sxs-lookup"><span data-stu-id="b79ce-113">People.Read</span></span>    |
|<span data-ttu-id="b79ce-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="b79ce-114">Application</span></span> | <span data-ttu-id="b79ce-115">People.Read.All</span><span class="sxs-lookup"><span data-stu-id="b79ce-115">People.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b79ce-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b79ce-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/people/{id}
GET /users/{id | userPrincipalName}/people/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b79ce-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b79ce-117">Optional query parameters</span></span>
<span data-ttu-id="b79ce-118">此方法支持以下 [OData 查询参数](../../../concepts/people_example.md)，有助于自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b79ce-118">This method supports the [OData Query Parameters](../../../concepts/people_example.md) to help customize the response.</span></span>

|<span data-ttu-id="b79ce-119">名称</span><span class="sxs-lookup"><span data-stu-id="b79ce-119">Name</span></span>|<span data-ttu-id="b79ce-120">值</span><span class="sxs-lookup"><span data-stu-id="b79ce-120">Value</span></span>|<span data-ttu-id="b79ce-121">说明</span><span class="sxs-lookup"><span data-stu-id="b79ce-121">Description</span></span>| 
|:---------------|:--------|:-------| 
|<span data-ttu-id="b79ce-122">$filter</span><span class="sxs-lookup"><span data-stu-id="b79ce-122">$filter</span></span>|<span data-ttu-id="b79ce-123">string</span><span class="sxs-lookup"><span data-stu-id="b79ce-123">string</span></span>|<span data-ttu-id="b79ce-124">将响应限制为仅记录中包含指定条件的那些人员。</span><span class="sxs-lookup"><span data-stu-id="b79ce-124">Limits the response to only those people whose record contains the specified criteria.</span></span>| 
|<span data-ttu-id="b79ce-125">$orderby</span><span class="sxs-lookup"><span data-stu-id="b79ce-125">$orderby</span></span>|<span data-ttu-id="b79ce-126">string</span><span class="sxs-lookup"><span data-stu-id="b79ce-126">string</span></span>|<span data-ttu-id="b79ce-127">默认情况下，按与查询的相关程度对响应中的人员进行排序。</span><span class="sxs-lookup"><span data-stu-id="b79ce-127">By default, the people in the response are sorted by their relevance to your query. You can change the order of the people in the response using the $orderby parameter.</span></span> <span data-ttu-id="b79ce-128">可以使用 *$orderby* 参数更改响应中的人员排序。</span><span class="sxs-lookup"><span data-stu-id="b79ce-128">By default, the people in the response are sorted by their relevance to your query. You can change the order of the people in the response using the *$orderby* parameter.</span></span>| 
|<span data-ttu-id="b79ce-129">$search</span><span class="sxs-lookup"><span data-stu-id="b79ce-129">$search</span></span>|<span data-ttu-id="b79ce-130">string</span><span class="sxs-lookup"><span data-stu-id="b79ce-130">string</span></span>|<span data-ttu-id="b79ce-131">按姓名或别名搜索人员。</span><span class="sxs-lookup"><span data-stu-id="b79ce-131">Search for people by name or alias. Supports fuzzy matching.</span></span> <span data-ttu-id="b79ce-132">支持模糊匹配</span><span class="sxs-lookup"><span data-stu-id="b79ce-132">Supports Fuzzy matching</span></span>| 
|<span data-ttu-id="b79ce-133">$select</span><span class="sxs-lookup"><span data-stu-id="b79ce-133">$select</span></span>|<span data-ttu-id="b79ce-134">string</span><span class="sxs-lookup"><span data-stu-id="b79ce-134">string</span></span>|<span data-ttu-id="b79ce-p105">要在响应中添加的属性列表（以逗号分隔）。为获得最佳结果，请仅选择所需属性的子集。</span><span class="sxs-lookup"><span data-stu-id="b79ce-p105">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>| 
|<span data-ttu-id="b79ce-137">$skip</span><span class="sxs-lookup"><span data-stu-id="b79ce-137">$skip</span></span>|<span data-ttu-id="b79ce-138">int</span><span class="sxs-lookup"><span data-stu-id="b79ce-138">int</span></span>|<span data-ttu-id="b79ce-p106">跳过前 n 个结果，可用于分页。使用 *$search* 时不支持此参数。</span><span class="sxs-lookup"><span data-stu-id="b79ce-p106">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>| 
|<span data-ttu-id="b79ce-141">$top</span><span class="sxs-lookup"><span data-stu-id="b79ce-141">$top</span></span>|<span data-ttu-id="b79ce-142">int</span><span class="sxs-lookup"><span data-stu-id="b79ce-142">int</span></span>|<span data-ttu-id="b79ce-143">要返回的结果数。</span><span class="sxs-lookup"><span data-stu-id="b79ce-143">Number of results to be returned.</span></span>| 

## <a name="request-headers"></a><span data-ttu-id="b79ce-144">请求标头</span><span class="sxs-lookup"><span data-stu-id="b79ce-144">Request headers</span></span>
| <span data-ttu-id="b79ce-145">名称</span><span class="sxs-lookup"><span data-stu-id="b79ce-145">Name</span></span>      |<span data-ttu-id="b79ce-146">说明</span><span class="sxs-lookup"><span data-stu-id="b79ce-146">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b79ce-147">Authorization</span><span class="sxs-lookup"><span data-stu-id="b79ce-147">Authorization</span></span>  | <span data-ttu-id="b79ce-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b79ce-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b79ce-150">请求正文</span><span class="sxs-lookup"><span data-stu-id="b79ce-150">Request body</span></span>
<span data-ttu-id="b79ce-151">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b79ce-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b79ce-152">响应</span><span class="sxs-lookup"><span data-stu-id="b79ce-152">Response</span></span>
<span data-ttu-id="b79ce-153">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [person](../resources/person.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b79ce-153">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/person.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b79ce-154">示例</span><span class="sxs-lookup"><span data-stu-id="b79ce-154">Examples</span></span>
#### <a name="request-1"></a><span data-ttu-id="b79ce-155">请求 1</span><span class="sxs-lookup"><span data-stu-id="b79ce-155">Request 1</span></span>
<span data-ttu-id="b79ce-156">下面展示了示例请求，以从用户组织中获取拥有此 ID 的用户。</span><span class="sxs-lookup"><span data-stu-id="b79ce-156">The following is an example of the request that gets the person who has this ID in the user's organization.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_person_by_id"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/people/e3d0513b-449e-4198-ba6f-bd97ae7cae85
```

#### <a name="response-1"></a><span data-ttu-id="b79ce-157">响应 1</span><span class="sxs-lookup"><span data-stu-id="b79ce-157">Response 1</span></span>
<span data-ttu-id="b79ce-158">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b79ce-158">Here is an example of the response.</span></span>

><span data-ttu-id="b79ce-159">**注意：**为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b79ce-159">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b79ce-160">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b79ce-160">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_person_by_id",
  "truncated": true,
  "@odata.type": "microsoft.graph.person"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 629

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
```

#### <a name="request-2"></a><span data-ttu-id="b79ce-161">请求 2</span><span class="sxs-lookup"><span data-stu-id="b79ce-161">Request 2</span></span>
<span data-ttu-id="b79ce-162">下面展示了示例请求，以从用户组织中获取拥有此 ID 的用户，并限制在响应中返回选定属性。</span><span class="sxs-lookup"><span data-stu-id="b79ce-162">The following is an example of the request that gets the person who has this ID in the user's organization and restricts the response to the selected properties.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_person_by_id_with_select"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/people/e3d0513b-449e-4198-ba6f-bd97ae7cae85?$select=displayName
```
#### <a name="response-2"></a><span data-ttu-id="b79ce-163">响应 2</span><span class="sxs-lookup"><span data-stu-id="b79ce-163">Response 2</span></span>
<span data-ttu-id="b79ce-164">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b79ce-164">Here is an example of the response.</span></span>

><span data-ttu-id="b79ce-165">**注意：**为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b79ce-165">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b79ce-166">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b79ce-166">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_person_by_id_with_select",
  "truncated": true,
  "@odata.type": "microsoft.graph.person"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 305

{
  "id": "e3d0513b-449e-4198-ba6f-bd97ae7cae85",
  "displayName": "Isaiah Langer"
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
