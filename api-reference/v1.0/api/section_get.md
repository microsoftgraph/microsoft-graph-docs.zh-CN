# <a name="get-section"></a><span data-ttu-id="14b3f-101">获取分区</span><span class="sxs-lookup"><span data-stu-id="14b3f-101">Get section</span></span>

<span data-ttu-id="14b3f-102">检索 [section](../resources/section.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="14b3f-102">Retrieve the properties and relationships of a [section](../resources/section.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="14b3f-103">权限</span><span class="sxs-lookup"><span data-stu-id="14b3f-103">Permissions</span></span>
<span data-ttu-id="14b3f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="14b3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="14b3f-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="14b3f-106">Permission type</span></span>      | <span data-ttu-id="14b3f-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="14b3f-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="14b3f-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="14b3f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="14b3f-109">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14b3f-109">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, or Notes.ReadWrite.All</span></span>    | 
|<span data-ttu-id="14b3f-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="14b3f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14b3f-111">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="14b3f-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, or Notes.ReadWrite.All</span></span>    | 
|<span data-ttu-id="14b3f-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="14b3f-112">Application</span></span> | <span data-ttu-id="14b3f-113">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14b3f-113">Notes.Read, Notes.ReadWrite, Notes.Read.All, or Notes.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="14b3f-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="14b3f-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sections/{id}
GET /users/{id | userPrincipalName}/onenote/sections/{id}
GET /groups/{id}/onenote/sections/{id}
GET /sites/{id}/onenote/sections/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="14b3f-115">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="14b3f-115">Optional query parameters</span></span>
<span data-ttu-id="14b3f-116">此方法支持 `select` 和 `expand` [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="14b3f-116">This method supports the `select` and `expand` [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="14b3f-p102">默认查询展开 `parentNotebook`，并选择其 `id`、`displayName` 和 `self` 属性。分区的有效 `expand` 值为 `parentNotebook` 和 `parentSectionGroup`。</span><span class="sxs-lookup"><span data-stu-id="14b3f-p102">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties. Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="14b3f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="14b3f-119">Request headers</span></span>
| <span data-ttu-id="14b3f-120">名称</span><span class="sxs-lookup"><span data-stu-id="14b3f-120">Name</span></span>       | <span data-ttu-id="14b3f-121">类型</span><span class="sxs-lookup"><span data-stu-id="14b3f-121">Type</span></span> | <span data-ttu-id="14b3f-122">说明</span><span class="sxs-lookup"><span data-stu-id="14b3f-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="14b3f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="14b3f-123">Authorization</span></span>  | <span data-ttu-id="14b3f-124">string</span><span class="sxs-lookup"><span data-stu-id="14b3f-124">string</span></span>  | <span data-ttu-id="14b3f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="14b3f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="14b3f-127">接受</span><span class="sxs-lookup"><span data-stu-id="14b3f-127">Accept</span></span> | <span data-ttu-id="14b3f-128">string</span><span class="sxs-lookup"><span data-stu-id="14b3f-128">string</span></span> | `application/json` | 

## <a name="request-body"></a><span data-ttu-id="14b3f-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="14b3f-129">Request body</span></span>
<span data-ttu-id="14b3f-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="14b3f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="14b3f-131">响应</span><span class="sxs-lookup"><span data-stu-id="14b3f-131">Response</span></span>

<span data-ttu-id="14b3f-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [section](../resources/section.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="14b3f-132">If successful, this method returns a `200 OK` response code and a [section](../resources/section.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="14b3f-133">示例</span><span class="sxs-lookup"><span data-stu-id="14b3f-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="14b3f-134">请求</span><span class="sxs-lookup"><span data-stu-id="14b3f-134">Request</span></span>
<span data-ttu-id="14b3f-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="14b3f-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_section"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/sections/{id}
```
##### <a name="response"></a><span data-ttu-id="14b3f-136">响应</span><span class="sxs-lookup"><span data-stu-id="14b3f-136">Response</span></span>
<span data-ttu-id="14b3f-p104">下面是一个响应示例。注意：为了简单起见，会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="14b3f-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteSection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 272

{
  "isDefault": true,
  "pagesUrl": "pagesUrl-value",
  "displayName": "name-value",
  "createdBy": {
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  },
  "lastModifiedBy": {
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get section",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->