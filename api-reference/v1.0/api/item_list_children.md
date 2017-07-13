# <span data-ttu-id="65cdd-101">列出 DriveItem 的子项</span><span class="sxs-lookup"><span data-stu-id="65cdd-101">List children of a driveItem</span></span>
<a id="list-children-of-a-driveitem" class="xliff"></a>

<span data-ttu-id="65cdd-102">在 DriveItem 的 **children** 关系中返回 [DriveItems](../resources/driveitem.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="65cdd-102">Return a collection of [DriveItems](../resources/driveitem.md) in the **children** relationship of a DriveItem.</span></span>

<span data-ttu-id="65cdd-103">具有非 null **文件夹**或**包** facet 的 DriveItem 可以拥有一个或多个子 DriveItem。</span><span class="sxs-lookup"><span data-stu-id="65cdd-103">DriveItems with a non-null **folder** or **package** facet can have one or more child DriveItems.</span></span>


## <span data-ttu-id="65cdd-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="65cdd-104">Prerequisites</span></span>
<a id="prerequisites" class="xliff"></a>
<span data-ttu-id="65cdd-105">要执行此 API，需要以下**范围**之一：</span><span class="sxs-lookup"><span data-stu-id="65cdd-105">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="65cdd-106">Files.Read</span><span class="sxs-lookup"><span data-stu-id="65cdd-106">Files.Read</span></span>
* <span data-ttu-id="65cdd-107">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="65cdd-107">Files.ReadWrite</span></span>
* <span data-ttu-id="65cdd-108">Files.Read.All</span><span class="sxs-lookup"><span data-stu-id="65cdd-108">Files.Read.All</span></span>
* <span data-ttu-id="65cdd-109">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65cdd-109">Files.ReadWrite.All</span></span>
* <span data-ttu-id="65cdd-110">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="65cdd-110">Sites.Read.All</span></span>
* <span data-ttu-id="65cdd-111">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65cdd-111">Sites.ReadWrite.All</span></span>

## <span data-ttu-id="65cdd-112">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="65cdd-112">HTTP request</span></span>
<a id="http-request" class="xliff"></a>
```http
GET /me/drive/root/children
GET /me/drive/items/{item-id}/children
GET /me/drive/root:/{item-path}:/children
GET /drives/{drive-id}/items/{item-id}/children
GET /groups/{group-id}/drive/root/children
GET /groups/{group-id}/drive/items/{item-id}
```

## <span data-ttu-id="65cdd-113">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="65cdd-113">Optional query parameters</span></span>
<a id="optional-query-parameters" class="xliff"></a>
<span data-ttu-id="65cdd-114">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="65cdd-114">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <span data-ttu-id="65cdd-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="65cdd-115">Request headers</span></span>
<a id="request-headers" class="xliff"></a>

| <span data-ttu-id="65cdd-116">名称</span><span class="sxs-lookup"><span data-stu-id="65cdd-116">Name</span></span>          | <span data-ttu-id="65cdd-117">类型</span><span class="sxs-lookup"><span data-stu-id="65cdd-117">Type</span></span>   | <span data-ttu-id="65cdd-118">说明</span><span class="sxs-lookup"><span data-stu-id="65cdd-118">Description</span></span>                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="65cdd-119">if-none-match</span><span class="sxs-lookup"><span data-stu-id="65cdd-119">if-none-match</span></span> | <span data-ttu-id="65cdd-120">String</span><span class="sxs-lookup"><span data-stu-id="65cdd-120">String</span></span> | <span data-ttu-id="65cdd-121">如果包含此请求标头，且提供的 eTag（或 cTag）与文件中的当前标记不匹配，则返回 `HTTP 304 Not Modified` 响应。</span><span class="sxs-lookup"><span data-stu-id="65cdd-121">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <span data-ttu-id="65cdd-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="65cdd-122">Request body</span></span>
<a id="request-body" class="xliff"></a>
<span data-ttu-id="65cdd-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="65cdd-123">Do not supply a request body for this method.</span></span>

## <span data-ttu-id="65cdd-124">示例</span><span class="sxs-lookup"><span data-stu-id="65cdd-124">Example</span></span>
<a id="example" class="xliff"></a>

##### <span data-ttu-id="65cdd-125">请求</span><span class="sxs-lookup"><span data-stu-id="65cdd-125">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="65cdd-126">下面是请求返回当前用户 OneDrive 的根文件夹中的 DriveItems 的示例。</span><span class="sxs-lookup"><span data-stu-id="65cdd-126">Here is an example request to return the DriveItems in the root folder of the current user's OneDrive.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_children"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/children
```

## <span data-ttu-id="65cdd-127">响应</span><span class="sxs-lookup"><span data-stu-id="65cdd-127">Response</span></span>
<a id="response" class="xliff"></a>

<span data-ttu-id="65cdd-128">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="65cdd-128">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {"name": "myfile.jpg", "size": 2048, "file": {} },
    {"name": "Documents", "folder": { "childCount": 4} },
    {"name": "Photos", "folder": { "childCount": 203} },
    {"name": "my sheet(1).xlsx", "size": 197 }
  ],
  "@odata.nextLink": "https://..."
}
```

<span data-ttu-id="65cdd-129">**注意：**如果集合超出默认页面大小（200 项），则在响应中返回 **@odata.nextLink** 属性以指示有更多项可用，并提供下一页项目的请求 URL。</span><span class="sxs-lookup"><span data-stu-id="65cdd-129">**Note:** If a collection exceeds the default page size (200 items), the **@odata.nextLink** property is returned in the response to indicate more items are available and provide the request URL for the next page of items.</span></span>

<span data-ttu-id="65cdd-130">可以通过 [可选的查询字符串参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 控制页面大小</span><span class="sxs-lookup"><span data-stu-id="65cdd-130">You can control the page size through [optional query string parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List the children of an item.",
  "keywords": "list,children,collection",
  "section": "documentation",
  "tocPath": "OneDrive/DriveItem/List children"
} -->
