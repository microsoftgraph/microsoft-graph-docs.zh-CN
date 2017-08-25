# <a name="list-children-of-a-driveitem"></a><span data-ttu-id="6e214-101">列出 DriveItem 的子项</span><span class="sxs-lookup"><span data-stu-id="6e214-101">List children of a driveItem</span></span>

<span data-ttu-id="6e214-102">在 DriveItem 的 **children** 关系中返回 [DriveItems](../resources/driveitem.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="6e214-102">Return a collection of [DriveItems](../resources/driveitem.md) in the **children** relationship of a DriveItem.</span></span>

<span data-ttu-id="6e214-103">具有非 null **folder** 或 **package** facet 的 DriveItem 可以拥有一个或多个子 DriveItem。</span><span class="sxs-lookup"><span data-stu-id="6e214-103">DriveItems with a non-null **folder** or **package** facet can have one or more child DriveItems.</span></span>


## <a name="permissions"></a><span data-ttu-id="6e214-104">权限</span><span class="sxs-lookup"><span data-stu-id="6e214-104">Permissions</span></span>
<span data-ttu-id="6e214-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="6e214-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6e214-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="6e214-107">Permission type</span></span>      | <span data-ttu-id="6e214-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6e214-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="6e214-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6e214-109">Delegated (work or school account)</span></span> | <span data-ttu-id="6e214-110">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e214-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    | 
|<span data-ttu-id="6e214-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6e214-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e214-112">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e214-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    | 
|<span data-ttu-id="6e214-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="6e214-113">Application</span></span> | <span data-ttu-id="6e214-114">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e214-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="6e214-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6e214-115">HTTP request</span></span>
```http
GET /me/drive/root/children
GET /me/drive/items/{item-id}/children
GET /me/drive/root:/{item-path}:/children
GET /drives/{drive-id}/items/{item-id}/children
GET /groups/{group-id}/drive/root/children
GET /groups/{group-id}/drive/items/{item-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6e214-116">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6e214-116">Optional query parameters</span></span>
<span data-ttu-id="6e214-117">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6e214-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6e214-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="6e214-118">Request headers</span></span>

| <span data-ttu-id="6e214-119">名称</span><span class="sxs-lookup"><span data-stu-id="6e214-119">Name</span></span>          | <span data-ttu-id="6e214-120">类型</span><span class="sxs-lookup"><span data-stu-id="6e214-120">Type</span></span>   | <span data-ttu-id="6e214-121">说明</span><span class="sxs-lookup"><span data-stu-id="6e214-121">Description</span></span>                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="6e214-122">if-none-match</span><span class="sxs-lookup"><span data-stu-id="6e214-122">if-none-match</span></span> | <span data-ttu-id="6e214-123">String</span><span class="sxs-lookup"><span data-stu-id="6e214-123">String</span></span> | <span data-ttu-id="6e214-124">如果包含此请求标头，且提供的 eTag（或 cTag）与文件中的当前标记不匹配，则返回 `HTTP 304 Not Modified` 响应。</span><span class="sxs-lookup"><span data-stu-id="6e214-124">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6e214-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="6e214-125">Request body</span></span>
<span data-ttu-id="6e214-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6e214-126">Do not supply a request body for this method.</span></span>

## <a name="example"></a><span data-ttu-id="6e214-127">示例</span><span class="sxs-lookup"><span data-stu-id="6e214-127">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6e214-128">请求</span><span class="sxs-lookup"><span data-stu-id="6e214-128">Request</span></span>
<span data-ttu-id="6e214-129">下面是请求返回当前用户 OneDrive 的根文件夹中的 DriveItems 的示例。</span><span class="sxs-lookup"><span data-stu-id="6e214-129">Here is an example request to return the DriveItems in the root folder of the current user's OneDrive.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_children"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/children
```

## <a name="response"></a><span data-ttu-id="6e214-130">响应</span><span class="sxs-lookup"><span data-stu-id="6e214-130">Response</span></span>

<span data-ttu-id="6e214-131">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6e214-131">Here is an example of the response.</span></span>
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

<span data-ttu-id="6e214-132">**注意：**如果集合超出默认页面大小（200 项），则在响应中返回 **@odata.nextLink** 属性以指示有更多项可用，并提供下一页项目的请求 URL。</span><span class="sxs-lookup"><span data-stu-id="6e214-132">**Note:** If a collection exceeds the default page size (200 items), the **@odata.nextLink** property is returned in the response to indicate more items are available and provide the request URL for the next page of items.</span></span>

<span data-ttu-id="6e214-133">可以通过 [可选的查询字符串参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 控制页面大小</span><span class="sxs-lookup"><span data-stu-id="6e214-133">You can control the page size through [optional query string parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List the children of an item.",
  "keywords": "list,children,collection",
  "section": "documentation",
  "tocPath": "OneDrive/DriveItem/List children"
} -->
