# <a name="delete-permission"></a><span data-ttu-id="9e3d7-101">删除权限</span><span class="sxs-lookup"><span data-stu-id="9e3d7-101">Delete permission</span></span>

<span data-ttu-id="9e3d7-102">删除 [DriveItem](../resources/driveitem.md) 访问权限。</span><span class="sxs-lookup"><span data-stu-id="9e3d7-102">Remove access to a [DriveItem](../resources/driveitem.md).</span></span>

<span data-ttu-id="9e3d7-p101">仅可删除非继承的权限。**InheritedFrom** 属性必须为 `null`。</span><span class="sxs-lookup"><span data-stu-id="9e3d7-p101">Only permissions that are not inherited can be deleted. The **inheritedFrom** property must be `null`.</span></span>

## <a name="permissions"></a><span data-ttu-id="9e3d7-105">权限</span><span class="sxs-lookup"><span data-stu-id="9e3d7-105">Permissions</span></span>
<span data-ttu-id="9e3d7-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="9e3d7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9e3d7-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9e3d7-108">Permission type</span></span>      | <span data-ttu-id="9e3d7-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9e3d7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9e3d7-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9e3d7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9e3d7-111">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e3d7-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="9e3d7-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9e3d7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e3d7-113">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e3d7-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="9e3d7-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="9e3d7-114">Application</span></span> | <span data-ttu-id="9e3d7-115">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e3d7-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9e3d7-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9e3d7-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /me/drive/items/{item-id}/permissions/{perm-id}
DELETE /me/drive/root:/{path}:/permissions/{perm-id}
DELETE /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
DELETE /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
```

## <a name="request-headers"></a><span data-ttu-id="9e3d7-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="9e3d7-117">Request headers</span></span>

| <span data-ttu-id="9e3d7-118">名称</span><span class="sxs-lookup"><span data-stu-id="9e3d7-118">Name</span></span>          | <span data-ttu-id="9e3d7-119">类型</span><span class="sxs-lookup"><span data-stu-id="9e3d7-119">Type</span></span>   | <span data-ttu-id="9e3d7-120">说明</span><span class="sxs-lookup"><span data-stu-id="9e3d7-120">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="9e3d7-121">if-match</span><span class="sxs-lookup"><span data-stu-id="9e3d7-121">if-match</span></span>      | <span data-ttu-id="9e3d7-122">string</span><span class="sxs-lookup"><span data-stu-id="9e3d7-122">string</span></span> | <span data-ttu-id="9e3d7-123">如果包含此请求标头，且提供的 eTag（或 cTag）与项中的当前标记不匹配，则返回 `412 Precondition Failed` 响应，并且不会删除该项。</span><span class="sxs-lookup"><span data-stu-id="9e3d7-123">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9e3d7-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="9e3d7-124">Request body</span></span>
<span data-ttu-id="9e3d7-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9e3d7-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e3d7-126">响应</span><span class="sxs-lookup"><span data-stu-id="9e3d7-126">Response</span></span>

<span data-ttu-id="9e3d7-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="9e3d7-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e3d7-129">示例</span><span class="sxs-lookup"><span data-stu-id="9e3d7-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9e3d7-130">请求</span><span class="sxs-lookup"><span data-stu-id="9e3d7-130">Request</span></span>

<span data-ttu-id="9e3d7-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9e3d7-131">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_permission"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/drive/root/items/{item-id}/permissions/{perm-id}
```

##### <a name="response"></a><span data-ttu-id="9e3d7-132">响应</span><span class="sxs-lookup"><span data-stu-id="9e3d7-132">Response</span></span>

<span data-ttu-id="9e3d7-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="9e3d7-133">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="remarks"></a><span data-ttu-id="9e3d7-134">注解</span><span class="sxs-lookup"><span data-stu-id="9e3d7-134">Remarks</span></span>

* <span data-ttu-id="9e3d7-135">具有 `personal`（OneDrive 个人版）**driveType** 的 [驱动器](../resources/drive.md) 无法创建或修改根 DriveItem 上的权限。</span><span class="sxs-lookup"><span data-stu-id="9e3d7-135">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive Personal) cannot create or modify permissions on the root DriveItem.</span></span> 

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete permission",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Delete permission"
}-->
