# <a name="move-a-driveitem"></a><span data-ttu-id="a314b-101">移动 DriveItem</span><span class="sxs-lookup"><span data-stu-id="a314b-101">Move a DriveItem</span></span>

<span data-ttu-id="a314b-p101">若要将 DriveItem 移动到新的父项，应用程序会请求更新要移动的 DriveItem 的 **parentReference**。这是[更新](item_update.md)方法的一种特殊情况。你的应用程序可以将以下操作组合到单个请求中：将项目移动到新的容器和更新项目的其他属性。</span><span class="sxs-lookup"><span data-stu-id="a314b-p101">To move a DriveItem to a new parent item, your app requests to update the **parentReference** of the DriveItem to move. This is a special case of the [Update](item_update.md) method. Your app can combine moving an item to a new container and updating other properties of the item into a single request.</span></span>

<span data-ttu-id="a314b-105">无法使用这一请求在[驱动器](../resources/drive.md)之间移动项目。</span><span class="sxs-lookup"><span data-stu-id="a314b-105">Items cannot be moved between [Drives](../resources/drive.md) using this request.</span></span>

## <a name="permissions"></a><span data-ttu-id="a314b-106">权限</span><span class="sxs-lookup"><span data-stu-id="a314b-106">Permissions</span></span>
<span data-ttu-id="a314b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a314b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a314b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a314b-109">Permission type</span></span>      | <span data-ttu-id="a314b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a314b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a314b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a314b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a314b-112">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a314b-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="a314b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a314b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a314b-114">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a314b-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="a314b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a314b-115">Application</span></span> | <span data-ttu-id="a314b-116">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a314b-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a314b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a314b-117">HTTP request</span></span>

```http
PATCH /me/drive/items/{item-id}
PATCH /me/drive/root:/{item-path}
PATCH /drives/{drive-id}/items/{item-id}
PATCH /groups/{group-id}/drive/{item-id}
```

## <a name="request-headers"></a><span data-ttu-id="a314b-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="a314b-118">Request headers</span></span>

| <span data-ttu-id="a314b-119">名称</span><span class="sxs-lookup"><span data-stu-id="a314b-119">Name</span></span>          | <span data-ttu-id="a314b-120">类型</span><span class="sxs-lookup"><span data-stu-id="a314b-120">Type</span></span>   | <span data-ttu-id="a314b-121">说明</span><span class="sxs-lookup"><span data-stu-id="a314b-121">Description</span></span>                                                                                                                                                         |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="a314b-122">if-match</span><span class="sxs-lookup"><span data-stu-id="a314b-122">if-match</span></span>      | <span data-ttu-id="a314b-123">String</span><span class="sxs-lookup"><span data-stu-id="a314b-123">String</span></span> | <span data-ttu-id="a314b-124">如果包含此请求标头，且提供的 eTag（或 cTag）与文件夹上的当前 eTag 不匹配，则返回 `412 Precondition Failed` 响应。</span><span class="sxs-lookup"><span data-stu-id="a314b-124">If this request header is included and the eTag (or cTag) provided does not match the current eTag on the folder, a `412 Precondition Failed` response is returned.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a314b-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="a314b-125">Request body</span></span>
<span data-ttu-id="a314b-p103">在请求正文中，提供 **parentReference** 属性的新值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="a314b-p103">In the request body, supply the new value for the **parentReference** property. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

<span data-ttu-id="a314b-p104">**注意：**将项目移动到 OneDrive 的根目录下时不能使用 `"id:" "root"` 语法。需要使用根文件夹的真实 ID，或对父引用使用 `{"path": "/drive/root"}`。</span><span class="sxs-lookup"><span data-stu-id="a314b-p104">**Note:** When moving items to the root of a OneDrive you cannot use the `"id:" "root"` syntax. You either need to use the real ID of the root folder, or use `{"path": "/drive/root"}` for the parent reference.</span></span>

## <a name="response"></a><span data-ttu-id="a314b-131">响应</span><span class="sxs-lookup"><span data-stu-id="a314b-131">Response</span></span>

<span data-ttu-id="a314b-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [DriveItem](../resources/driveitem.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="a314b-132">If successful, this method returns a `200 OK` response code and updated [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a314b-133">示例</span><span class="sxs-lookup"><span data-stu-id="a314b-133">Example</span></span>
<span data-ttu-id="a314b-134">本示例将 {item-id} 指定的项目移动到用户 OneDrive 的**文档**文件夹中。</span><span class="sxs-lookup"><span data-stu-id="a314b-134">This example moves an item specified by {item-id} into the **Documents** folder in the user's OneDrive.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_item"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{item-id}
Content-type: application/json

{
    "name": "new-item-name",
    "parentReference" : {"path": "/drive/root:/Documents"}
}
```

##### <a name="response"></a><span data-ttu-id="a314b-135">响应</span><span class="sxs-lookup"><span data-stu-id="a314b-135">Response</span></span>

<span data-ttu-id="a314b-136">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="a314b-136">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "0123456789abc",
    "name": "new-item-name",
    "folder": { "childCount": 3 },
  "parentReference": {
    "id": "507DE6D5-0201-496A-AA87-5E2563247982",
    "path": "/drive/root:/Documents"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Move item",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
