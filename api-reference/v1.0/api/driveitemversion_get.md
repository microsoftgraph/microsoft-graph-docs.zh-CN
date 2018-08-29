# <a name="get-a-driveitemversion-resource"></a><span data-ttu-id="83f61-101">获取 DriveItemVersion 资源</span><span class="sxs-lookup"><span data-stu-id="83f61-101">Get a DriveItemVersion resource (preview)</span></span>

<span data-ttu-id="83f61-102">检索 [DriveItem](../resources/driveitem.md) 的某个特定版本的元数据。</span><span class="sxs-lookup"><span data-stu-id="83f61-102">Retrieve the metadata for a specific version of a [DriveItem](../resources/driveitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="83f61-103">权限</span><span class="sxs-lookup"><span data-stu-id="83f61-103">Permissions</span></span>

<span data-ttu-id="83f61-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="83f61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="83f61-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="83f61-106">Permission type</span></span>      | <span data-ttu-id="83f61-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="83f61-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="83f61-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="83f61-108">Delegated (work or school account)</span></span> | <span data-ttu-id="83f61-109">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83f61-109">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="83f61-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="83f61-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83f61-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83f61-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="83f61-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="83f61-112">Application</span></span> | <span data-ttu-id="83f61-113">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83f61-113">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="83f61-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="83f61-114">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions/{version-id}
GET /groups/{group-id}/drive/{item-id}/versions/{version-id}
GET /me/drive/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/drive/items/{item-id}/versions/{version-id}
GET /users/{user-id}/drive/items/{item-id}/versions/{version-id}
```

## <a name="response"></a><span data-ttu-id="83f61-115">响应</span><span class="sxs-lookup"><span data-stu-id="83f61-115">Response</span></span>

<span data-ttu-id="83f61-116">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [DriveItemVersion](../resources/driveitemversion.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="83f61-116">If successful, this method returns a `200 OK` response code and a [DriveItemVersion](../resources/driveitemversion.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="83f61-117">示例</span><span class="sxs-lookup"><span data-stu-id="83f61-117">Example</span></span>

<span data-ttu-id="83f61-118">本示例检索当前用户驱动器中的文件的版本。</span><span class="sxs-lookup"><span data-stu-id="83f61-118">This example retrieves a version of a file in the current user's drive.</span></span>

### <a name="http-request"></a><span data-ttu-id="83f61-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="83f61-119">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-single-version", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/versions/{version-id}
```

### <a name="response"></a><span data-ttu-id="83f61-120">响应</span><span class="sxs-lookup"><span data-stu-id="83f61-120">Response</span></span>

<span data-ttu-id="83f61-121">这将返回版本的集合：</span><span class="sxs-lookup"><span data-stu-id="83f61-121">This returns a collection of versions:</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItemVersion", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "D4990684-58CE-4FAB-9B87-D6C49E74F298",
    "lastModifiedBy": {
    "user": {
        "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
        "displayName": "Ryan Gregg"
    }
    },
    "lastModifiedDateTime": "2017-09-14T12:34:53.912Z",
    "size": 123
}
```

## <a name="remarks"></a><span data-ttu-id="83f61-122">注解</span><span class="sxs-lookup"><span data-stu-id="83f61-122">Remarks</span></span>

<span data-ttu-id="83f61-123">OneDrive 不保留文件以前版本的完整元数据。</span><span class="sxs-lookup"><span data-stu-id="83f61-123">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="83f61-124">当应用检索文件的可用版本列表时，将返回 [DriveItemVersion](../resources/driveItemVersion.md) 资源，它提供有关特定版本的可用信息。</span><span class="sxs-lookup"><span data-stu-id="83f61-124">When your app retrieves the list of available versions for a file, a [DriveItemVersion](../resources/driveItemVersion.md) resource is returned that provides the available information about the specific version.</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history"
} -->
