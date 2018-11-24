# <a name="delete-subscription"></a><span data-ttu-id="673ac-101">删除订阅</span><span class="sxs-lookup"><span data-stu-id="673ac-101">Delete subscription</span></span>

<span data-ttu-id="673ac-102">删除订阅。</span><span class="sxs-lookup"><span data-stu-id="673ac-102">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="673ac-103">权限</span><span class="sxs-lookup"><span data-stu-id="673ac-103">Permissions</span></span>

<span data-ttu-id="673ac-p101">下表列出了对各个资源所需权限的建议。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="673ac-p101">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="673ac-106">资源类型/项</span><span class="sxs-lookup"><span data-stu-id="673ac-106">Resource type / Item</span></span>        | <span data-ttu-id="673ac-107">权限</span><span class="sxs-lookup"><span data-stu-id="673ac-107">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="673ac-108">联系人</span><span class="sxs-lookup"><span data-stu-id="673ac-108">Contacts</span></span>                    | <span data-ttu-id="673ac-109">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="673ac-109">Contacts.Read</span></span>       |
| <span data-ttu-id="673ac-110">Conversations</span><span class="sxs-lookup"><span data-stu-id="673ac-110">Conversations</span></span>               | <span data-ttu-id="673ac-111">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="673ac-111">Group.Read.All</span></span>      |
| <span data-ttu-id="673ac-112">Events</span><span class="sxs-lookup"><span data-stu-id="673ac-112">Events</span></span>                      | <span data-ttu-id="673ac-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="673ac-113">Calendars.Read</span></span>      |
| <span data-ttu-id="673ac-114">Messages</span><span class="sxs-lookup"><span data-stu-id="673ac-114">Messages</span></span>                    | <span data-ttu-id="673ac-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="673ac-115">Mail.Read</span></span>           |
| <span data-ttu-id="673ac-116">Groups</span><span class="sxs-lookup"><span data-stu-id="673ac-116">Groups</span></span>                      | <span data-ttu-id="673ac-117">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="673ac-117">Group.Read.All</span></span>      |
| <span data-ttu-id="673ac-118">Users</span><span class="sxs-lookup"><span data-stu-id="673ac-118">Users</span></span>                       | <span data-ttu-id="673ac-119">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="673ac-119">User.Read.All</span></span>       |
| <span data-ttu-id="673ac-120">Drive（用户的 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="673ac-120">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="673ac-121">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="673ac-121">Files.ReadWrite</span></span>     |
| <span data-ttu-id="673ac-122">驱动器 （共享的 SharePoint 内容和驱动器）</span><span class="sxs-lookup"><span data-stu-id="673ac-122">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="673ac-123">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="673ac-123">Files.ReadWrite.All</span></span> |
|<span data-ttu-id="673ac-124">安全警报</span><span class="sxs-lookup"><span data-stu-id="673ac-124">Security alert</span></span>| <span data-ttu-id="673ac-125">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="673ac-125">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="673ac-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="673ac-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="673ac-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="673ac-127">Request headers</span></span>

| <span data-ttu-id="673ac-128">名称</span><span class="sxs-lookup"><span data-stu-id="673ac-128">Name</span></span>       | <span data-ttu-id="673ac-129">类型</span><span class="sxs-lookup"><span data-stu-id="673ac-129">Type</span></span> | <span data-ttu-id="673ac-130">说明</span><span class="sxs-lookup"><span data-stu-id="673ac-130">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="673ac-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="673ac-131">Authorization</span></span>  | <span data-ttu-id="673ac-132">string</span><span class="sxs-lookup"><span data-stu-id="673ac-132">string</span></span>  | <span data-ttu-id="673ac-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="673ac-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="673ac-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="673ac-135">Request body</span></span>

<span data-ttu-id="673ac-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="673ac-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="673ac-137">响应</span><span class="sxs-lookup"><span data-stu-id="673ac-137">Response</span></span>

<span data-ttu-id="673ac-138">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="673ac-138">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="673ac-139">示例</span><span class="sxs-lookup"><span data-stu-id="673ac-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="673ac-140">请求</span><span class="sxs-lookup"><span data-stu-id="673ac-140">Request</span></span>

<span data-ttu-id="673ac-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="673ac-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="673ac-142">响应</span><span class="sxs-lookup"><span data-stu-id="673ac-142">Response</span></span>

<span data-ttu-id="673ac-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="673ac-143">Here is an example of the response.</span></span>
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
