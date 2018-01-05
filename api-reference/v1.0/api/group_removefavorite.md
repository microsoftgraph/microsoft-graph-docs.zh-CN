# <a name="group-removefavorite"></a><span data-ttu-id="a2b5d-101">group: removeFavorite</span><span class="sxs-lookup"><span data-stu-id="a2b5d-101">group: removeFavorite</span></span>
<span data-ttu-id="a2b5d-p101">从当前用户收藏夹组列表中删除组。仅支持 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="a2b5d-p101">Remove the group from the list of the current user's favorite groups. Supported for only Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="a2b5d-104">权限</span><span class="sxs-lookup"><span data-stu-id="a2b5d-104">Permissions</span></span>
<span data-ttu-id="a2b5d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a2b5d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a2b5d-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="a2b5d-107">Permission type</span></span>      | <span data-ttu-id="a2b5d-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a2b5d-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a2b5d-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a2b5d-109">Delegated (work or school account)</span></span> | <span data-ttu-id="a2b5d-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2b5d-110">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a2b5d-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a2b5d-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2b5d-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="a2b5d-112">Not supported.</span></span>    |
|<span data-ttu-id="a2b5d-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="a2b5d-113">Application</span></span> | <span data-ttu-id="a2b5d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a2b5d-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a2b5d-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a2b5d-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/removeFavorite
```
## <a name="request-headers"></a><span data-ttu-id="a2b5d-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="a2b5d-116">Request headers</span></span>
| <span data-ttu-id="a2b5d-117">标头</span><span class="sxs-lookup"><span data-stu-id="a2b5d-117">Header</span></span>       | <span data-ttu-id="a2b5d-118">值</span><span class="sxs-lookup"><span data-stu-id="a2b5d-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a2b5d-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2b5d-119">Authorization</span></span>  | <span data-ttu-id="a2b5d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a2b5d-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a2b5d-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="a2b5d-122">Request body</span></span>
<span data-ttu-id="a2b5d-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a2b5d-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a2b5d-124">响应</span><span class="sxs-lookup"><span data-stu-id="a2b5d-124">Response</span></span>
<span data-ttu-id="a2b5d-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="a2b5d-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2b5d-127">示例</span><span class="sxs-lookup"><span data-stu-id="a2b5d-127">Example</span></span>
<span data-ttu-id="a2b5d-128">下面的示例展示了如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="a2b5d-128">Here is an example of how to call this API.</span></span>

#### <a name="request"></a><span data-ttu-id="a2b5d-129">请求</span><span class="sxs-lookup"><span data-stu-id="a2b5d-129">Request</span></span>
<span data-ttu-id="a2b5d-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a2b5d-130">The following is an example of the request body.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_removefavorite"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/removeFavorite
```

#### <a name="response"></a><span data-ttu-id="a2b5d-131">响应</span><span class="sxs-lookup"><span data-stu-id="a2b5d-131">Response</span></span>
<span data-ttu-id="a2b5d-132">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a2b5d-132">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: removeFavorite",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->