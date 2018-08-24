# <a name="delete-subscription"></a><span data-ttu-id="d1104-101">删除订阅</span><span class="sxs-lookup"><span data-stu-id="d1104-101">Delete subscription</span></span>

<span data-ttu-id="d1104-102">删除订阅。</span><span class="sxs-lookup"><span data-stu-id="d1104-102">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="d1104-103">权限</span><span class="sxs-lookup"><span data-stu-id="d1104-103">Permissions</span></span>

<span data-ttu-id="d1104-p101">下表列出了对各个资源所需权限的建议。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="d1104-p101">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="d1104-106">资源类型/项</span><span class="sxs-lookup"><span data-stu-id="d1104-106">Resource type / Item</span></span>        | <span data-ttu-id="d1104-107">权限</span><span class="sxs-lookup"><span data-stu-id="d1104-107">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="d1104-108">联系人</span><span class="sxs-lookup"><span data-stu-id="d1104-108">Contacts</span></span>                    | <span data-ttu-id="d1104-109">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="d1104-109">Contacts.Read</span></span>       |
| <span data-ttu-id="d1104-110">对话</span><span class="sxs-lookup"><span data-stu-id="d1104-110">Conversations</span></span>               | <span data-ttu-id="d1104-111">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="d1104-111">Group.Read.All</span></span>      |
| <span data-ttu-id="d1104-112">事件</span><span class="sxs-lookup"><span data-stu-id="d1104-112">Events</span></span>                      | <span data-ttu-id="d1104-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d1104-113">Calendars.Read</span></span>      |
| <span data-ttu-id="d1104-114">消息</span><span class="sxs-lookup"><span data-stu-id="d1104-114">Messages</span></span>                    | <span data-ttu-id="d1104-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="d1104-115">Mail.Read</span></span>           |
| <span data-ttu-id="d1104-116">组</span><span class="sxs-lookup"><span data-stu-id="d1104-116">Groups</span></span>                      | <span data-ttu-id="d1104-117">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="d1104-117">Group.Read.All</span></span>      |
| <span data-ttu-id="d1104-118">用户</span><span class="sxs-lookup"><span data-stu-id="d1104-118">Users</span></span>                       | <span data-ttu-id="d1104-119">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="d1104-119">User.Read.All</span></span>       |
| <span data-ttu-id="d1104-120">Drive（用户的 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="d1104-120">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="d1104-121">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d1104-121">Files.ReadWrite</span></span>     |
| <span data-ttu-id="d1104-122">驱动器（SharePoint 共享的内容和驱动器）</span><span class="sxs-lookup"><span data-stu-id="d1104-122">Drives (Sharepoint shared content and drives)</span></span> | <span data-ttu-id="d1104-123">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1104-123">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d1104-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d1104-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d1104-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="d1104-125">Request headers</span></span>

| <span data-ttu-id="d1104-126">名称</span><span class="sxs-lookup"><span data-stu-id="d1104-126">Name</span></span>       | <span data-ttu-id="d1104-127">类型</span><span class="sxs-lookup"><span data-stu-id="d1104-127">Type</span></span> | <span data-ttu-id="d1104-128">说明</span><span class="sxs-lookup"><span data-stu-id="d1104-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d1104-129">授权</span><span class="sxs-lookup"><span data-stu-id="d1104-129">Authorization</span></span>  | <span data-ttu-id="d1104-130">字符串</span><span class="sxs-lookup"><span data-stu-id="d1104-130">string</span></span>  | <span data-ttu-id="d1104-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d1104-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d1104-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="d1104-133">Request body</span></span>

<span data-ttu-id="d1104-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d1104-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1104-135">响应</span><span class="sxs-lookup"><span data-stu-id="d1104-135">Response</span></span>

<span data-ttu-id="d1104-136">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="d1104-136">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d1104-137">示例</span><span class="sxs-lookup"><span data-stu-id="d1104-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d1104-138">请求</span><span class="sxs-lookup"><span data-stu-id="d1104-138">Request</span></span>

<span data-ttu-id="d1104-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d1104-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="d1104-140">响应</span><span class="sxs-lookup"><span data-stu-id="d1104-140">Response</span></span>

<span data-ttu-id="d1104-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d1104-141">Here is an example of the response.</span></span>
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
