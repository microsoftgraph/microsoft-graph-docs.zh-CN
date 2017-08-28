# <a name="get-photo"></a><span data-ttu-id="ba3f2-101">获取照片</span><span class="sxs-lookup"><span data-stu-id="ba3f2-101">Get photo</span></span>

<span data-ttu-id="ba3f2-102">检索 photo 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ba3f2-102">Retrieve the properties and relationships of photo object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ba3f2-103">权限</span><span class="sxs-lookup"><span data-stu-id="ba3f2-103">Permissions</span></span>
<span data-ttu-id="ba3f2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="ba3f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ba3f2-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="ba3f2-106">Permission type</span></span>      | <span data-ttu-id="ba3f2-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ba3f2-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ba3f2-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ba3f2-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ba3f2-109">Files.Read</span><span class="sxs-lookup"><span data-stu-id="ba3f2-109">Files.Read</span></span>    |
|<span data-ttu-id="ba3f2-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ba3f2-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba3f2-111">Files.Read</span><span class="sxs-lookup"><span data-stu-id="ba3f2-111">Files.Read</span></span>    |
|<span data-ttu-id="ba3f2-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="ba3f2-112">Application</span></span> | <span data-ttu-id="ba3f2-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="ba3f2-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba3f2-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ba3f2-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/photo
GET /groups/{id}/photo
GET /drive/root/createdByUser/photo
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ba3f2-115">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ba3f2-115">Optional query parameters</span></span>
<span data-ttu-id="ba3f2-116">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ba3f2-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ba3f2-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="ba3f2-117">Request headers</span></span>
| <span data-ttu-id="ba3f2-118">名称</span><span class="sxs-lookup"><span data-stu-id="ba3f2-118">Name</span></span>       | <span data-ttu-id="ba3f2-119">类型</span><span class="sxs-lookup"><span data-stu-id="ba3f2-119">Type</span></span> | <span data-ttu-id="ba3f2-120">说明</span><span class="sxs-lookup"><span data-stu-id="ba3f2-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ba3f2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba3f2-121">Authorization</span></span>  | <span data-ttu-id="ba3f2-122">string</span><span class="sxs-lookup"><span data-stu-id="ba3f2-122">string</span></span>  | <span data-ttu-id="ba3f2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ba3f2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ba3f2-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="ba3f2-125">Request body</span></span>
<span data-ttu-id="ba3f2-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ba3f2-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba3f2-127">响应</span><span class="sxs-lookup"><span data-stu-id="ba3f2-127">Response</span></span>

<span data-ttu-id="ba3f2-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [photo](../resources/photo.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ba3f2-128">If successful, this method returns a `200 OK` response code and [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ba3f2-129">示例</span><span class="sxs-lookup"><span data-stu-id="ba3f2-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ba3f2-130">请求</span><span class="sxs-lookup"><span data-stu-id="ba3f2-130">Request</span></span>
<span data-ttu-id="ba3f2-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ba3f2-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photo"
}-->
```http
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo
```
##### <a name="response"></a><span data-ttu-id="ba3f2-132">响应</span><span class="sxs-lookup"><span data-stu-id="ba3f2-132">Response</span></span>
<span data-ttu-id="ba3f2-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ba3f2-133">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.profilePhoto"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 53

{
  "height": 99,
  "width": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
