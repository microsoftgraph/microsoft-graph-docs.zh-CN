# <a name="delete-subscription"></a><span data-ttu-id="f83b8-101">删除订阅</span><span class="sxs-lookup"><span data-stu-id="f83b8-101">Delete subscription</span></span>

<span data-ttu-id="f83b8-102">删除订阅。</span><span class="sxs-lookup"><span data-stu-id="f83b8-102">Delete a subscription.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f83b8-103">先决条件</span><span class="sxs-lookup"><span data-stu-id="f83b8-103">Prerequisites</span></span>

<span data-ttu-id="f83b8-104">下表列出了对各个资源所需权限的建议。</span><span class="sxs-lookup"><span data-stu-id="f83b8-104">The following table lists the suggested permission needed for each resource.</span></span>

| <span data-ttu-id="f83b8-105">资源类型/项</span><span class="sxs-lookup"><span data-stu-id="f83b8-105">Resource type / Item</span></span>        | <span data-ttu-id="f83b8-106">范围</span><span class="sxs-lookup"><span data-stu-id="f83b8-106">Scope</span></span>               |
|-----------------------------|---------------------|
| <span data-ttu-id="f83b8-107">Contacts</span><span class="sxs-lookup"><span data-stu-id="f83b8-107">Contacts</span></span>                    | <span data-ttu-id="f83b8-108">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="f83b8-108">Contacts.Read</span></span>       |
| <span data-ttu-id="f83b8-109">Conversations</span><span class="sxs-lookup"><span data-stu-id="f83b8-109">Conversations</span></span>               | <span data-ttu-id="f83b8-110">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="f83b8-110">Group.Read.All</span></span>      |
| <span data-ttu-id="f83b8-111">Events</span><span class="sxs-lookup"><span data-stu-id="f83b8-111">Events</span></span>                      | <span data-ttu-id="f83b8-112">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f83b8-112">Calendars.Read</span></span>      |
| <span data-ttu-id="f83b8-113">Messages</span><span class="sxs-lookup"><span data-stu-id="f83b8-113">Messages</span></span>                    | <span data-ttu-id="f83b8-114">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="f83b8-114">Mail.Read</span></span>           |
| <span data-ttu-id="f83b8-115">Drive（用户的 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="f83b8-115">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="f83b8-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f83b8-116">Files.ReadWrite</span></span>     |
| <span data-ttu-id="f83b8-117">Drives（Sharepoint 共享内容和驱动器）</span><span class="sxs-lookup"><span data-stu-id="f83b8-117">Drives (Sharepoint shared content and drives)</span></span> | <span data-ttu-id="f83b8-118">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f83b8-118">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f83b8-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f83b8-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /subscriptions/{subscriptionId}
```
## <a name="request-headers"></a><span data-ttu-id="f83b8-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f83b8-120">Request headers</span></span>
| <span data-ttu-id="f83b8-121">名称</span><span class="sxs-lookup"><span data-stu-id="f83b8-121">Name</span></span>       | <span data-ttu-id="f83b8-122">类型</span><span class="sxs-lookup"><span data-stu-id="f83b8-122">Type</span></span> | <span data-ttu-id="f83b8-123">说明</span><span class="sxs-lookup"><span data-stu-id="f83b8-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f83b8-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f83b8-124">Authorization</span></span>  | <span data-ttu-id="f83b8-125">string</span><span class="sxs-lookup"><span data-stu-id="f83b8-125">string</span></span>  | <span data-ttu-id="f83b8-p101">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f83b8-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f83b8-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="f83b8-128">Request body</span></span>
<span data-ttu-id="f83b8-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f83b8-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f83b8-130">响应</span><span class="sxs-lookup"><span data-stu-id="f83b8-130">Response</span></span>

<span data-ttu-id="f83b8-131">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="f83b8-131">If successful, this method returns a `204 No Content` response code.</span></span>
## <a name="example"></a><span data-ttu-id="f83b8-132">示例</span><span class="sxs-lookup"><span data-stu-id="f83b8-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f83b8-133">请求</span><span class="sxs-lookup"><span data-stu-id="f83b8-133">Request</span></span>
<span data-ttu-id="f83b8-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f83b8-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{subscriptionId}
```
##### <a name="response"></a><span data-ttu-id="f83b8-135">响应</span><span class="sxs-lookup"><span data-stu-id="f83b8-135">Response</span></span>
<span data-ttu-id="f83b8-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f83b8-136">Here is an example of the response.</span></span>
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
