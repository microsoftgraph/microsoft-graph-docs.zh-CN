# <a name="delete-subscription"></a><span data-ttu-id="e2f53-101">删除订阅</span><span class="sxs-lookup"><span data-stu-id="e2f53-101">Delete subscription</span></span>

<span data-ttu-id="e2f53-102">删除订阅。</span><span class="sxs-lookup"><span data-stu-id="e2f53-102">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="e2f53-103">权限</span><span class="sxs-lookup"><span data-stu-id="e2f53-103">Permissions</span></span>

<span data-ttu-id="e2f53-p101">下表列出了对各个资源所需权限的建议。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="e2f53-p101">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="e2f53-106">资源类型/项</span><span class="sxs-lookup"><span data-stu-id="e2f53-106">Resource type / Item</span></span>        | <span data-ttu-id="e2f53-107">权限</span><span class="sxs-lookup"><span data-stu-id="e2f53-107">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="e2f53-108">联系人</span><span class="sxs-lookup"><span data-stu-id="e2f53-108">Contacts</span></span>                    | <span data-ttu-id="e2f53-109">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="e2f53-109">Contacts.Read</span></span>       |
| <span data-ttu-id="e2f53-110">Conversations</span><span class="sxs-lookup"><span data-stu-id="e2f53-110">Conversations</span></span>               | <span data-ttu-id="e2f53-111">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2f53-111">Group.Read.All</span></span>      |
| <span data-ttu-id="e2f53-112">Events</span><span class="sxs-lookup"><span data-stu-id="e2f53-112">Events</span></span>                      | <span data-ttu-id="e2f53-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e2f53-113">Calendars.Read</span></span>      |
| <span data-ttu-id="e2f53-114">Messages</span><span class="sxs-lookup"><span data-stu-id="e2f53-114">Messages</span></span>                    | <span data-ttu-id="e2f53-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="e2f53-115">Mail.Read</span></span>           |
| <span data-ttu-id="e2f53-116">Drive（用户的 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="e2f53-116">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="e2f53-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e2f53-117">Files.ReadWrite</span></span>     |
| <span data-ttu-id="e2f53-118">Drives（Sharepoint 共享内容和驱动器）</span><span class="sxs-lookup"><span data-stu-id="e2f53-118">Drives (Sharepoint shared content and drives)</span></span> | <span data-ttu-id="e2f53-119">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2f53-119">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2f53-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e2f53-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /subscriptions/{subscriptionId}
```
## <a name="request-headers"></a><span data-ttu-id="e2f53-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="e2f53-121">Request headers</span></span>
| <span data-ttu-id="e2f53-122">名称</span><span class="sxs-lookup"><span data-stu-id="e2f53-122">Name</span></span>       | <span data-ttu-id="e2f53-123">类型</span><span class="sxs-lookup"><span data-stu-id="e2f53-123">Type</span></span> | <span data-ttu-id="e2f53-124">说明</span><span class="sxs-lookup"><span data-stu-id="e2f53-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e2f53-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2f53-125">Authorization</span></span>  | <span data-ttu-id="e2f53-126">string</span><span class="sxs-lookup"><span data-stu-id="e2f53-126">string</span></span>  | <span data-ttu-id="e2f53-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e2f53-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e2f53-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="e2f53-129">Request body</span></span>
<span data-ttu-id="e2f53-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e2f53-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2f53-131">响应</span><span class="sxs-lookup"><span data-stu-id="e2f53-131">Response</span></span>

<span data-ttu-id="e2f53-132">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="e2f53-132">If successful, this method returns a `204 No Content` response code.</span></span>
## <a name="example"></a><span data-ttu-id="e2f53-133">示例</span><span class="sxs-lookup"><span data-stu-id="e2f53-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e2f53-134">请求</span><span class="sxs-lookup"><span data-stu-id="e2f53-134">Request</span></span>
<span data-ttu-id="e2f53-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e2f53-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{subscriptionId}
```
##### <a name="response"></a><span data-ttu-id="e2f53-136">响应</span><span class="sxs-lookup"><span data-stu-id="e2f53-136">Response</span></span>
<span data-ttu-id="e2f53-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e2f53-137">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->
```http
HTTP/1.1 204 No Content
```


<!-- {
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
