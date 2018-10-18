# <a name="restore-a-previous-version-of-a-driveitem"></a><span data-ttu-id="a4db0-101">还原 DriveItem 的以前版本</span><span class="sxs-lookup"><span data-stu-id="a4db0-101">Restore a previous version of a DriveItem</span></span>

<span data-ttu-id="a4db0-102">将 DriveItem 的以前版本还原为当前版本。</span><span class="sxs-lookup"><span data-stu-id="a4db0-102">Restore a previous version of a DriveItem to be the current version.</span></span> <span data-ttu-id="a4db0-103">这将使用以前版本的内容创建一个新版本，但保留该文件的所有现有版本。</span><span class="sxs-lookup"><span data-stu-id="a4db0-103">This will create a new version with the contents of the previous version, but preserves all existing versions of the file.</span></span>

## <a name="permissions"></a><span data-ttu-id="a4db0-104">权限</span><span class="sxs-lookup"><span data-stu-id="a4db0-104">Permissions</span></span>

<span data-ttu-id="a4db0-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a4db0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a4db0-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="a4db0-107">Permission type</span></span>      | <span data-ttu-id="a4db0-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a4db0-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a4db0-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a4db0-109">Delegated (work or school account)</span></span> | <span data-ttu-id="a4db0-110">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4db0-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="a4db0-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a4db0-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4db0-112">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4db0-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="a4db0-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="a4db0-113">Application</span></span> | <span data-ttu-id="a4db0-114">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4db0-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a4db0-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a4db0-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/versions/{version-id}/restoreVersion
POST /groups/{groupId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /me/drive/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{siteId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /users/{userId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="a4db0-116">请求正文</span><span class="sxs-lookup"><span data-stu-id="a4db0-116">Request body</span></span>

<span data-ttu-id="a4db0-117">无需请求正文。</span><span class="sxs-lookup"><span data-stu-id="a4db0-117">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="a4db0-118">示例</span><span class="sxs-lookup"><span data-stu-id="a4db0-118">Example</span></span>

<span data-ttu-id="a4db0-119">本示例还原由 `{item-id}` 和 `{version-id}` 标识的文件的一个版本。</span><span class="sxs-lookup"><span data-stu-id="a4db0-119">This example restores a version of a file identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="a4db0-120">响应</span><span class="sxs-lookup"><span data-stu-id="a4db0-120">Response</span></span>

<span data-ttu-id="a4db0-121">如果成功，该 API 调用会返回 `204 No Content`。</span><span class="sxs-lookup"><span data-stu-id="a4db0-121">If successful, the API call returns a `204 No Content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy"
} -->
