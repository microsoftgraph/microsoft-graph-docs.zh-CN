# <a name="create-acceptedsender"></a><span data-ttu-id="18693-101">删除 acceptedSender</span><span class="sxs-lookup"><span data-stu-id="18693-101">Create acceptedSender</span></span>

<span data-ttu-id="18693-102">向 acceptedSender 列表中添加新用户或组。</span><span class="sxs-lookup"><span data-stu-id="18693-102">Add a new user or group to the acceptedSender list.</span></span>

<span data-ttu-id="18693-p101">在请求主体的 `@odata.id` 中指定用户或组。已接受的发件人列表中的用户可以发布到组对话。确保未在接受的发件人和拒绝的发件人列表中指定同一用户或组，否则会发生错误。</span><span class="sxs-lookup"><span data-stu-id="18693-p101">Specify the user or group in `@odata.id` in the request body. Users in the accepted senders list can post to conversations of the group . Make sure you do not specify the same user or group in the accepted senders and rejected senders lists, otherwise you will get an error.</span></span>
## <a name="permissions"></a><span data-ttu-id="18693-106">权限</span><span class="sxs-lookup"><span data-stu-id="18693-106">Permissions</span></span>
<span data-ttu-id="18693-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="18693-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="18693-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="18693-109">Permission type</span></span>      | <span data-ttu-id="18693-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="18693-110">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="18693-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="18693-111">Delegated (work or school account)</span></span> | <span data-ttu-id="18693-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18693-112">Group.ReadWrite.All</span></span>    | 
|<span data-ttu-id="18693-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="18693-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18693-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="18693-114">Not supported.</span></span>    | 
|<span data-ttu-id="18693-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="18693-115">Application</span></span> | <span data-ttu-id="18693-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18693-116">Group.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="18693-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="18693-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/acceptedSenders/$ref
```
## <a name="request-headers"></a><span data-ttu-id="18693-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="18693-118">Request headers</span></span>
| <span data-ttu-id="18693-119">标头</span><span class="sxs-lookup"><span data-stu-id="18693-119">Header</span></span>       | <span data-ttu-id="18693-120">值</span><span class="sxs-lookup"><span data-stu-id="18693-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="18693-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="18693-121">Authorization</span></span>  | <span data-ttu-id="18693-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="18693-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="18693-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="18693-124">Request body</span></span>
<span data-ttu-id="18693-125">在请求正文中，提供 user 或 group 对象的 ID。</span><span class="sxs-lookup"><span data-stu-id="18693-125">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="18693-126">响应</span><span class="sxs-lookup"><span data-stu-id="18693-126">Response</span></span>

<span data-ttu-id="18693-127">此方法返回 `204, No Content` 响应代码，不返回任何响应正文。</span><span class="sxs-lookup"><span data-stu-id="18693-127">This method returns `204, No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="18693-128">示例</span><span class="sxs-lookup"><span data-stu-id="18693-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="18693-129">请求</span><span class="sxs-lookup"><span data-stu-id="18693-129">Request</span></span>
<span data-ttu-id="18693-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="18693-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/acceptedSenders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id":"https://graph.microsoft.com/v1.0/users/alexd@contoso.com"
}
```
##### <a name="response"></a><span data-ttu-id="18693-131">响应</span><span class="sxs-lookup"><span data-stu-id="18693-131">Response</span></span>
<span data-ttu-id="18693-132">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="18693-132">Here is an example of the response.</span></span>
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
  "description": "Create acceptedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
