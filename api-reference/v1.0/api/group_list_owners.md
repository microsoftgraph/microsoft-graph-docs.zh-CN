# <a name="list-owners"></a><span data-ttu-id="78756-101">列出所有者</span><span class="sxs-lookup"><span data-stu-id="78756-101">List owners</span></span>
<span data-ttu-id="78756-p101">检索组的所有者列表。所有者是一组具有 group 对象修改权限的非管理员用户。</span><span class="sxs-lookup"><span data-stu-id="78756-p101">Retrieve a list of the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="78756-104">权限</span><span class="sxs-lookup"><span data-stu-id="78756-104">Permissions</span></span>
<span data-ttu-id="78756-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="78756-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="78756-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="78756-107">Permission type</span></span>      | <span data-ttu-id="78756-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="78756-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="78756-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="78756-109">Delegated (work or school account)</span></span> | <span data-ttu-id="78756-110">Group.Read.All 和 User.ReadBasic.All、Group.Read.All 和 User.Read.All、Group.Read.All 和 User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78756-110">Group.Read.All and User.ReadBasic.All, Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All</span></span>   |
|<span data-ttu-id="78756-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="78756-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78756-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="78756-112">Not supported.</span></span>    |
|<span data-ttu-id="78756-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="78756-113">Application</span></span> | <span data-ttu-id="78756-114">Group.Read.All 和 User.Read.All、Group.Read.All 和User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78756-114">Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="78756-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="78756-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/owners
```

## <a name="optional-query-parameters"></a><span data-ttu-id="78756-116">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="78756-116">Optional query parameters</span></span>
<span data-ttu-id="78756-117">此方法支持 [OData 查询参数](../../../concepts/query_parameters.md) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="78756-117">This method supports the [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="78756-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="78756-118">Request headers</span></span>
| <span data-ttu-id="78756-119">名称</span><span class="sxs-lookup"><span data-stu-id="78756-119">Name</span></span>       | <span data-ttu-id="78756-120">类型</span><span class="sxs-lookup"><span data-stu-id="78756-120">Type</span></span> | <span data-ttu-id="78756-121">说明</span><span class="sxs-lookup"><span data-stu-id="78756-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="78756-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="78756-122">Authorization</span></span>  | <span data-ttu-id="78756-123">string</span><span class="sxs-lookup"><span data-stu-id="78756-123">string</span></span>  | <span data-ttu-id="78756-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="78756-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="78756-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="78756-126">Request body</span></span>
<span data-ttu-id="78756-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="78756-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="78756-128">响应</span><span class="sxs-lookup"><span data-stu-id="78756-128">Response</span></span>
<span data-ttu-id="78756-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/user.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="78756-129">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78756-130">示例</span><span class="sxs-lookup"><span data-stu-id="78756-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="78756-131">请求</span><span class="sxs-lookup"><span data-stu-id="78756-131">Request</span></span>
<span data-ttu-id="78756-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="78756-132">The following is an example of the request body.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/owners
```

#### <a name="response"></a><span data-ttu-id="78756-133">响应</span><span class="sxs-lookup"><span data-stu-id="78756-133">Response</span></span>
<span data-ttu-id="78756-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="78756-134">Here is an example of the response.</span></span>
><span data-ttu-id="78756-135">**注意：**为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="78756-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="78756-136">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="78756-136">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.user"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
