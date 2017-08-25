# <a name="update-driveitem-properties"></a><span data-ttu-id="b87d5-101">更新 DriveItem 属性</span><span class="sxs-lookup"><span data-stu-id="b87d5-101">Update DriveItem properties</span></span>

<span data-ttu-id="b87d5-102">按 ID 或路径更新 [DriveItem](../resources/driveitem.md) 元数据。</span><span class="sxs-lookup"><span data-stu-id="b87d5-102">Update the metadata for a [DriveItem](../resources/driveitem.md) by ID or path.</span></span>

<span data-ttu-id="b87d5-103">还可以通过更新项的 **parentReference** 属性，使用更新将[项移动到](item_move.md)其他父级。</span><span class="sxs-lookup"><span data-stu-id="b87d5-103">You can also use update to [move an item](item_move.md) to another parent by updating the item's **parentReference** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="b87d5-104">权限</span><span class="sxs-lookup"><span data-stu-id="b87d5-104">Permissions</span></span>
<span data-ttu-id="b87d5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="b87d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b87d5-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="b87d5-107">Permission type</span></span>      | <span data-ttu-id="b87d5-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b87d5-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="b87d5-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b87d5-109">Delegated (work or school account)</span></span> | <span data-ttu-id="b87d5-110">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b87d5-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    | 
|<span data-ttu-id="b87d5-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b87d5-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b87d5-112">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b87d5-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    | 
|<span data-ttu-id="b87d5-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="b87d5-113">Application</span></span> | <span data-ttu-id="b87d5-114">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b87d5-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b87d5-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b87d5-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{item-id}
PATCH /me/drive/root:/{item-path}
PATCH /drives/{drive-id}/items/{item-id}
PATCH /groups/{group-id}/drive/items/{item-id}
```

## <a name="request-headers"></a><span data-ttu-id="b87d5-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="b87d5-116">Request headers</span></span>

| <span data-ttu-id="b87d5-117">名称</span><span class="sxs-lookup"><span data-stu-id="b87d5-117">Name</span></span>          | <span data-ttu-id="b87d5-118">类型</span><span class="sxs-lookup"><span data-stu-id="b87d5-118">Type</span></span>   | <span data-ttu-id="b87d5-119">说明</span><span class="sxs-lookup"><span data-stu-id="b87d5-119">Description</span></span>                                                                                                                                                         |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="b87d5-120">if-match</span><span class="sxs-lookup"><span data-stu-id="b87d5-120">if-match</span></span>      | <span data-ttu-id="b87d5-121">String</span><span class="sxs-lookup"><span data-stu-id="b87d5-121">String</span></span> | <span data-ttu-id="b87d5-122">如果包含此请求标头，且提供的 eTag（或 cTag）与文件夹上的当前 eTag 不匹配，则返回 `412 Precondition Failed` 响应。</span><span class="sxs-lookup"><span data-stu-id="b87d5-122">If this request header is included and the eTag (or cTag) provided does not match the current eTag on the folder, a `412 Precondition Failed` response is returned.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b87d5-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="b87d5-123">Request body</span></span>
<span data-ttu-id="b87d5-p102">在请求正文中，提供应更新的属性的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，应用不应包括尚未更改的属性。</span><span class="sxs-lookup"><span data-stu-id="b87d5-p102">In the request body, supply the values for properties that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance your app should not include properties that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="b87d5-127">响应</span><span class="sxs-lookup"><span data-stu-id="b87d5-127">Response</span></span>

<span data-ttu-id="b87d5-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [DriveItem](../resources/driveitem.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="b87d5-128">If successful, this method returns a `200 OK` response code and updated [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b87d5-129">示例</span><span class="sxs-lookup"><span data-stu-id="b87d5-129">Example</span></span>
<span data-ttu-id="b87d5-130">此示例重命名 driveItem。</span><span class="sxs-lookup"><span data-stu-id="b87d5-130">This example renames the driveItem.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_item"
}-->
```http
PATCH /me/drive/items/{item-id}
Content-type: application/json

{
    "name": "new-file-name.docx"
}
```

##### <a name="response"></a><span data-ttu-id="b87d5-131">响应</span><span class="sxs-lookup"><span data-stu-id="b87d5-131">Response</span></span>

<span data-ttu-id="b87d5-p103">以下示例显示了相应的响应。为提高可读性，此响应被截断。</span><span class="sxs-lookup"><span data-stu-id="b87d5-p103">The following example shows the response. This response is truncated for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "01NKDM7HMOJTVYMDOSXFDK2QJDXCDI3WUK",
    "name": "new-file-name.docx",
    "file": { }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update item",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Update item"
}-->
