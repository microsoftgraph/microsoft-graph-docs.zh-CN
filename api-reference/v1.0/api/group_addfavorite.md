# <a name="group-addfavorite"></a><span data-ttu-id="51dac-101">group: addFavorite</span><span class="sxs-lookup"><span data-stu-id="51dac-101">group: addFavorite</span></span>
<span data-ttu-id="51dac-p101">将组添加到当前用户的收藏夹组列表中。仅支持 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="51dac-p101">Add the group to the list of the current user's favorite groups. Supported for only Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="51dac-104">权限</span><span class="sxs-lookup"><span data-stu-id="51dac-104">Permissions</span></span>
<span data-ttu-id="51dac-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="51dac-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="51dac-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="51dac-107">Permission type</span></span>      | <span data-ttu-id="51dac-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="51dac-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="51dac-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="51dac-109">Delegated (work or school account)</span></span> | <span data-ttu-id="51dac-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51dac-110">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="51dac-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="51dac-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51dac-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="51dac-112">Not supported.</span></span>    |
|<span data-ttu-id="51dac-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="51dac-113">Application</span></span> | <span data-ttu-id="51dac-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="51dac-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="51dac-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="51dac-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/addFavorite
```

## <a name="request-headers"></a><span data-ttu-id="51dac-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="51dac-116">Request headers</span></span>
| <span data-ttu-id="51dac-117">标头</span><span class="sxs-lookup"><span data-stu-id="51dac-117">Header</span></span>       | <span data-ttu-id="51dac-118">值</span><span class="sxs-lookup"><span data-stu-id="51dac-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="51dac-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="51dac-119">Authorization</span></span>  | <span data-ttu-id="51dac-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="51dac-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="51dac-122">Prefer</span><span class="sxs-lookup"><span data-stu-id="51dac-122">Prefer</span></span> | <span data-ttu-id="51dac-123">return=minimal。</span><span class="sxs-lookup"><span data-stu-id="51dac-123">return=minimal.</span></span> <span data-ttu-id="51dac-124">如果 minimal 响应头包含在请求头中，那么成功响应返回 `204 No Content` 代码。</span><span class="sxs-lookup"><span data-stu-id="51dac-124">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="51dac-125">可选。</span><span class="sxs-lookup"><span data-stu-id="51dac-125">Optional.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="51dac-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="51dac-126">Request body</span></span>
<span data-ttu-id="51dac-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="51dac-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51dac-128">响应</span><span class="sxs-lookup"><span data-stu-id="51dac-128">Response</span></span>
<span data-ttu-id="51dac-p105">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="51dac-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51dac-131">示例</span><span class="sxs-lookup"><span data-stu-id="51dac-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="51dac-132">请求</span><span class="sxs-lookup"><span data-stu-id="51dac-132">Request</span></span>
<span data-ttu-id="51dac-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="51dac-133">The following is an example of the request body.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_addfavorite"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/addFavorite
```

#### <a name="response"></a><span data-ttu-id="51dac-134">响应</span><span class="sxs-lookup"><span data-stu-id="51dac-134">Response</span></span>
<span data-ttu-id="51dac-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="51dac-135">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: addFavorite",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
