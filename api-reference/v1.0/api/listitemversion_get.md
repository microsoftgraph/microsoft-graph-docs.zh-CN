# <a name="get-a-listitemversion-resource"></a><span data-ttu-id="eb7a5-101">获取 ListItemVersion 资源</span><span class="sxs-lookup"><span data-stu-id="eb7a5-101">Get a ListItemVersion resource (preview)</span></span>

<span data-ttu-id="eb7a5-102">检索 [ListItem](../resources/listitem.md) 的某个特定版本的元数据。</span><span class="sxs-lookup"><span data-stu-id="eb7a5-102">Retrieve the metadata for a specific version of a [ListItem](../resources/listitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="eb7a5-103">权限</span><span class="sxs-lookup"><span data-stu-id="eb7a5-103">Permissions</span></span>

<span data-ttu-id="eb7a5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="eb7a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|            <span data-ttu-id="eb7a5-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="eb7a5-106">Permission type</span></span>             | <span data-ttu-id="eb7a5-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="eb7a5-107">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="eb7a5-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eb7a5-108">Delegated (work or school account)</span></span>     | <span data-ttu-id="eb7a5-109">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb7a5-109">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="eb7a5-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eb7a5-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb7a5-111">无</span><span class="sxs-lookup"><span data-stu-id="eb7a5-111">n/a</span></span>                                         |
| <span data-ttu-id="eb7a5-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="eb7a5-112">Application</span></span>                            | <span data-ttu-id="eb7a5-113">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb7a5-113">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="eb7a5-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eb7a5-114">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}
```


## <a name="response"></a><span data-ttu-id="eb7a5-115">响应</span><span class="sxs-lookup"><span data-stu-id="eb7a5-115">Response</span></span>

<span data-ttu-id="eb7a5-116">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [ListItemVersion](../resources/listitemversion.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="eb7a5-116">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/listitemversion.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="eb7a5-117">示例</span><span class="sxs-lookup"><span data-stu-id="eb7a5-117">Example</span></span>

<span data-ttu-id="eb7a5-118">本示例检索 listItem 的版本，并扩展字段集合以请求 listItem 中的字段值。</span><span class="sxs-lookup"><span data-stu-id="eb7a5-118">This example retrieves a version of a listItem and expands the fields collection to request the values of fields in the listItem.</span></span>

### <a name="http-request"></a><span data-ttu-id="eb7a5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eb7a5-119">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-single-version-listItem", "scopes": "files.read sites.read.all", "tags": "service.graph service.sharepoint" } -->

```http
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}?expand=fields
```

### <a name="response"></a><span data-ttu-id="eb7a5-120">响应</span><span class="sxs-lookup"><span data-stu-id="eb7a5-120">Response</span></span>

<span data-ttu-id="eb7a5-121">这将返回版本的集合：</span><span class="sxs-lookup"><span data-stu-id="eb7a5-121">This returns a collection of versions:</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItemVersion", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "1.0",
    "lastModifiedBy": {
    "user": {
        "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
        "displayName": "Ryan Gregg"
    }
    },
    "lastModifiedDateTime": "2017-09-14T12:34:53.912Z",
    "fields": {  }
}
```

<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history"
} -->
