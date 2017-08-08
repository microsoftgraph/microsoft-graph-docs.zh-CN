# <a name="enumerate-subsites-of-a-site"></a><span data-ttu-id="8a83f-101">枚举网站的子网站</span><span class="sxs-lookup"><span data-stu-id="8a83f-101">Enumerate subsites of a site</span></span>

<span data-ttu-id="8a83f-102">获取为[网站][]定义的子网站集合。</span><span class="sxs-lookup"><span data-stu-id="8a83f-102">Get a collection of subsites defined for a [site][].</span></span>

<span data-ttu-id="8a83f-103">[网站]: ../resources/site.md</span><span class="sxs-lookup"><span data-stu-id="8a83f-103">[site]: ../resources/site.md</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8a83f-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="8a83f-104">Prerequisites</span></span>

<span data-ttu-id="8a83f-105">要执行此请求，需要以下范围之一：</span><span class="sxs-lookup"><span data-stu-id="8a83f-105">One of the following scopes is required to execute this request:</span></span>

* <span data-ttu-id="8a83f-106">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="8a83f-106">Sites.Read.All</span></span>
* <span data-ttu-id="8a83f-107">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a83f-107">Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="8a83f-108">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8a83f-108">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /sites/{site-id}/sites
```

## <a name="example"></a><span data-ttu-id="8a83f-109">示例</span><span class="sxs-lookup"><span data-stu-id="8a83f-109">Example</span></span>

#### <a name="request"></a><span data-ttu-id="8a83f-110">请求</span><span class="sxs-lookup"><span data-stu-id="8a83f-110">Request</span></span>

<!-- { "blockType": "request", "name": "list-subsites" } -->

```http
GET /sites/{site-id}/sites
```

#### <a name="response"></a><span data-ttu-id="8a83f-111">响应</span><span class="sxs-lookup"><span data-stu-id="8a83f-111">Response</span></span>

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
