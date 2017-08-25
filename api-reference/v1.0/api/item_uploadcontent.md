# <a name="upload-or-replace-the-contents-of-a-driveitem"></a><span data-ttu-id="aa361-101">上载或替换 driveItem 的内容</span><span class="sxs-lookup"><span data-stu-id="aa361-101">Upload or replace the contents of a driveItem</span></span>

<span data-ttu-id="aa361-p101">通过简单的上载 API，你可以在单个 API 调用中提供新文件的内容，也可以更新现有文件的内容。此方法仅支持最大大小为 4 MB 的文件。</span><span class="sxs-lookup"><span data-stu-id="aa361-p101">The simple upload API allows you to provide the contents of a new file or update the contents of an existing file in a single API call. This method only supports files up to 4MB in size.</span></span>

<span data-ttu-id="aa361-104">若要上传大文件，请参阅[通过上传会话上传大文件](item_createuploadsession.md)。</span><span class="sxs-lookup"><span data-stu-id="aa361-104">To upload large files see [Upload large files with an upload session](item_createuploadsession.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="aa361-105">权限</span><span class="sxs-lookup"><span data-stu-id="aa361-105">Permissions</span></span>
<span data-ttu-id="aa361-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="aa361-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="aa361-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="aa361-108">Permission type</span></span>      | <span data-ttu-id="aa361-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aa361-109">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="aa361-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aa361-110">Delegated (work or school account)</span></span> | <span data-ttu-id="aa361-111">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa361-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    | 
|<span data-ttu-id="aa361-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aa361-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa361-113">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa361-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    | 
|<span data-ttu-id="aa361-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="aa361-114">Application</span></span> | <span data-ttu-id="aa361-115">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa361-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="aa361-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aa361-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /me/drive/items/{parent-id}:/{filename}:/content
PUT /me/drive/root:/{parent-path}/{filename}:/content
PUT /me/drive/items/{parent-id}/children/{filename}/content
PUT /groups/{id}/drive/items/{parent-id}/children/{filename}/content
```

## <a name="request-body"></a><span data-ttu-id="aa361-117">请求正文</span><span class="sxs-lookup"><span data-stu-id="aa361-117">Request body</span></span>
<span data-ttu-id="aa361-118">请求正文的内容应该是要上载文件的二进制流。</span><span class="sxs-lookup"><span data-stu-id="aa361-118">The contents of the request body should be the binary stream of the file to be uploaded.</span></span>

## <a name="response"></a><span data-ttu-id="aa361-119">响应</span><span class="sxs-lookup"><span data-stu-id="aa361-119">Response</span></span>

<span data-ttu-id="aa361-120">如果成功，此方法在新建文件的响应正文中返回 [driveItem](../resources/driveitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="aa361-120">If successful, this method returns a [driveItem](../resources/driveitem.md) object in the response body for the newly created file.</span></span>

## <a name="example"></a><span data-ttu-id="aa361-121">示例</span><span class="sxs-lookup"><span data-stu-id="aa361-121">Example</span></span>
<span data-ttu-id="aa361-122">此示例通过已登录用户的 OneDrive 路径上载文件。</span><span class="sxs-lookup"><span data-stu-id="aa361-122">This example uploads a file by path to the signed-in user's OneDrive.</span></span>

<!-- {
  "blockType": "request",
  "name": "upload_item"
}-->
```http
PUT /me/drive/root:/{item-path}:/content
Content-type: text/plain

The contents of the file goes here.
```

##### <a name="response"></a><span data-ttu-id="aa361-123">响应</span><span class="sxs-lookup"><span data-stu-id="aa361-123">Response</span></span>

<span data-ttu-id="aa361-124">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="aa361-124">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
} -->
```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "0123456789abc",
  "name": "myfile.jpg",
  "size": 10191,
  "file": { }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Upload item",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
