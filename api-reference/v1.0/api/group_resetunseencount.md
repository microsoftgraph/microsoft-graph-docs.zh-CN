# <a name="group-resetunseencount"></a><span data-ttu-id="2d260-101">组：resetUnseenCount</span><span class="sxs-lookup"><span data-stu-id="2d260-101">group: resetUnseenCount</span></span>

<span data-ttu-id="2d260-p101">重置当前用户自上次访问后未查看的所有帖子的 unseenCount。仅支持 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="2d260-p101">Reset the unseenCount of all the posts that the current user has not seen since their last visit. Supported for only Office 365 groups.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2d260-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="2d260-104">Prerequisites</span></span>
<span data-ttu-id="2d260-105">要执行此 API，需要以下**范围**之一：*Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="2d260-105">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All*</span></span> 
## <a name="http-request"></a><span data-ttu-id="2d260-106">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2d260-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/resetUnseenCount
```
## <a name="request-headers"></a><span data-ttu-id="2d260-107">请求标头</span><span class="sxs-lookup"><span data-stu-id="2d260-107">Request headers</span></span>
| <span data-ttu-id="2d260-108">标头</span><span class="sxs-lookup"><span data-stu-id="2d260-108">Header</span></span>       | <span data-ttu-id="2d260-109">值</span><span class="sxs-lookup"><span data-stu-id="2d260-109">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2d260-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d260-110">Authorization</span></span>  | <span data-ttu-id="2d260-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2d260-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2d260-113">请求正文</span><span class="sxs-lookup"><span data-stu-id="2d260-113">Request body</span></span>
<span data-ttu-id="2d260-114">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2d260-114">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2d260-115">响应</span><span class="sxs-lookup"><span data-stu-id="2d260-115">Response</span></span>

<span data-ttu-id="2d260-p103">如果成功，此方法返回 `200, OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="2d260-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d260-118">示例</span><span class="sxs-lookup"><span data-stu-id="2d260-118">Example</span></span>
<span data-ttu-id="2d260-119">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="2d260-119">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2d260-120">请求</span><span class="sxs-lookup"><span data-stu-id="2d260-120">Request</span></span>
<span data-ttu-id="2d260-121">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2d260-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_resetunseencount"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/resetUnseenCount
```

##### <a name="response"></a><span data-ttu-id="2d260-122">响应</span><span class="sxs-lookup"><span data-stu-id="2d260-122">Response</span></span>
<span data-ttu-id="2d260-123">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="2d260-123">Here is an example of the response.</span></span> 
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
  "description": "group: resetUnseenCount",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
