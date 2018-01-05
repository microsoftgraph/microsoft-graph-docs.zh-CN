# <a name="list-photos"></a><span data-ttu-id="ac1fb-101">List photos</span><span class="sxs-lookup"><span data-stu-id="ac1fb-101">List photos</span></span>
<span data-ttu-id="ac1fb-102">检索 [profilePhoto](../resources/profilephoto.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="ac1fb-102">Retrieve a list of [profilePhoto](../resources/profilephoto.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="ac1fb-103">权限</span><span class="sxs-lookup"><span data-stu-id="ac1fb-103">Permissions</span></span>
<span data-ttu-id="ac1fb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="ac1fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ac1fb-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="ac1fb-106">Permission type</span></span>      | <span data-ttu-id="ac1fb-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ac1fb-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ac1fb-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ac1fb-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ac1fb-109">Group.ReadBasic.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac1fb-109">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span> |
|<span data-ttu-id="ac1fb-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ac1fb-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac1fb-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="ac1fb-111">Not supported.</span></span>    |
|<span data-ttu-id="ac1fb-112">应用</span><span class="sxs-lookup"><span data-stu-id="ac1fb-112">Application</span></span> | <span data-ttu-id="ac1fb-113">Group.ReadBasic.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac1fb-113">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ac1fb-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ac1fb-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/photos
GET /users/{id | userPrincipalName}/joinedGroups/{id}/photos
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ac1fb-115">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ac1fb-115">Optional query parameters</span></span>
<span data-ttu-id="ac1fb-116">此方法支持 [OData 查询参数](../../../concepts/query_parameters.md) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ac1fb-116">This method supports the [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ac1fb-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="ac1fb-117">Request headers</span></span>
| <span data-ttu-id="ac1fb-118">名称</span><span class="sxs-lookup"><span data-stu-id="ac1fb-118">Name</span></span>       | <span data-ttu-id="ac1fb-119">类型</span><span class="sxs-lookup"><span data-stu-id="ac1fb-119">Type</span></span> | <span data-ttu-id="ac1fb-120">说明</span><span class="sxs-lookup"><span data-stu-id="ac1fb-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ac1fb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac1fb-121">Authorization</span></span>  | <span data-ttu-id="ac1fb-122">string</span><span class="sxs-lookup"><span data-stu-id="ac1fb-122">string</span></span>  | <span data-ttu-id="ac1fb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ac1fb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ac1fb-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="ac1fb-125">Request body</span></span>
<span data-ttu-id="ac1fb-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ac1fb-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ac1fb-127">响应</span><span class="sxs-lookup"><span data-stu-id="ac1fb-127">Response</span></span>
<span data-ttu-id="ac1fb-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [profilePhoto](../resources/profilephoto.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ac1fb-128">If successful, this method returns a `200 OK` response code and collection of [profilePhoto](../resources/profilephoto.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac1fb-129">示例</span><span class="sxs-lookup"><span data-stu-id="ac1fb-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="ac1fb-130">请求</span><span class="sxs-lookup"><span data-stu-id="ac1fb-130">Request</span></span>
<span data-ttu-id="ac1fb-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ac1fb-131">The following is an example of the request body.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photos"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/photos
```

#### <a name="response"></a><span data-ttu-id="ac1fb-132">响应</span><span class="sxs-lookup"><span data-stu-id="ac1fb-132">Response</span></span>
<span data-ttu-id="ac1fb-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ac1fb-133">Here is an example of the response.</span></span>
><span data-ttu-id="ac1fb-134">**注意：**为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ac1fb-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ac1fb-135">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ac1fb-135">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profilePhoto",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 94

{
  "value": [
    {
      "height": 99,
      "width": 99,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List photos",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
