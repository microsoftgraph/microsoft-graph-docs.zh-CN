<span data-ttu-id="6325f-p101">通过使用其 ID 或路径删除 [DriveItem](../resources/driveitem.md)。注意，使用此方法删除项将把项移动到回收站中，而不是永久删除该项。</span><span class="sxs-lookup"><span data-stu-id="6325f-p101">Delete a [DriveItem](../resources/driveitem.md) by using its ID or path. Note that deleting items using this method will move the items to the recycle bin instead of permanently deleting the item.</span></span>

通过使用其 ID 或路径删除 [DriveItem](../resources/driveitem.md)。注意，使用此方法删除项将把项移动到回收站中，而不是永久删除该项。

## <span data-ttu-id="6325f-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="6325f-104">Prerequisites</span></span>
<a id="prerequisites" class="xliff"></a>
<span data-ttu-id="6325f-105">要执行此 API，需要以下**范围**之一：</span><span class="sxs-lookup"><span data-stu-id="6325f-105">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="6325f-106">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6325f-106">Files.ReadWrite</span></span>
* <span data-ttu-id="6325f-107">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6325f-107">Files.ReadWrite.All</span></span>
* <span data-ttu-id="6325f-108">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6325f-108">Sites.ReadWrite.All</span></span>

## <span data-ttu-id="6325f-109">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6325f-109">HTTP request</span></span>
<a id="http-request" class="xliff"></a>

<!-- { "blockType": "ignored" } -->
```
DELETE /me/drive/items/{item-id}
DELETE /me/drive/root:/{item-path}
DELETE /drives/{drive-id}/items/{item-id}
DELETE /groups/{group-id}/drive/items/{item-id}
```

## <span data-ttu-id="6325f-110">请求标头</span><span class="sxs-lookup"><span data-stu-id="6325f-110">Request headers</span></span>
<a id="request-headers" class="xliff"></a>

| <span data-ttu-id="6325f-111">名称</span><span class="sxs-lookup"><span data-stu-id="6325f-111">Name</span></span>          | <span data-ttu-id="6325f-112">类型</span><span class="sxs-lookup"><span data-stu-id="6325f-112">Type</span></span>   | <span data-ttu-id="6325f-113">说明</span><span class="sxs-lookup"><span data-stu-id="6325f-113">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="6325f-114">if-match</span><span class="sxs-lookup"><span data-stu-id="6325f-114">if-match</span></span>      | <span data-ttu-id="6325f-115">String</span><span class="sxs-lookup"><span data-stu-id="6325f-115">String</span></span> | <span data-ttu-id="6325f-116">如果包含此请求标头，且提供的 eTag（或 cTag）与项中的当前标记不匹配，则返回 `412 Precondition Failed` 响应，并且不会删除该项。</span><span class="sxs-lookup"><span data-stu-id="6325f-116">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <span data-ttu-id="6325f-117">请求正文</span><span class="sxs-lookup"><span data-stu-id="6325f-117">Request body</span></span>
<a id="request-body" class="xliff"></a>
<span data-ttu-id="6325f-118">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6325f-118">Do not supply a request body for this method.</span></span>

## <span data-ttu-id="6325f-119">示例</span><span class="sxs-lookup"><span data-stu-id="6325f-119">Example</span></span>
<a id="example" class="xliff"></a>

<span data-ttu-id="6325f-120">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="6325f-120">Here is an example of how to call this API.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete-item"
}-->
```
DELETE https://graph.microsoft.com/v1.0/me/drive/items/{item-id}
```

## <span data-ttu-id="6325f-121">响应</span><span class="sxs-lookup"><span data-stu-id="6325f-121">Response</span></span>
<a id="response" class="xliff"></a>

<span data-ttu-id="6325f-122">如果成功，此调用将返回 `204 No Content` 响应，表示资源已被删除，没有可返回的内容。</span><span class="sxs-lookup"><span data-stu-id="6325f-122">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

<!-- { "blockType": "response" } -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete item",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Delete item"
}-->
