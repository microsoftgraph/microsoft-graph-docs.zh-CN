# <a name="download-the-contents-of-a-driveitem"></a><span data-ttu-id="c4d37-101">下载 DriveItem 的内容</span><span class="sxs-lookup"><span data-stu-id="c4d37-101">Download the contents of a DriveItem</span></span>

<span data-ttu-id="c4d37-p101">下载 DriveItem 的内容。只可以下载具有 **file** 属性的 driveItem。</span><span class="sxs-lookup"><span data-stu-id="c4d37-p101">Download the contents for a driveItem. Only driveItem with the **file** property can be downloaded.</span></span>

## <a name="permissions"></a><span data-ttu-id="c4d37-104">权限</span><span class="sxs-lookup"><span data-stu-id="c4d37-104">Permissions</span></span>
<span data-ttu-id="c4d37-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="c4d37-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c4d37-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="c4d37-107">Permission type</span></span>      | <span data-ttu-id="c4d37-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c4d37-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="c4d37-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c4d37-109">Delegated (work or school account)</span></span> | <span data-ttu-id="c4d37-110">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4d37-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    | 
|<span data-ttu-id="c4d37-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c4d37-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4d37-112">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4d37-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    | 
|<span data-ttu-id="c4d37-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="c4d37-113">Application</span></span> | <span data-ttu-id="c4d37-114">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4d37-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c4d37-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c4d37-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root:/{item-path}:/content
GET /me/drive/items/{item-id}/content
GET /drives/items/{item-id}/content
GET /groups/{group-id}/drive/items/{item-id}/content
```

## <a name="request-headers"></a><span data-ttu-id="c4d37-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="c4d37-116">Request headers</span></span>

| <span data-ttu-id="c4d37-117">名称</span><span class="sxs-lookup"><span data-stu-id="c4d37-117">Name</span></span>          | <span data-ttu-id="c4d37-118">值</span><span class="sxs-lookup"><span data-stu-id="c4d37-118">Value</span></span>  | <span data-ttu-id="c4d37-119">说明</span><span class="sxs-lookup"><span data-stu-id="c4d37-119">Description</span></span>                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="c4d37-120">if-none-match</span><span class="sxs-lookup"><span data-stu-id="c4d37-120">if-none-match</span></span> | <span data-ttu-id="c4d37-121">String</span><span class="sxs-lookup"><span data-stu-id="c4d37-121">String</span></span> | <span data-ttu-id="c4d37-122">如果包含此请求标头，且提供的 eTag（或 cTag）与文件中的当前标记不匹配，则返回 `HTTP 304 Not Modified` 响应。</span><span class="sxs-lookup"><span data-stu-id="c4d37-122">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |


## <a name="request-body"></a><span data-ttu-id="c4d37-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="c4d37-123">Request body</span></span>
<span data-ttu-id="c4d37-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c4d37-124">Do not supply a request body for this method.</span></span>

## <a name="example"></a><span data-ttu-id="c4d37-125">示例</span><span class="sxs-lookup"><span data-stu-id="c4d37-125">Example</span></span>
<span data-ttu-id="c4d37-126">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="c4d37-126">Here is an example of how to call this API.</span></span>


<!-- { "blockType": "request", "name": "driveitem-download-contents" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/content
```

##### <a name="response"></a><span data-ttu-id="c4d37-127">响应</span><span class="sxs-lookup"><span data-stu-id="c4d37-127">Response</span></span>
<span data-ttu-id="c4d37-p103">返回 `302 Found` 响应，该响应重定向到文件的预先身份验证的下载 URL。这是可通过 DriveItem 上的 `@microsoft.graph.downloadUrl` 属性获得的同一个 URL。</span><span class="sxs-lookup"><span data-stu-id="c4d37-p103">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the file. This is the same URL available through the `@microsoft.graph.downloadUrl` property on the DriveItem.</span></span>

<span data-ttu-id="c4d37-p104">若要下载该文件的内容，应用程序将需要遵循响应中的 `Location` 标头。许多 HTTP 客户端库将自动遵循 302 重定向并立即开始下载文件。</span><span class="sxs-lookup"><span data-stu-id="c4d37-p104">To download the contents of the file your application will need to follow the `Location` header in the response. Many HTTP client libraries will automatically follow the 302 redirection and start downloading the file immedately.</span></span>

<span data-ttu-id="c4d37-132">预先身份验证的下载 URL 仅在较短的一段时间 （几分钟后）内有效，不需要 `Authorization` 标头即可下载。</span><span class="sxs-lookup"><span data-stu-id="c4d37-132">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->
```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

## <a name="partial-range-downloads"></a><span data-ttu-id="c4d37-133">部分范围下载</span><span class="sxs-lookup"><span data-stu-id="c4d37-133">Partial range downloads</span></span>

<span data-ttu-id="c4d37-p105">若要从文件中下载部分范围的字节，应用程序可以使用 [RFC 2616](https://www.ietf.org/rfc/rfc2616.txt) 中指定的 `Range` 标头。请注意，必须将 `Range` 标头附加到实际 `@microsoft.graph.downloadUrl` URL，而不是 `/content` 的请求。</span><span class="sxs-lookup"><span data-stu-id="c4d37-p105">To download a partial range of bytes from the file, your app can use the `Range` header as specified in [RFC 2616](https://www.ietf.org/rfc/rfc2616.txt). Note that you must append the `Range` header to the actual `@microsoft.graph.downloadUrl` URL and not to the request for `/content`.</span></span>

<!-- { "blockType": "request", "name": "driveitem-get-partial-content" } -->
```http
GET https://b0mpua-by3301.files.1drv.com/y23vmag
Range: bytes=0-1023
```

<span data-ttu-id="c4d37-p106">此方法将返回 `HTTP 206 Partial Content` 响应和文件中字节的请求区域。如果无法生成此范围，可能会忽略 Range 标头，并会返回包含文件完整内容的 `HTTP 200` 响应。</span><span class="sxs-lookup"><span data-stu-id="c4d37-p106">This will return an `HTTP 206 Partial Content` response with the request range of bytes from the file. If the range cannot be generated the Range header may be ignored and an `HTTP 200` response would be returned with the full contents of the file.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->
```http
HTTP/1.1 206 Partial Content
Content-Range: bytes 0-1023/2048

<first 1024 bytes of file>
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Download item",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Download file"
}-->
