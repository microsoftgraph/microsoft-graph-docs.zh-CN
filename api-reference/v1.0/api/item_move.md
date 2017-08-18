# <a name="move-a-driveitem"></a><span data-ttu-id="1fce3-101">移动 DriveItem</span><span class="sxs-lookup"><span data-stu-id="1fce3-101">Move a DriveItem</span></span>

<span data-ttu-id="1fce3-p101">若要将 DriveItem 移动到新的父项，应用程序会请求更新要移动的 DriveItem 的 **parentReference**。这是[更新](item_update.md)方法的一种特殊情况。你的应用程序可以将以下操作组合到单个请求中：将项目移动到新的容器和更新项目的其他属性。</span><span class="sxs-lookup"><span data-stu-id="1fce3-p101">To move a DriveItem to a new parent item, your app requests to update the **parentReference** of the DriveItem to move. This is a special case of the [Update](item_update.md) method. Your app can combine moving an item to a new container and updating other properties of the item into a single request.</span></span>

<span data-ttu-id="1fce3-105">无法使用这一请求在 [驱动器](../resources/drive.md) 之间移动项目。</span><span class="sxs-lookup"><span data-stu-id="1fce3-105">Items cannot be moved between [Drives](../resources/drive.md) using this request.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1fce3-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="1fce3-106">Prerequisites</span></span>
<span data-ttu-id="1fce3-107">要执行此 API，需要以下**范围**之一：</span><span class="sxs-lookup"><span data-stu-id="1fce3-107">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="1fce3-108">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1fce3-108">Files.ReadWrite</span></span>
* <span data-ttu-id="1fce3-109">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fce3-109">Files.ReadWrite.All</span></span>
* <span data-ttu-id="1fce3-110">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fce3-110">Sites.ReadWrite.All</span></span>


## <a name="http-request"></a><span data-ttu-id="1fce3-111">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1fce3-111">HTTP request</span></span>

```http
PATCH /me/drive/items/{item-id}
PATCH /me/drive/root:/{item-path}
PATCH /drives/{drive-id}/items/{item-id}
PATCH /groups/{group-id}/drive/{item-id}
```

## <a name="request-headers"></a><span data-ttu-id="1fce3-112">请求标头</span><span class="sxs-lookup"><span data-stu-id="1fce3-112">Request headers</span></span>

| <span data-ttu-id="1fce3-113">名称</span><span class="sxs-lookup"><span data-stu-id="1fce3-113">Name</span></span>          | <span data-ttu-id="1fce3-114">类型</span><span class="sxs-lookup"><span data-stu-id="1fce3-114">Type</span></span>   | <span data-ttu-id="1fce3-115">说明</span><span class="sxs-lookup"><span data-stu-id="1fce3-115">Description</span></span>                                                                                                                                                         |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="1fce3-116">if-match</span><span class="sxs-lookup"><span data-stu-id="1fce3-116">if-match</span></span>      | <span data-ttu-id="1fce3-117">String</span><span class="sxs-lookup"><span data-stu-id="1fce3-117">String</span></span> | <span data-ttu-id="1fce3-118">如果包含此请求标头，且提供的 eTag（或 cTag）与文件夹上的当前 eTag 不匹配，则返回 `412 Precondition Failed` 响应。</span><span class="sxs-lookup"><span data-stu-id="1fce3-118">If this request header is included and the eTag (or cTag) provided does not match the current eTag on the folder, a `412 Precondition Failed` response is returned.</span></span> |


## <a name="request-body"></a><span data-ttu-id="1fce3-119">请求正文</span><span class="sxs-lookup"><span data-stu-id="1fce3-119">Request body</span></span>
<span data-ttu-id="1fce3-p102">在请求正文中，提供 **parentReference** 属性的新值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="1fce3-p102">In the request body, supply the new value for the **parentReference** property. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

<span data-ttu-id="1fce3-p103">**注意：**将项目移动到 OneDrive 的根目录下时不能使用 `"id:" "root"` 语法。需要使用根文件夹的真实 ID，或对父引用使用 `{"path": "/drive/root"}`。</span><span class="sxs-lookup"><span data-stu-id="1fce3-p103">**Note:** When moving items to the root of a OneDrive you cannot use the `"id:" "root"` syntax. You either need to use the real ID of the root folder, or use `{"path": "/drive/root"}` for the parent reference.</span></span>

## <a name="response"></a><span data-ttu-id="1fce3-125">响应</span><span class="sxs-lookup"><span data-stu-id="1fce3-125">Response</span></span>

<span data-ttu-id="1fce3-126">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [DriveItem](../resources/driveitem.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="1fce3-126">If successful, this method returns a `200 OK` response code and updated [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1fce3-127">示例</span><span class="sxs-lookup"><span data-stu-id="1fce3-127">Example</span></span>
<span data-ttu-id="1fce3-128">本示例将 {item-id} 指定的项目移动到用户 OneDrive 的**文档**文件夹中。</span><span class="sxs-lookup"><span data-stu-id="1fce3-128">This example moves an item specified by {item-id} into the **Documents** folder in the user's OneDrive.</span></span>

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

##### <a name="response"></a><span data-ttu-id="1fce3-129">响应</span><span class="sxs-lookup"><span data-stu-id="1fce3-129">Response</span></span>

<span data-ttu-id="1fce3-130">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="1fce3-130">The following example shows the response.</span></span>

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
