# <a name="get-notebook"></a><span data-ttu-id="33f6a-101">获取笔记本</span><span class="sxs-lookup"><span data-stu-id="33f6a-101">Get notebook</span></span>

<span data-ttu-id="33f6a-102">检索 [notebook](../resources/notebook.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="33f6a-102">Retrieve the properties and relationships of a [notebook](../resources/notebook.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="33f6a-103">权限</span><span class="sxs-lookup"><span data-stu-id="33f6a-103">Permissions</span></span>
<span data-ttu-id="33f6a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="33f6a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="33f6a-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="33f6a-106">Permission type</span></span>      | <span data-ttu-id="33f6a-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="33f6a-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="33f6a-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="33f6a-108">Delegated (work or school account)</span></span> | <span data-ttu-id="33f6a-109">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33f6a-109">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="33f6a-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="33f6a-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33f6a-111">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="33f6a-111">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="33f6a-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="33f6a-112">Application</span></span> | <span data-ttu-id="33f6a-113">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33f6a-113">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="33f6a-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="33f6a-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/{id}
GET /users/{id | userPrincipalName}/onenote/notebooks/{id}
GET /groups/{id}/onenote/notebooks/{id}
GET /sites/{id}/onenote/notebooks/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="33f6a-115">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="33f6a-115">Optional query parameters</span></span>
<span data-ttu-id="33f6a-116">此方法支持 `select` 和 `expand` [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="33f6a-116">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="33f6a-117">笔记本的有效 `expand` 值为 `sections` 和 `sectionGroups`。</span><span class="sxs-lookup"><span data-stu-id="33f6a-117">Valid `expand` values for notebooks are `sections` and `sectionGroups`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="33f6a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="33f6a-118">Request headers</span></span>
| <span data-ttu-id="33f6a-119">名称</span><span class="sxs-lookup"><span data-stu-id="33f6a-119">Name</span></span>       | <span data-ttu-id="33f6a-120">类型</span><span class="sxs-lookup"><span data-stu-id="33f6a-120">Type</span></span> | <span data-ttu-id="33f6a-121">说明</span><span class="sxs-lookup"><span data-stu-id="33f6a-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="33f6a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="33f6a-122">Authorization</span></span>  | <span data-ttu-id="33f6a-123">string</span><span class="sxs-lookup"><span data-stu-id="33f6a-123">string</span></span>  | <span data-ttu-id="33f6a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="33f6a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="33f6a-126">Accept</span><span class="sxs-lookup"><span data-stu-id="33f6a-126">Accept</span></span> | <span data-ttu-id="33f6a-127">string</span><span class="sxs-lookup"><span data-stu-id="33f6a-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="33f6a-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="33f6a-128">Request body</span></span>
<span data-ttu-id="33f6a-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="33f6a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="33f6a-130">响应</span><span class="sxs-lookup"><span data-stu-id="33f6a-130">Response</span></span>

<span data-ttu-id="33f6a-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [notebook](../resources/notebook.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="33f6a-131">If successful, this method returns a `200 OK` response code and a [notebook](../resources/notebook.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="33f6a-132">示例</span><span class="sxs-lookup"><span data-stu-id="33f6a-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="33f6a-133">请求</span><span class="sxs-lookup"><span data-stu-id="33f6a-133">Request</span></span>
<span data-ttu-id="33f6a-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="33f6a-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_notebook"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}
```
##### <a name="response"></a><span data-ttu-id="33f6a-135">响应</span><span class="sxs-lookup"><span data-stu-id="33f6a-135">Response</span></span>
<span data-ttu-id="33f6a-p103">下面是一个响应示例。注意：为了简单起见，会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="33f6a-p103">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 284

{
  "isDefault": true,
  "userRole": {
  },
  "isShared": true,
  "sectionsUrl": "sectionsUrl-value",
  "sectionGroupsUrl": "sectionGroupsUrl-value",
  "links": {
    "oneNoteClientUrl": {
      "href": "href-value"
    },
    "oneNoteWebUrl": {
      "href": "href-value"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get notebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
