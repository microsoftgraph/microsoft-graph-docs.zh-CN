# <a name="create-rejectedsender"></a><span data-ttu-id="57b0b-101">创建 rejectedSender</span><span class="sxs-lookup"><span data-stu-id="57b0b-101">Create rejectedSender</span></span>

<span data-ttu-id="57b0b-102">将新用户或组添加到 acceptedSender 列表中。</span><span class="sxs-lookup"><span data-stu-id="57b0b-102">Add a new user or group to the rejectedSender list.</span></span>

<span data-ttu-id="57b0b-p101">在请求主体的 `@odata.id` 中指定用户或组。已拒绝的发件人列表中的用户无法发布到组对话（在 POST 请求 URL 中标识）。确保未在拒绝的发件人和接受的发件人列表中指定同一用户或组，否则会发生错误。</span><span class="sxs-lookup"><span data-stu-id="57b0b-p101">Specify the user or group in `@odata.id` in the request body. Users in the rejected senders list cannot post to conversations of the group (identified in the POST request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="57b0b-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="57b0b-106">Prerequisites</span></span>
<span data-ttu-id="57b0b-107">要执行此 API，需要以下**范围**之一：*Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="57b0b-107">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="57b0b-108">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="57b0b-108">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/rejectedSenders/$ref
```
## <a name="request-headers"></a><span data-ttu-id="57b0b-109">请求标头</span><span class="sxs-lookup"><span data-stu-id="57b0b-109">Request headers</span></span>
| <span data-ttu-id="57b0b-110">标头</span><span class="sxs-lookup"><span data-stu-id="57b0b-110">Header</span></span>       | <span data-ttu-id="57b0b-111">值</span><span class="sxs-lookup"><span data-stu-id="57b0b-111">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="57b0b-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="57b0b-112">Authorization</span></span>  | <span data-ttu-id="57b0b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="57b0b-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="57b0b-115">请求正文</span><span class="sxs-lookup"><span data-stu-id="57b0b-115">Request body</span></span>
<span data-ttu-id="57b0b-116">在请求正文中，提供 user 或 group 对象的 ID。</span><span class="sxs-lookup"><span data-stu-id="57b0b-116">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="57b0b-117">响应</span><span class="sxs-lookup"><span data-stu-id="57b0b-117">Response</span></span>

<span data-ttu-id="57b0b-118">此方法返回 `204, No Content` 响应代码，不返回任何响应正文。</span><span class="sxs-lookup"><span data-stu-id="57b0b-118">This method returns `204, No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="57b0b-119">示例</span><span class="sxs-lookup"><span data-stu-id="57b0b-119">Example</span></span>
##### <a name="request"></a><span data-ttu-id="57b0b-120">请求</span><span class="sxs-lookup"><span data-stu-id="57b0b-120">Request</span></span>
<span data-ttu-id="57b0b-121">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="57b0b-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/rejectedSenders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id":"https://graph.microsoft.com/v1.0/users/alexd@contoso.com"
}
```
##### <a name="response"></a><span data-ttu-id="57b0b-122">响应</span><span class="sxs-lookup"><span data-stu-id="57b0b-122">Response</span></span>
<span data-ttu-id="57b0b-123">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="57b0b-123">Here is an example of the response.</span></span>
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
  "description": "Create rejectedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
