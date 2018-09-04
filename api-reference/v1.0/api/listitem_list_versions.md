# <a name="listing-versions-of-a-listitem"></a><span data-ttu-id="fc46a-101">列出 ListItem 的版本</span><span class="sxs-lookup"><span data-stu-id="fc46a-101">Listing versions of a ListItem (preview)</span></span>

<span data-ttu-id="fc46a-102">SharePoint 可以配置为保留列表项的历史记录。</span><span class="sxs-lookup"><span data-stu-id="fc46a-102">SharePoint can be configured to retain the history for list items.</span></span>

<span data-ttu-id="fc46a-103">以前版本可能会保留有限的一段时间，具体取决于管理员设置，这对于每个用户或位置可能是唯一的。</span><span class="sxs-lookup"><span data-stu-id="fc46a-103">Previous versions may be retained for a finite period of time depending on admin settings which may be unique per user or location.</span></span>

## <a name="permissions"></a><span data-ttu-id="fc46a-104">权限</span><span class="sxs-lookup"><span data-stu-id="fc46a-104">Permissions</span></span>

<span data-ttu-id="fc46a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="fc46a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|            <span data-ttu-id="fc46a-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="fc46a-107">Permission type</span></span>             | <span data-ttu-id="fc46a-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fc46a-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="fc46a-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fc46a-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="fc46a-110">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc46a-110">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="fc46a-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fc46a-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc46a-112">无</span><span class="sxs-lookup"><span data-stu-id="fc46a-112">n/a</span></span>                                         |
| <span data-ttu-id="fc46a-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="fc46a-113">Application</span></span>                            | <span data-ttu-id="fc46a-114">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc46a-114">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="fc46a-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fc46a-115">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions
```

## <a name="response"></a><span data-ttu-id="fc46a-116">响应</span><span class="sxs-lookup"><span data-stu-id="fc46a-116">Response</span></span>

<span data-ttu-id="fc46a-117">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [ListItemVersion](../resources/listitemversion.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="fc46a-117">If successful, this method returns a `200 OK` response code and collection of [ListItemVersion](../resources/listitemversion.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="fc46a-118">示例</span><span class="sxs-lookup"><span data-stu-id="fc46a-118">Example</span></span>

<span data-ttu-id="fc46a-119">本示例检索 SharePoint 列表中的 listItem 的版本：</span><span class="sxs-lookup"><span data-stu-id="fc46a-119">This example retrieves the versions of a listItem in a SharePoint list:</span></span>

### <a name="http-request"></a><span data-ttu-id="fc46a-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fc46a-120">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-previous-versions-listitem", "scopes": "files.read sites.read.all" } -->

```http
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions
```

### <a name="response"></a><span data-ttu-id="fc46a-121">响应</span><span class="sxs-lookup"><span data-stu-id="fc46a-121">Response</span></span>

<span data-ttu-id="fc46a-122">这将返回版本的集合：</span><span class="sxs-lookup"><span data-stu-id="fc46a-122">This returns a collection of versions:</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.listItemVersion)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value":
  [
    {
      "id": "3.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-14T12:34:53.912Z"
    },
    {
      "id": "2.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-11T10:21:03.000Z"
    },
    {
      "id": "1.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-10T15:20:01.125Z"
    }
  ]
}
```


<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history"
} -->
