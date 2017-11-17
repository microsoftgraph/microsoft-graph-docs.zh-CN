# <a name="get-resource"></a><span data-ttu-id="ffc64-101">获取资源</span><span class="sxs-lookup"><span data-stu-id="ffc64-101">Get resource</span></span>

<span data-ttu-id="ffc64-102">检索文件或图像 [resource](../resources/resource.md) 对象的二进制数据。</span><span class="sxs-lookup"><span data-stu-id="ffc64-102">Retrieve the binary data of a file or image [resource](../resources/resource.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ffc64-103">权限</span><span class="sxs-lookup"><span data-stu-id="ffc64-103">Permissions</span></span>
<span data-ttu-id="ffc64-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="ffc64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ffc64-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="ffc64-106">Permission type</span></span>      | <span data-ttu-id="ffc64-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ffc64-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ffc64-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ffc64-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ffc64-109">Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffc64-109">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="ffc64-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ffc64-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ffc64-111">Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ffc64-111">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="ffc64-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="ffc64-112">Application</span></span> | <span data-ttu-id="ffc64-113">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffc64-113">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ffc64-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ffc64-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/resources/{id}/content
GET /users/{id | userPrincipalName}/onenote/resources/{id}/content
GET /groups/{id}/onenote/resources/{id}/content
GET /sites/{id}/onenote/resources/{id}/content
```

## <a name="request-headers"></a><span data-ttu-id="ffc64-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="ffc64-115">Request headers</span></span>
| <span data-ttu-id="ffc64-116">名称</span><span class="sxs-lookup"><span data-stu-id="ffc64-116">Name</span></span>       | <span data-ttu-id="ffc64-117">类型</span><span class="sxs-lookup"><span data-stu-id="ffc64-117">Type</span></span> | <span data-ttu-id="ffc64-118">说明</span><span class="sxs-lookup"><span data-stu-id="ffc64-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ffc64-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="ffc64-119">Authorization</span></span>  | <span data-ttu-id="ffc64-120">string</span><span class="sxs-lookup"><span data-stu-id="ffc64-120">string</span></span>  | <span data-ttu-id="ffc64-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ffc64-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ffc64-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="ffc64-123">Request body</span></span>
<span data-ttu-id="ffc64-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ffc64-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ffc64-125">响应</span><span class="sxs-lookup"><span data-stu-id="ffc64-125">Response</span></span>

<span data-ttu-id="ffc64-126">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和图像或文件二进制数据。</span><span class="sxs-lookup"><span data-stu-id="ffc64-126">If successful, this method returns a `200 OK` response code and the image or file binary data in the response body.</span></span>

<span data-ttu-id="ffc64-127">注意：图像无法直接在浏览器中呈现，因为与页面内容的其他部分一样，检索它们需要授权。</span><span class="sxs-lookup"><span data-stu-id="ffc64-127">Note: Images won't render directly in a browser because they require authorization to retrieve them, like the rest of the page content.</span></span>
## <a name="example"></a><span data-ttu-id="ffc64-128">示例</span><span class="sxs-lookup"><span data-stu-id="ffc64-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ffc64-129">请求</span><span class="sxs-lookup"><span data-stu-id="ffc64-129">Request</span></span>
<span data-ttu-id="ffc64-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ffc64-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_resource"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/resources/{id}/content
```
##### <a name="response"></a><span data-ttu-id="ffc64-131">响应</span><span class="sxs-lookup"><span data-stu-id="ffc64-131">Response</span></span>
<span data-ttu-id="ffc64-132">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ffc64-132">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->
```http
HTTP/1.1 200 OK

...binary data...
```
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.onenoteResource"
} -->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
