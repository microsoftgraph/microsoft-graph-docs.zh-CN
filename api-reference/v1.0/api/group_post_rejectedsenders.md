# <a name="create-rejectedsender"></a><span data-ttu-id="f149e-101">创建 rejectedSender</span><span class="sxs-lookup"><span data-stu-id="f149e-101">Create rejectedSender</span></span>

<span data-ttu-id="f149e-102">将新用户或组添加到 acceptedSender 列表中。</span><span class="sxs-lookup"><span data-stu-id="f149e-102">Add a new user or group to the rejectedSender list.</span></span>

<span data-ttu-id="f149e-p101">在请求主体的 `@odata.id` 中指定用户或组。已拒绝的发件人列表中的用户无法发布到组对话（在 POST 请求 URL 中标识）。确保未在拒绝的发件人和接受的发件人列表中指定同一用户或组，否则会发生错误。</span><span class="sxs-lookup"><span data-stu-id="f149e-p101">Specify the user or group in `@odata.id` in the request body. Users in the rejected senders list cannot post to conversations of the group (identified in the POST request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>
## <a name="permissions"></a><span data-ttu-id="f149e-106">权限</span><span class="sxs-lookup"><span data-stu-id="f149e-106">Permissions</span></span>
<span data-ttu-id="f149e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="f149e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f149e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f149e-109">Permission type</span></span>      | <span data-ttu-id="f149e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f149e-110">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="f149e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f149e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f149e-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f149e-112">Group.ReadWrite.All</span></span>    | 
|<span data-ttu-id="f149e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f149e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f149e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f149e-114">Not supported.</span></span>    | 
|<span data-ttu-id="f149e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f149e-115">Application</span></span> | <span data-ttu-id="f149e-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f149e-116">Group.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f149e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f149e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/rejectedSenders/$ref
```
## <a name="request-headers"></a><span data-ttu-id="f149e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f149e-118">Request headers</span></span>
| <span data-ttu-id="f149e-119">标头</span><span class="sxs-lookup"><span data-stu-id="f149e-119">Header</span></span>       | <span data-ttu-id="f149e-120">值</span><span class="sxs-lookup"><span data-stu-id="f149e-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f149e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f149e-121">Authorization</span></span>  | <span data-ttu-id="f149e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f149e-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f149e-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="f149e-124">Request body</span></span>
<span data-ttu-id="f149e-125">在请求正文中，提供 user 或 group 对象的 ID。</span><span class="sxs-lookup"><span data-stu-id="f149e-125">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="f149e-126">响应</span><span class="sxs-lookup"><span data-stu-id="f149e-126">Response</span></span>

<span data-ttu-id="f149e-127">此方法返回 `204, No Content` 响应代码，不返回任何响应正文。</span><span class="sxs-lookup"><span data-stu-id="f149e-127">This method returns `204, No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="f149e-128">示例</span><span class="sxs-lookup"><span data-stu-id="f149e-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f149e-129">请求</span><span class="sxs-lookup"><span data-stu-id="f149e-129">Request</span></span>
<span data-ttu-id="f149e-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f149e-130">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="f149e-131">响应</span><span class="sxs-lookup"><span data-stu-id="f149e-131">Response</span></span>
<span data-ttu-id="f149e-132">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f149e-132">Here is an example of the response.</span></span>
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
