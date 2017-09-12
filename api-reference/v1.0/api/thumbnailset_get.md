# <a name="get-thumbnailset"></a><span data-ttu-id="301e6-101">Get thumbnailSet</span><span class="sxs-lookup"><span data-stu-id="301e6-101">Get thumbnailSet</span></span>

<span data-ttu-id="301e6-102">检索 [thumbnailSet](../resources/thumbnailset.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="301e6-102">Retrieve the properties and relationships of a [thumbnailSet](../resources/thumbnailset.md) object.</span></span>

<span data-ttu-id="301e6-103">有关详细信息，请参阅[列出缩略图](item_list_thumbnails.md)。</span><span class="sxs-lookup"><span data-stu-id="301e6-103">For more info, see [List thumbnails](item_list_thumbnails.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="301e6-104">权限</span><span class="sxs-lookup"><span data-stu-id="301e6-104">Permissions</span></span>
<span data-ttu-id="301e6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="301e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="301e6-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="301e6-107">Permission type</span></span>      | <span data-ttu-id="301e6-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="301e6-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="301e6-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="301e6-109">Delegated (work or school account)</span></span> | <span data-ttu-id="301e6-110">Files.Read</span><span class="sxs-lookup"><span data-stu-id="301e6-110">Files.Read</span></span>    | 
|<span data-ttu-id="301e6-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="301e6-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="301e6-112">Files.Read</span><span class="sxs-lookup"><span data-stu-id="301e6-112">Files.Read</span></span>    | 
|<span data-ttu-id="301e6-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="301e6-113">Application</span></span> | <span data-ttu-id="301e6-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="301e6-114">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="301e6-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="301e6-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /drive/root/thumbnails/{id}
GET /drive/items/{id}/thumbnails/{id}
GET /drives/{id}/root/thumbnails/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="301e6-116">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="301e6-116">Optional query parameters</span></span>
<span data-ttu-id="301e6-117">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="301e6-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="301e6-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="301e6-118">Request headers</span></span>
| <span data-ttu-id="301e6-119">名称</span><span class="sxs-lookup"><span data-stu-id="301e6-119">Name</span></span>       | <span data-ttu-id="301e6-120">类型</span><span class="sxs-lookup"><span data-stu-id="301e6-120">Type</span></span> | <span data-ttu-id="301e6-121">说明</span><span class="sxs-lookup"><span data-stu-id="301e6-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="301e6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="301e6-122">Authorization</span></span>  | <span data-ttu-id="301e6-123">string</span><span class="sxs-lookup"><span data-stu-id="301e6-123">string</span></span>  | <span data-ttu-id="301e6-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="301e6-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="301e6-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="301e6-126">Request body</span></span>
<span data-ttu-id="301e6-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="301e6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="301e6-128">响应</span><span class="sxs-lookup"><span data-stu-id="301e6-128">Response</span></span>

<span data-ttu-id="301e6-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [thumbnailSet](../resources/thumbnailset.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="301e6-129">If successful, this method returns a `200 OK` response code and [thumbnailSet](../resources/thumbnailset.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="301e6-130">示例</span><span class="sxs-lookup"><span data-stu-id="301e6-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="301e6-131">请求</span><span class="sxs-lookup"><span data-stu-id="301e6-131">Request</span></span>
<span data-ttu-id="301e6-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="301e6-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_thumbnailset"
}-->
```http
GET https://graph.microsoft.com/v1.0/drive/root/thumbnails/{id}
```
##### <a name="response"></a><span data-ttu-id="301e6-133">响应</span><span class="sxs-lookup"><span data-stu-id="301e6-133">Response</span></span>
<span data-ttu-id="301e6-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="301e6-134">Here is an example of the response.</span></span>
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
