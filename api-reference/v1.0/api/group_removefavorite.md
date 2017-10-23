# <a name="group-removefavorite"></a><span data-ttu-id="d0718-101">group: removeFavorite</span><span class="sxs-lookup"><span data-stu-id="d0718-101">group: removeFavorite</span></span>
<span data-ttu-id="d0718-p101">从当前用户收藏夹组列表中删除组。仅支持 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="d0718-p101">Remove the group from the list of the current user's favorite groups. Supported for only Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="d0718-104">权限</span><span class="sxs-lookup"><span data-stu-id="d0718-104">Permissions</span></span>
<span data-ttu-id="d0718-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="d0718-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d0718-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="d0718-107">Permission type</span></span>      | <span data-ttu-id="d0718-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d0718-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0718-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d0718-109">Delegated (work or school account)</span></span> | <span data-ttu-id="d0718-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0718-110">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d0718-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d0718-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0718-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="d0718-112">Not supported.</span></span>    |
|<span data-ttu-id="d0718-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="d0718-113">Application</span></span> | <span data-ttu-id="d0718-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0718-114">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d0718-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d0718-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/removeFavorite
```
## <a name="request-headers"></a><span data-ttu-id="d0718-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="d0718-116">Request headers</span></span>
| <span data-ttu-id="d0718-117">标头</span><span class="sxs-lookup"><span data-stu-id="d0718-117">Header</span></span>       | <span data-ttu-id="d0718-118">值</span><span class="sxs-lookup"><span data-stu-id="d0718-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d0718-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0718-119">Authorization</span></span>  | <span data-ttu-id="d0718-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d0718-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d0718-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="d0718-122">Request body</span></span>
<span data-ttu-id="d0718-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d0718-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d0718-124">响应</span><span class="sxs-lookup"><span data-stu-id="d0718-124">Response</span></span>

<span data-ttu-id="d0718-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="d0718-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0718-127">示例</span><span class="sxs-lookup"><span data-stu-id="d0718-127">Example</span></span>
<span data-ttu-id="d0718-128">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="d0718-128">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d0718-129">请求</span><span class="sxs-lookup"><span data-stu-id="d0718-129">Request</span></span>
<span data-ttu-id="d0718-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d0718-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_removefavorite"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/removeFavorite
```

##### <a name="response"></a><span data-ttu-id="d0718-131">响应</span><span class="sxs-lookup"><span data-stu-id="d0718-131">Response</span></span>
<span data-ttu-id="d0718-132">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d0718-132">Here is an example of the response.</span></span>
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
  "description": "group: removeFavorite",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->