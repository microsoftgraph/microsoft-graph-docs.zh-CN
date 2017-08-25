# <a name="get-a-driveitem-resource"></a><span data-ttu-id="236dc-101">获取 DriveItem 资源</span><span class="sxs-lookup"><span data-stu-id="236dc-101">Get a DriveItem resource</span></span>

<span data-ttu-id="236dc-102">通过文件系统路径或 ID 在[驱动器](../resources/drive.md)中检索 [DriveItem](../resources/driveitem.md) 的元数据。</span><span class="sxs-lookup"><span data-stu-id="236dc-102">Retrieve the metadata for a [DriveItem](../resources/driveitem.md) in a [Drive](../resources/drive.md) by file system path or ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="236dc-103">权限</span><span class="sxs-lookup"><span data-stu-id="236dc-103">Permissions</span></span>
<span data-ttu-id="236dc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="236dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="236dc-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="236dc-106">Permission type</span></span>      | <span data-ttu-id="236dc-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="236dc-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="236dc-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="236dc-108">Delegated (work or school account)</span></span> | <span data-ttu-id="236dc-109">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="236dc-109">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    | 
|<span data-ttu-id="236dc-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="236dc-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="236dc-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="236dc-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    | 
|<span data-ttu-id="236dc-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="236dc-112">Application</span></span> | <span data-ttu-id="236dc-113">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="236dc-113">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="236dc-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="236dc-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{item-id}
GET /me/drive/root:/{item-path}
GET /drives/{drive-id}/items/{item-id}
GET /groups/{group-id}/drive/items/{item-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="236dc-115">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="236dc-115">Optional query parameters</span></span>
<span data-ttu-id="236dc-116">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="236dc-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="236dc-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="236dc-117">Request headers</span></span>

| <span data-ttu-id="236dc-118">名称</span><span class="sxs-lookup"><span data-stu-id="236dc-118">Name</span></span>          | <span data-ttu-id="236dc-119">值</span><span class="sxs-lookup"><span data-stu-id="236dc-119">Value</span></span>  | <span data-ttu-id="236dc-120">说明</span><span class="sxs-lookup"><span data-stu-id="236dc-120">Description</span></span>                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="236dc-121">if-none-match</span><span class="sxs-lookup"><span data-stu-id="236dc-121">if-none-match</span></span> | <span data-ttu-id="236dc-122">String</span><span class="sxs-lookup"><span data-stu-id="236dc-122">String</span></span> | <span data-ttu-id="236dc-123">如果包含此请求标头，且提供的 eTag（或 cTag）与文件中的当前标记不匹配，则返回 `HTTP 304 Not Modified` 响应。</span><span class="sxs-lookup"><span data-stu-id="236dc-123">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |


## <a name="request-body"></a><span data-ttu-id="236dc-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="236dc-124">Request body</span></span>
<span data-ttu-id="236dc-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="236dc-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="236dc-126">响应</span><span class="sxs-lookup"><span data-stu-id="236dc-126">Response</span></span>

<span data-ttu-id="236dc-127">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [DriveItem](../resources/driveitem.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="236dc-127">If successful, this method returns a `200 OK` response code and the [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="236dc-128">示例</span><span class="sxs-lookup"><span data-stu-id="236dc-128">Example</span></span>

##### <a name="request"></a><span data-ttu-id="236dc-129">请求</span><span class="sxs-lookup"><span data-stu-id="236dc-129">Request</span></span>

<span data-ttu-id="236dc-130">下面是用户的 OneDrive 的根文件夹请求示例。</span><span class="sxs-lookup"><span data-stu-id="236dc-130">Here is an example of the request to the root folder of the user's OneDrive.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_item"
}-->
```
GET https://graph.microsoft.com/v1.0//me/drive/root
```

##### <a name="response"></a><span data-ttu-id="236dc-131">响应</span><span class="sxs-lookup"><span data-stu-id="236dc-131">Response</span></span>
<span data-ttu-id="236dc-132">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="236dc-132">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "createdBy": {
      "user": {
          "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
          "displayName": "Ryan Gregg"
      }
  },
  "createdDateTime": "2016-03-21T20:01:37Z",
  "cTag": "\"c:{86EB4C8E-D20D-46B9-AD41-23B8868DDA8A},0\"",
  "eTag": "\"{86EB4C8E-D20D-46B9-AD41-23B8868DDA8A},1\"",
  "folder": { "childCount": 120 },
  "id": "01NKDM7HMOJTVYMDOSXFDK2QJDXCDI3WUK",
  "lastModifiedBy": {
      "user": {
          "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
          "displayName": "Ryan Gregg"
      }
  },
  "lastModifiedDateTime": "2016-03-21T20:01:37Z",
  "name": "OneDrive",
  "root": { },
  "size": 157286400,
  "webUrl": "https://contoso-my.sharepoint.com/personal/rgregg_contoso_com/Documents"
}
```

## <a name="notes"></a><span data-ttu-id="236dc-133">说明</span><span class="sxs-lookup"><span data-stu-id="236dc-133">Notes</span></span>

<span data-ttu-id="236dc-134">如果某个项具有**子项**关系，在检索该项的元数据时可以使用 [`$expand` 查询字符串参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来包括同一调用中的项的子项。</span><span class="sxs-lookup"><span data-stu-id="236dc-134">You can use the [`$expand` query string parameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to include the children of an item in the same call as retrieving the metadata of an item if the item has a **children** relationship.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get item",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Get item"
}-->
