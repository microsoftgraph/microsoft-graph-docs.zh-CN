<span data-ttu-id="a4f39-p101">通过简单的上载 API，你可以在单个 API 调用中提供新文件的内容，也可以更新现有文件的内容。此方法仅支持最大大小为 4 MB 的文件。</span><span class="sxs-lookup"><span data-stu-id="a4f39-p101">The simple upload API allows you to provide the contents of a new file or update the contents of an existing file in a single API call. This method only supports files up to 4MB in size.</span></span>

通过简单的上载 API，你可以在单个 API 调用中提供新文件的内容，也可以更新现有文件的内容。此方法仅支持最大大小为 4 MB 的文件。

<span data-ttu-id="a4f39-104">若要上载大文件，请参阅 [通过上载会话上载大文件](item_createuploadsession.md)。</span><span class="sxs-lookup"><span data-stu-id="a4f39-104">To upload large files see [Upload large files with an upload session](item_createuploadsession.md).</span></span>

## <span data-ttu-id="a4f39-105">先决条件</span><span class="sxs-lookup"><span data-stu-id="a4f39-105">Prerequisites</span></span>
<a id="prerequisites" class="xliff"></a>
<span data-ttu-id="a4f39-106">要执行此 API，需要以下**范围**之一：</span><span class="sxs-lookup"><span data-stu-id="a4f39-106">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="a4f39-107">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a4f39-107">Files.ReadWrite</span></span>
* <span data-ttu-id="a4f39-108">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4f39-108">Files.ReadWrite.All</span></span>
* <span data-ttu-id="a4f39-109">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4f39-109">Sites.ReadWrite.All</span></span>


## <span data-ttu-id="a4f39-110">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a4f39-110">HTTP request</span></span>
<a id="http-request" class="xliff"></a>
<!-- { "blockType": "ignored" } -->
```http
PUT /me/drive/items/{parent-id}:/{filename}:/content
PUT /me/drive/root:/{parent-path}/{filename}:/content
PUT /me/drive/items/{parent-id}/children/{filename}/content
PUT /groups/{id}/drive/items/{parent-id}/children/{filename}/content
```

## <span data-ttu-id="a4f39-111">请求正文</span><span class="sxs-lookup"><span data-stu-id="a4f39-111">Request body</span></span>
<a id="request-body" class="xliff"></a>
<span data-ttu-id="a4f39-112">请求正文的内容应该是要上载文件的二进制流。</span><span class="sxs-lookup"><span data-stu-id="a4f39-112">The contents of the request body should be the binary stream of the file to be uploaded.</span></span>

## <span data-ttu-id="a4f39-113">响应</span><span class="sxs-lookup"><span data-stu-id="a4f39-113">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="a4f39-114">如果成功，此方法在新建文件的响应正文中返回 [driveItem](../resources/driveitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a4f39-114">If successful, this method returns a [driveItem](../resources/driveitem.md) object in the response body for the newly created file.</span></span>

## <span data-ttu-id="a4f39-115">示例</span><span class="sxs-lookup"><span data-stu-id="a4f39-115">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="a4f39-116">此示例通过已登录用户的 OneDrive 路径上载文件。</span><span class="sxs-lookup"><span data-stu-id="a4f39-116">This example uploads a file by path to the signed-in user's OneDrive.</span></span>

<!-- {
  "blockType": "request",
  "name": "upload_item"
}-->
```http
PUT /me/drive/root:/{item-path}:/content
Content-type: text/plain

The contents of the file goes here.
```

## <span data-ttu-id="a4f39-117">响应</span><span class="sxs-lookup"><span data-stu-id="a4f39-117">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="a4f39-118">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a4f39-118">Here is an example of the response.</span></span>
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
