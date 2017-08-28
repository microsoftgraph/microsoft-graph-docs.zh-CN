# <a name="get-thumbnailset"></a><span data-ttu-id="74498-101">Get thumbnailSet</span><span class="sxs-lookup"><span data-stu-id="74498-101">Get thumbnailSet</span></span>

<span data-ttu-id="74498-102">检索 [thumbnailSet](../resources/thumbnailset.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="74498-102">Retrieve the properties and relationships of a [thumbnailSet](../resources/thumbnailset.md) object.</span></span>

<span data-ttu-id="74498-103">有关详细信息，请参阅 [列出缩略图](item_list_thumbnails.md)。</span><span class="sxs-lookup"><span data-stu-id="74498-103">For more info, see [List thumbnails](item_list_thumbnails.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="74498-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="74498-104">Prerequisites</span></span>
<span data-ttu-id="74498-105">要执行此 API，需要以下**范围**之一：</span><span class="sxs-lookup"><span data-stu-id="74498-105">One of the following **scopes** is required to execute this API:</span></span>

  * <span data-ttu-id="74498-106">Files.Read</span><span class="sxs-lookup"><span data-stu-id="74498-106">Files.Read</span></span>

## <a name="http-request"></a><span data-ttu-id="74498-107">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="74498-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /drive/root/thumbnails/{id}
GET /drive/items/{id}/thumbnails/{id}
GET /drives/{id}/root/thumbnails/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="74498-108">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="74498-108">Optional query parameters</span></span>
<span data-ttu-id="74498-109">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="74498-109">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="74498-110">请求标头</span><span class="sxs-lookup"><span data-stu-id="74498-110">Request headers</span></span>
| <span data-ttu-id="74498-111">名称</span><span class="sxs-lookup"><span data-stu-id="74498-111">Name</span></span>       | <span data-ttu-id="74498-112">类型</span><span class="sxs-lookup"><span data-stu-id="74498-112">Type</span></span> | <span data-ttu-id="74498-113">说明</span><span class="sxs-lookup"><span data-stu-id="74498-113">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="74498-114">Authorization</span><span class="sxs-lookup"><span data-stu-id="74498-114">Authorization</span></span>  | <span data-ttu-id="74498-115">string</span><span class="sxs-lookup"><span data-stu-id="74498-115">string</span></span>  | <span data-ttu-id="74498-p101">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="74498-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="74498-118">请求正文</span><span class="sxs-lookup"><span data-stu-id="74498-118">Request body</span></span>
<span data-ttu-id="74498-119">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="74498-119">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="74498-120">响应</span><span class="sxs-lookup"><span data-stu-id="74498-120">Response</span></span>

<span data-ttu-id="74498-121">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [thumbnailSet](../resources/thumbnailset.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="74498-121">If successful, this method returns a `200 OK` response code and [thumbnailSet](../resources/thumbnailset.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="74498-122">示例</span><span class="sxs-lookup"><span data-stu-id="74498-122">Example</span></span>
##### <a name="request"></a><span data-ttu-id="74498-123">请求</span><span class="sxs-lookup"><span data-stu-id="74498-123">Request</span></span>
<span data-ttu-id="74498-124">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="74498-124">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_thumbnailset"
}-->
```http
GET https://graph.microsoft.com/v1.0/drive/root/thumbnails/{id}
```
##### <a name="response"></a><span data-ttu-id="74498-125">响应</span><span class="sxs-lookup"><span data-stu-id="74498-125">Response</span></span>
<span data-ttu-id="74498-126">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="74498-126">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.thumbnailSet"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 456

{
  "id": "id-value",
  "large": {
    "height": 99,
    "url": "url-value",
    "width": 99
  },
  "medium": {
    "height": 99,
    "url": "url-value",
    "width": 99
  },
  "small": {
    "height": 99,
    "url": "url-value",
    "width": 99
  },
  "source": {
    "height": 99,
    "url": "url-value",
    "width": 99
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get thumbnailSet",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
