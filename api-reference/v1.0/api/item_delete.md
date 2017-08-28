# <a name="delete-a-driveitem"></a><span data-ttu-id="ab286-101">删除 DriveItem</span><span class="sxs-lookup"><span data-stu-id="ab286-101">Delete a DriveItem</span></span>

<span data-ttu-id="ab286-p101">通过使用其 ID 或路径删除 [DriveItem](../resources/driveitem.md)。注意，使用此方法删除项将把项移动到回收站中，而不是永久删除该项。</span><span class="sxs-lookup"><span data-stu-id="ab286-p101">Delete a [DriveItem](../resources/driveitem.md) by using its ID or path. Note that deleting items using this method will move the items to the recycle bin instead of permanently deleting the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="ab286-104">权限</span><span class="sxs-lookup"><span data-stu-id="ab286-104">Permissions</span></span>
<span data-ttu-id="ab286-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="ab286-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ab286-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="ab286-107">Permission type</span></span>      | <span data-ttu-id="ab286-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ab286-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab286-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ab286-109">Delegated (work or school account)</span></span> | <span data-ttu-id="ab286-110">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab286-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="ab286-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ab286-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab286-112">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab286-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="ab286-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="ab286-113">Application</span></span> | <span data-ttu-id="ab286-114">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab286-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab286-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ab286-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```
DELETE /me/drive/items/{item-id}
DELETE /me/drive/root:/{item-path}
DELETE /drives/{drive-id}/items/{item-id}
DELETE /groups/{group-id}/drive/items/{item-id}
```

## <a name="request-headers"></a><span data-ttu-id="ab286-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="ab286-116">Request headers</span></span>

| <span data-ttu-id="ab286-117">名称</span><span class="sxs-lookup"><span data-stu-id="ab286-117">Name</span></span>          | <span data-ttu-id="ab286-118">类型</span><span class="sxs-lookup"><span data-stu-id="ab286-118">Type</span></span>   | <span data-ttu-id="ab286-119">说明</span><span class="sxs-lookup"><span data-stu-id="ab286-119">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="ab286-120">if-match</span><span class="sxs-lookup"><span data-stu-id="ab286-120">if-match</span></span>      | <span data-ttu-id="ab286-121">String</span><span class="sxs-lookup"><span data-stu-id="ab286-121">String</span></span> | <span data-ttu-id="ab286-122">如果包含此请求标头，且提供的 eTag（或 cTag）与项中的当前标记不匹配，则返回 `412 Precondition Failed` 响应，并且不会删除该项。</span><span class="sxs-lookup"><span data-stu-id="ab286-122">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ab286-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="ab286-123">Request body</span></span>
<span data-ttu-id="ab286-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ab286-124">Do not supply a request body for this method.</span></span>

## <a name="example"></a><span data-ttu-id="ab286-125">示例</span><span class="sxs-lookup"><span data-stu-id="ab286-125">Example</span></span>

<span data-ttu-id="ab286-126">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="ab286-126">Here is an example of how to call this API.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete-item"
}-->
```
DELETE https://graph.microsoft.com/v1.0/me/drive/items/{item-id}
```

## <a name="response"></a><span data-ttu-id="ab286-127">响应</span><span class="sxs-lookup"><span data-stu-id="ab286-127">Response</span></span>

<span data-ttu-id="ab286-128">如果成功，此调用将返回 `204 No Content` 响应，表示资源已被删除，没有可返回的内容。</span><span class="sxs-lookup"><span data-stu-id="ab286-128">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

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
