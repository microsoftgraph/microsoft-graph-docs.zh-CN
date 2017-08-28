# <a name="enumerate-subsites-of-a-site"></a><span data-ttu-id="b372f-101">枚举网站的子网站</span><span class="sxs-lookup"><span data-stu-id="b372f-101">Enumerate subsites of a site</span></span>

<span data-ttu-id="b372f-102">获取为[网站][]定义的子网站集合。</span><span class="sxs-lookup"><span data-stu-id="b372f-102">Get a collection of subsites defined for a [site][].</span></span>

<span data-ttu-id="b372f-103">[网站]: ../resources/site.md</span><span class="sxs-lookup"><span data-stu-id="b372f-103">[site]: ../resources/site.md</span></span>

## <a name="permissions"></a><span data-ttu-id="b372f-104">权限</span><span class="sxs-lookup"><span data-stu-id="b372f-104">Permissions</span></span>

<span data-ttu-id="b372f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="b372f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b372f-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="b372f-107">Permission type</span></span>      | <span data-ttu-id="b372f-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b372f-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b372f-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b372f-109">Delegated (work or school account)</span></span> | <span data-ttu-id="b372f-110">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b372f-110">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="b372f-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b372f-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b372f-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="b372f-112">Not supported.</span></span>    |
|<span data-ttu-id="b372f-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="b372f-113">Application</span></span> | <span data-ttu-id="b372f-114">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b372f-114">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b372f-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b372f-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /sites/{site-id}/sites
```

## <a name="example"></a><span data-ttu-id="b372f-116">示例</span><span class="sxs-lookup"><span data-stu-id="b372f-116">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b372f-117">请求</span><span class="sxs-lookup"><span data-stu-id="b372f-117">Request</span></span>

<!-- { "blockType": "request", "name": "list-subsites" } -->

```http
GET /sites/{site-id}/sites
```

#### <a name="response"></a><span data-ttu-id="b372f-118">响应</span><span class="sxs-lookup"><span data-stu-id="b372f-118">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "da60e844-ba1d-49bc-b4d4-d5e36bae9019,712a596e-90a1-49e3-9b48-bfa80bee8740",
      "name": "Team A Subsite",
      "description": "",
      "createdDateTime": "2016-10-18T03:05:59Z",
      "lastModifiedDateTime": "2016-10-18T10:40:59Z",
      "webUrl": "https://contoso.sharepoint.com/sites/site/subsiteA"
    },
    {
      "id": "da60e844-ba1d-49bc-b4d4-d5e36bae9019,0271110f-634f-4300-a841-3a8a2e851851",
      "name": "Team B Subsite",
      "description": "",
      "createdDateTime": "2016-10-18T03:05:59Z",
      "lastModifiedDateTime": "2016-10-18T10:40:59Z",
      "webUrl": "https://contoso.sharepoint.com/sites/site/subsiteB"
    }
  ]
}
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Site/Enumerate subsites"
} -->
