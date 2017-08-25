# <a name="get-page"></a><span data-ttu-id="661df-101">获取页面</span><span class="sxs-lookup"><span data-stu-id="661df-101">Get page</span></span>

<span data-ttu-id="661df-102">检索[页面](../resources/page.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="661df-102">Retrieve the properties and relationships of a [page](../resources/page.md) object.</span></span>

<span data-ttu-id="661df-103">**获取页面信息**</span><span class="sxs-lookup"><span data-stu-id="661df-103">**Getting page information**</span></span>

<span data-ttu-id="661df-104">根据页标识符访问页面的元数据：</span><span class="sxs-lookup"><span data-stu-id="661df-104">Access a page's metadata by page identifier:</span></span>

```
GET /me/onenote/pages/{id}
```

<span data-ttu-id="661df-105">**获取页面内容**</span><span class="sxs-lookup"><span data-stu-id="661df-105">**Getting page content**</span></span>

<span data-ttu-id="661df-106">可以使用页面的 `content` 终结点获取页面的 HTML 内容：</span><span class="sxs-lookup"><span data-stu-id="661df-106">You can use the page's `content` endpoint to get the HTML content of a page:</span></span>

```
GET /me/onenote/pages/{id}/content[?includeIDs=true]
GET /me/onenote/pages/{id}/$value[?includeIDs=true]
```

<span data-ttu-id="661df-107">`includeIDs=true` 查询选项用于[更新页面](../api/page_update.md)。</span><span class="sxs-lookup"><span data-stu-id="661df-107">The `includeIDs=true` query option is used to [update pages](../api/page_update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="661df-108">权限</span><span class="sxs-lookup"><span data-stu-id="661df-108">Permissions</span></span>
<span data-ttu-id="661df-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="661df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="661df-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="661df-111">Permission type</span></span>      | <span data-ttu-id="661df-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="661df-112">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="661df-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="661df-113">Delegated (work or school account)</span></span> | <span data-ttu-id="661df-114">Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="661df-114">Notes.Read, Notes.ReadWrite, Notes.Read.All, or Notes.ReadWrite.All</span></span>    | 
|<span data-ttu-id="661df-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="661df-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="661df-116">Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="661df-116">Notes.Read, Notes.ReadWrite</span></span>    | 
|<span data-ttu-id="661df-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="661df-117">Application</span></span> | <span data-ttu-id="661df-118">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="661df-118">Notes.Read, Notes.ReadWrite, Notes.Read.All, or Notes.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="661df-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="661df-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/pages/{id}
GET /users/{id | userPrincipalName}/onenote/pages/{id}
GET /groups/{id}/onenote/pages/{id}
GET /sites/{id}/onenote/pages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="661df-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="661df-120">Optional query parameters</span></span>
<span data-ttu-id="661df-121">此方法支持 `select` 和 `expand` [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="661df-121">This method supports the `select` and `expand` [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="661df-p102">默认响应将展开 `parentSection` 并选择分区的 `id`、`name`、和 `self` 属性。页面的有效 `expand` 值为 `parentNotebook` 和 `parentSection`。</span><span class="sxs-lookup"><span data-stu-id="661df-p102">The default response expands `parentSection` and selects the section's `id`, `name`, and `self` properties. Valid `expand` values for pages are `parentNotebook` and `parentSection`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="661df-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="661df-124">Request headers</span></span>
| <span data-ttu-id="661df-125">名称</span><span class="sxs-lookup"><span data-stu-id="661df-125">Name</span></span>       | <span data-ttu-id="661df-126">类型</span><span class="sxs-lookup"><span data-stu-id="661df-126">Type</span></span> | <span data-ttu-id="661df-127">说明</span><span class="sxs-lookup"><span data-stu-id="661df-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="661df-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="661df-128">Authorization</span></span>  | <span data-ttu-id="661df-129">string</span><span class="sxs-lookup"><span data-stu-id="661df-129">string</span></span>  | <span data-ttu-id="661df-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="661df-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="661df-132">接受</span><span class="sxs-lookup"><span data-stu-id="661df-132">Accept</span></span> | <span data-ttu-id="661df-133">string</span><span class="sxs-lookup"><span data-stu-id="661df-133">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="661df-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="661df-134">Request body</span></span>
<span data-ttu-id="661df-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="661df-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="661df-136">响应</span><span class="sxs-lookup"><span data-stu-id="661df-136">Response</span></span>

<span data-ttu-id="661df-137">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [page](../resources/page.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="661df-137">If successful, this method returns a `200 OK` response code and the [page](../resources/page.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="661df-138">示例</span><span class="sxs-lookup"><span data-stu-id="661df-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="661df-139">请求</span><span class="sxs-lookup"><span data-stu-id="661df-139">Request</span></span>
<span data-ttu-id="661df-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="661df-140">Here is an example of the request.</span></span>
 <!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/pages/{id}
```
##### <a name="response"></a><span data-ttu-id="661df-141">响应</span><span class="sxs-lookup"><span data-stu-id="661df-141">Response</span></span>
<span data-ttu-id="661df-p104">下面是一个响应示例。注意：为了简单起见，会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="661df-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
 <!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 312

{
  "title": "title-value",
  "createdByAppId": "createdByAppId-value",
  "links": {
    "oneNoteClientUrl": {
      "href": "href-value"
    },
    "oneNoteWebUrl": {
      "href": "href-value"
    }
  },
  "contentUrl": "contentUrl-value",
  "content": "content-value",
  "lastModifiedDateTime": "2016-10-19T10:37:00Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get page",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
