# <a name="copy-a-driveitem"></a><span data-ttu-id="4c84f-101">复制 DriveItem</span><span class="sxs-lookup"><span data-stu-id="4c84f-101">Copy a DriveItem</span></span>

<span data-ttu-id="4c84f-102">在新父级下或使用新名称创建一个 [driveItem](../resources/driveitem.md) 副本（包括任何子级）。</span><span class="sxs-lookup"><span data-stu-id="4c84f-102">Creates a copy of a [driveItem](../resources/driveitem.md) (including any children) under a new parent or with a new name.</span></span>

## <a name="permissions"></a><span data-ttu-id="4c84f-103">权限</span><span class="sxs-lookup"><span data-stu-id="4c84f-103">Permissions</span></span>
<span data-ttu-id="4c84f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="4c84f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4c84f-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="4c84f-106">Permission type</span></span>      | <span data-ttu-id="4c84f-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4c84f-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="4c84f-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4c84f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="4c84f-109">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c84f-109">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    | 
|<span data-ttu-id="4c84f-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4c84f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c84f-111">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c84f-111">Files.ReadWrite, Files.ReadWrite.All</span></span>    | 
|<span data-ttu-id="4c84f-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="4c84f-112">Application</span></span> | <span data-ttu-id="4c84f-113">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c84f-113">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="4c84f-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4c84f-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```
POST /me/drive/items/{item-id}/copy
POST /me/drive/root:/{path}:/copy
POST /groups/{group-id}/drive/items/{item-id}/copy
```

## <a name="request-body"></a><span data-ttu-id="4c84f-115">请求正文</span><span class="sxs-lookup"><span data-stu-id="4c84f-115">Request body</span></span>
<span data-ttu-id="4c84f-116">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="4c84f-116">In the request body, provide a JSON object with the following parameters.</span></span>


| <span data-ttu-id="4c84f-117">名称</span><span class="sxs-lookup"><span data-stu-id="4c84f-117">Name</span></span>            | <span data-ttu-id="4c84f-118">值</span><span class="sxs-lookup"><span data-stu-id="4c84f-118">Value</span></span>                                          | <span data-ttu-id="4c84f-119">说明</span><span class="sxs-lookup"><span data-stu-id="4c84f-119">Description</span></span>                                                                                                 |
|:----------------|:-----------------------------------------------|:------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="4c84f-120">parentReference</span><span class="sxs-lookup"><span data-stu-id="4c84f-120">parentReference</span></span> | [<span data-ttu-id="4c84f-121">ItemReference</span><span class="sxs-lookup"><span data-stu-id="4c84f-121">ItemReference</span></span>](../resources/itemreference.md) | <span data-ttu-id="4c84f-p102">可选。引用在其中创建副本的父项。</span><span class="sxs-lookup"><span data-stu-id="4c84f-p102">Optional. Reference to the parent item the copy will be created in.</span></span>                                         |
| <span data-ttu-id="4c84f-124">name</span><span class="sxs-lookup"><span data-stu-id="4c84f-124">name</span></span>            | <span data-ttu-id="4c84f-125">string</span><span class="sxs-lookup"><span data-stu-id="4c84f-125">string</span></span>                                         | <span data-ttu-id="4c84f-p103">可选。副本的新名称。如果没有新名称，将与原始版本同名。</span><span class="sxs-lookup"><span data-stu-id="4c84f-p103">Optional. The new name for the copy. If this isn't provided, the same name will be used as the original.</span></span>    |

<span data-ttu-id="4c84f-p104">**注意：**_ParentReference_ 应包括 `id` 或 `path`，但不能同时包括两者。如果这两项都包括在内，它们需要引用相同的项，否则将发生错误。</span><span class="sxs-lookup"><span data-stu-id="4c84f-p104">**Note:** The _parentReference_ should include either an `id` or `path` but not both. If both are included, they need to reference the same item or an error will occur.</span></span>

## <a name="example"></a><span data-ttu-id="4c84f-131">示例</span><span class="sxs-lookup"><span data-stu-id="4c84f-131">Example</span></span>

<!-- { "blockType": "request", "name": "copy-item", "scopes": "files.readwrite" } -->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/copy
Content-Type: application/json

{
  "parentReference": {
    "path": "/drive/root:/Documents"
  },
  "name": "contoso plan.docx"
}
```

## <a name="response"></a><span data-ttu-id="4c84f-132">响应</span><span class="sxs-lookup"><span data-stu-id="4c84f-132">Response</span></span>

<span data-ttu-id="4c84f-133">返回有关如何在接受请求时监控复制进度的详细信息。</span><span class="sxs-lookup"><span data-stu-id="4c84f-133">Returns details about how to monitor the progress of the copy, upon accepting the request.</span></span>

<!-- { "blockType": "response" } -->
```http
HTTP/1.1 202 Accepted
```

## <a name="remarks"></a><span data-ttu-id="4c84f-134">注解</span><span class="sxs-lookup"><span data-stu-id="4c84f-134">Remarks</span></span>

<span data-ttu-id="4c84f-p105">在许多情况下，复制操作采用异步执行。API 响应仅指明复制操作获得接受还是遭到拒绝（比如说，由于目标文件名已被其他对象使用而遭到拒绝）。</span><span class="sxs-lookup"><span data-stu-id="4c84f-p105">In many cases the copy action is performed asynchronously. The response from the API will only indicate that the copy operation was accepted or rejected, say due to the destination filename already being in use.</span></span>

<span data-ttu-id="4c84f-137">**注意：**API 未提供用于确认复制是否成功的方法。</span><span class="sxs-lookup"><span data-stu-id="4c84f-137">**Note:** The API does not provide a method to know if the copy was successful.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Copy"
} -->
