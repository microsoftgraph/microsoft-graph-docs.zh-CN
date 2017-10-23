# <a name="post-forward"></a><span data-ttu-id="fdffc-101">帖子：转发</span><span class="sxs-lookup"><span data-stu-id="fdffc-101">post: forward</span></span>

<span data-ttu-id="fdffc-p101">将帖子转发给收件人。可以在请求中同时指定父对话和线程，或者仅指定父线程，而不指定父对话。</span><span class="sxs-lookup"><span data-stu-id="fdffc-p101">Forward a post to a recipient. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span> 

## <a name="permissions"></a><span data-ttu-id="fdffc-104">权限</span><span class="sxs-lookup"><span data-stu-id="fdffc-104">Permissions</span></span>
<span data-ttu-id="fdffc-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="fdffc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fdffc-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="fdffc-107">Permission type</span></span>      | <span data-ttu-id="fdffc-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fdffc-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fdffc-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fdffc-109">Delegated (work or school account)</span></span> | <span data-ttu-id="fdffc-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdffc-110">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="fdffc-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fdffc-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fdffc-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="fdffc-112">Not supported.</span></span>    |
|<span data-ttu-id="fdffc-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="fdffc-113">Application</span></span> | <span data-ttu-id="fdffc-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdffc-114">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fdffc-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fdffc-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/forward
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/forward

```
## <a name="request-headers"></a><span data-ttu-id="fdffc-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="fdffc-116">Request headers</span></span>
| <span data-ttu-id="fdffc-117">标头</span><span class="sxs-lookup"><span data-stu-id="fdffc-117">Header</span></span>       | <span data-ttu-id="fdffc-118">值</span><span class="sxs-lookup"><span data-stu-id="fdffc-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fdffc-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="fdffc-119">Authorization</span></span>  | <span data-ttu-id="fdffc-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fdffc-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fdffc-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="fdffc-122">Request body</span></span>
<span data-ttu-id="fdffc-123">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="fdffc-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fdffc-124">参数</span><span class="sxs-lookup"><span data-stu-id="fdffc-124">Parameter</span></span>    | <span data-ttu-id="fdffc-125">类型</span><span class="sxs-lookup"><span data-stu-id="fdffc-125">Type</span></span>   |<span data-ttu-id="fdffc-126">说明</span><span class="sxs-lookup"><span data-stu-id="fdffc-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fdffc-127">注释</span><span class="sxs-lookup"><span data-stu-id="fdffc-127">comment</span></span>|<span data-ttu-id="fdffc-128">String</span><span class="sxs-lookup"><span data-stu-id="fdffc-128">String</span></span>|<span data-ttu-id="fdffc-129">与帖子一起转发的可选注释。</span><span class="sxs-lookup"><span data-stu-id="fdffc-129">Optional comment that is forwarded together with the post.</span></span>|
|<span data-ttu-id="fdffc-130">toRecipients</span><span class="sxs-lookup"><span data-stu-id="fdffc-130">toRecipients</span></span>|<span data-ttu-id="fdffc-131">[收件人](../resources/recipient.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fdffc-131">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="fdffc-132">线程要转发至的收件人。</span><span class="sxs-lookup"><span data-stu-id="fdffc-132">The recipients to whom the threaded is forwarded to.</span></span>|

## <a name="response"></a><span data-ttu-id="fdffc-133">响应</span><span class="sxs-lookup"><span data-stu-id="fdffc-133">Response</span></span>

<span data-ttu-id="fdffc-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="fdffc-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fdffc-136">示例</span><span class="sxs-lookup"><span data-stu-id="fdffc-136">Example</span></span>
<span data-ttu-id="fdffc-137">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="fdffc-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fdffc-138">请求</span><span class="sxs-lookup"><span data-stu-id="fdffc-138">Request</span></span>
<span data-ttu-id="fdffc-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fdffc-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_forward"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/forward
Content-type: application/json
Content-length: 166

{
  "comment": "comment-value",
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="fdffc-140">响应</span><span class="sxs-lookup"><span data-stu-id="fdffc-140">Response</span></span>
<span data-ttu-id="fdffc-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="fdffc-141">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "post: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
