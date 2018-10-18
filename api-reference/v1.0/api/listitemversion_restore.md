# <a name="restore-a-previous-version-of-a-listitem"></a><span data-ttu-id="2c534-101">还原 ListItem 的以前版本</span><span class="sxs-lookup"><span data-stu-id="2c534-101">Restore a previous version of a ListItem</span></span>

<span data-ttu-id="2c534-102">将 ListItem 的以前版本还原为当前版本。</span><span class="sxs-lookup"><span data-stu-id="2c534-102">Restore a previous version of a ListItem to be the current version.</span></span> <span data-ttu-id="2c534-103">这将使用以前版本的内容创建一个新版本，但保留项的所有现有版本。</span><span class="sxs-lookup"><span data-stu-id="2c534-103">This will create a new version with the contents of the previous version, but preserves all existing versions of the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="2c534-104">权限</span><span class="sxs-lookup"><span data-stu-id="2c534-104">Permissions</span></span>

<span data-ttu-id="2c534-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="2c534-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|            <span data-ttu-id="2c534-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="2c534-107">Permission type</span></span>             |         <span data-ttu-id="2c534-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2c534-108">Permissions (from least to most privileged)</span></span>          |
| :------------------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="2c534-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2c534-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="2c534-110">Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="2c534-110">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |
| <span data-ttu-id="2c534-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2c534-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c534-112">无</span><span class="sxs-lookup"><span data-stu-id="2c534-112">n/a</span></span>                                                          |
| <span data-ttu-id="2c534-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="2c534-113">Application</span></span>                            | <span data-ttu-id="2c534-114">Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="2c534-114">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2c534-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2c534-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="2c534-116">请求正文</span><span class="sxs-lookup"><span data-stu-id="2c534-116">Request body</span></span>

<span data-ttu-id="2c534-117">无需请求正文。</span><span class="sxs-lookup"><span data-stu-id="2c534-117">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="2c534-118">示例</span><span class="sxs-lookup"><span data-stu-id="2c534-118">Example</span></span>

<span data-ttu-id="2c534-119">本示例还原由 `{item-id}` 和 `{version-id}` 标识的 listItem 的一个版本。</span><span class="sxs-lookup"><span data-stu-id="2c534-119">This example restores a version of a listItem identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version-listItem", "scopes": "files.readwrite sites.readwrite.all", "target": "action", "tags": "service.graph service.sharepoint" } -->

```http
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="2c534-120">响应</span><span class="sxs-lookup"><span data-stu-id="2c534-120">Response</span></span>

<span data-ttu-id="2c534-121">如果成功，该 API 调用会返回 `204 No Content`。</span><span class="sxs-lookup"><span data-stu-id="2c534-121">If successful, the API call returns a `204 No Content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy"
} -->
