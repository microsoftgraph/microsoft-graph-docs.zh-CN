# <a name="group-subscribebymail"></a><span data-ttu-id="3398a-101">组：subscribeByMail</span><span class="sxs-lookup"><span data-stu-id="3398a-101">group: subscribeByMail</span></span>

<span data-ttu-id="3398a-p101">调用此方法将允许当前用户接收有关该组中新帖子、活动和文件的电子邮件通知。仅支持 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="3398a-p101">Calling this method will enable the current user to receive email notifications for this group, about new posts, events, and files in that group. Supported for only Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="3398a-104">权限</span><span class="sxs-lookup"><span data-stu-id="3398a-104">Permissions</span></span>
<span data-ttu-id="3398a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="3398a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3398a-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="3398a-107">Permission type</span></span>      | <span data-ttu-id="3398a-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3398a-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3398a-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3398a-109">Delegated (work or school account)</span></span> | <span data-ttu-id="3398a-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3398a-110">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3398a-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3398a-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3398a-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="3398a-112">Not supported.</span></span>    |
|<span data-ttu-id="3398a-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="3398a-113">Application</span></span> | <span data-ttu-id="3398a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3398a-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3398a-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3398a-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/subscribeByMail
```
## <a name="request-headers"></a><span data-ttu-id="3398a-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="3398a-116">Request headers</span></span>
| <span data-ttu-id="3398a-117">标头</span><span class="sxs-lookup"><span data-stu-id="3398a-117">Header</span></span>       | <span data-ttu-id="3398a-118">值</span><span class="sxs-lookup"><span data-stu-id="3398a-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3398a-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="3398a-119">Authorization</span></span>  | <span data-ttu-id="3398a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3398a-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3398a-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="3398a-122">Request body</span></span>
<span data-ttu-id="3398a-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3398a-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3398a-124">响应</span><span class="sxs-lookup"><span data-stu-id="3398a-124">Response</span></span>
<span data-ttu-id="3398a-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="3398a-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3398a-127">示例</span><span class="sxs-lookup"><span data-stu-id="3398a-127">Example</span></span>
<span data-ttu-id="3398a-128">下面的示例展示了如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="3398a-128">Here is an example of how to call this API.</span></span>

#### <a name="request"></a><span data-ttu-id="3398a-129">请求</span><span class="sxs-lookup"><span data-stu-id="3398a-129">Request</span></span>
<span data-ttu-id="3398a-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3398a-130">The following is an example of the request body.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_subscribebymail"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/subscribeByMail
```

#### <a name="response"></a><span data-ttu-id="3398a-131">响应</span><span class="sxs-lookup"><span data-stu-id="3398a-131">Response</span></span>
<span data-ttu-id="3398a-132">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3398a-132">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: subscribeByMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->