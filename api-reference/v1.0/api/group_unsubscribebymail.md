# <a name="group-unsubscribebymail"></a><span data-ttu-id="84d96-101">组：unsubscribeByMail</span><span class="sxs-lookup"><span data-stu-id="84d96-101">group: unsubscribeByMail</span></span>

<span data-ttu-id="84d96-p101">调用此方法可使当前用户在该组中收到有关该组的新帖子、事件和文件的电子邮件通知。仅支持 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="84d96-p101">Calling this method will prevent the current user from receiving email notifications for this group about new posts, events, and files in that group. Supported for only Office 365 groups.</span></span> 
## <a name="prerequisites"></a><span data-ttu-id="84d96-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="84d96-104">Prerequisites</span></span>
<span data-ttu-id="84d96-105">要执行此 API，需要以下**范围**之一：*Group.ReadWrite.All* 
*Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="84d96-105">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All* 
*Group.ReadWrite.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="84d96-106">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="84d96-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/unsubscribeByMail
```
## <a name="request-headers"></a><span data-ttu-id="84d96-107">请求标头</span><span class="sxs-lookup"><span data-stu-id="84d96-107">Request headers</span></span>
| <span data-ttu-id="84d96-108">标头</span><span class="sxs-lookup"><span data-stu-id="84d96-108">Header</span></span>       | <span data-ttu-id="84d96-109">值</span><span class="sxs-lookup"><span data-stu-id="84d96-109">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="84d96-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="84d96-110">Authorization</span></span>  | <span data-ttu-id="84d96-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="84d96-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="84d96-113">请求正文</span><span class="sxs-lookup"><span data-stu-id="84d96-113">Request body</span></span>

## <a name="response"></a><span data-ttu-id="84d96-114">响应</span><span class="sxs-lookup"><span data-stu-id="84d96-114">Response</span></span>

<span data-ttu-id="84d96-p103">如果成功，此方法返回 `200, OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="84d96-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84d96-117">示例</span><span class="sxs-lookup"><span data-stu-id="84d96-117">Example</span></span>
<span data-ttu-id="84d96-118">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="84d96-118">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="84d96-119">请求</span><span class="sxs-lookup"><span data-stu-id="84d96-119">Request</span></span>
<span data-ttu-id="84d96-120">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="84d96-120">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_unsubscribebymail"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/unsubscribeByMail
```

##### <a name="response"></a><span data-ttu-id="84d96-121">响应</span><span class="sxs-lookup"><span data-stu-id="84d96-121">Response</span></span>
<span data-ttu-id="84d96-122">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="84d96-122">Here is an example of the response.</span></span> 
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
  "description": "group: unsubscribeByMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
