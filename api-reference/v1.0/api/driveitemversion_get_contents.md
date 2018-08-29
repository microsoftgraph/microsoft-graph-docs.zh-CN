# <a name="download-contents-of-a-driveitemversion-resource"></a><span data-ttu-id="63faa-101">下载 DriveItemVersion 资源的内容</span><span class="sxs-lookup"><span data-stu-id="63faa-101">Download contents of a DriveItemVersion resource (preview)</span></span>

<span data-ttu-id="63faa-102">检索某个特定版本的 [DriveItem](../resources/driveitem.md) 的内容。</span><span class="sxs-lookup"><span data-stu-id="63faa-102">Retrieve the contents of a specific version of a [DriveItem](../resources/driveitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="63faa-103">权限</span><span class="sxs-lookup"><span data-stu-id="63faa-103">Permissions</span></span>

<span data-ttu-id="63faa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="63faa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="63faa-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="63faa-106">Permission type</span></span>      | <span data-ttu-id="63faa-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="63faa-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="63faa-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="63faa-108">Delegated (work or school account)</span></span> | <span data-ttu-id="63faa-109">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63faa-109">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="63faa-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="63faa-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63faa-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63faa-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="63faa-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="63faa-112">Application</span></span> | <span data-ttu-id="63faa-113">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63faa-113">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="63faa-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="63faa-114">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions/{version-id}/content
GET /groups/{group-id}/drive/{item-id}/versions/{version-id}/content
GET /me/drive/items/{item-id}/versions/{version-id}/content
GET /sites/{site-id}/drive/items/{item-id}/versions/{version-id}/content
GET /users/{user-id}/drive/items/{item-id}/versions/{version-id}/content
```

## <a name="response"></a><span data-ttu-id="63faa-115">响应</span><span class="sxs-lookup"><span data-stu-id="63faa-115">Response</span></span>

<span data-ttu-id="63faa-116">返回 `302 Found` 响应，重定向到文件字节已预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="63faa-116">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the bytes of the file.</span></span>

<span data-ttu-id="63faa-p102">若要下载该文件的内容，应用程序将需要遵循响应中的 `Location` 标头。许多 HTTP 客户端库将自动遵循 302 重定向并立即开始下载文件。</span><span class="sxs-lookup"><span data-stu-id="63faa-p102">To download the contents of the file your application will need to follow the `Location` header in the response. Many HTTP client libraries will automatically follow the 302 redirection and start downloading the file immedately.</span></span>

<span data-ttu-id="63faa-119">预先验证的下载 URL 仅在较短的一段时间 （几分钟后）内有效，不需要 `Authorization` 标头即可下载。</span><span class="sxs-lookup"><span data-stu-id="63faa-119">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

## <a name="example"></a><span data-ttu-id="63faa-120">示例</span><span class="sxs-lookup"><span data-stu-id="63faa-120">Example</span></span>

<span data-ttu-id="63faa-121">本示例检索当前用户驱动器中的文件的版本。</span><span class="sxs-lookup"><span data-stu-id="63faa-121">This example retrieves a version of a file in the current user's drive.</span></span>

### <a name="http-request"></a><span data-ttu-id="63faa-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="63faa-122">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-version-contents", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/versions/{version-id}/content
```

### <a name="response"></a><span data-ttu-id="63faa-123">响应</span><span class="sxs-lookup"><span data-stu-id="63faa-123">Response</span></span>

<span data-ttu-id="63faa-124">会返回一个重定向链接，可以在其中下载版本的内容。</span><span class="sxs-lookup"><span data-stu-id="63faa-124">This returns a redirect to where the contents of the version can be downloaded.</span></span>

<!-- { "blockType": "response", "isEmpty": true  } -->

```http
HTTP/1.1 302 Found
Location: https://onedrive.com/34FF49D6...
```


## <a name="remarks"></a><span data-ttu-id="63faa-125">注解</span><span class="sxs-lookup"><span data-stu-id="63faa-125">Remarks</span></span>

<span data-ttu-id="63faa-126">OneDrive 不保留文件以前版本的完整元数据。</span><span class="sxs-lookup"><span data-stu-id="63faa-126">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="63faa-127">当应用检索文件的可用版本列表时，将返回 [DriveItemVersion](../resources/driveItemVersion.md) 资源，它提供有关特定版本的可用信息。</span><span class="sxs-lookup"><span data-stu-id="63faa-127">When your app retrieves the list of available versions for a file, a [DriveItemVersion](../resources/driveItemVersion.md) resource is returned that provides the available information about the specific version.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history"
} -->
