# <a name="get-onenoteoperation"></a><span data-ttu-id="d5cb4-101">获得 onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="d5cb4-101">Get onenoteOperation</span></span>

<span data-ttu-id="d5cb4-p101">获取长时间运行的 OneNote 操作的状态。这适用于在响应中返回 **Operation-Location** 标头的操作，例如 `CopyNotebook`、`CopyToNotebook`、`CopyToSectionGroup`、`and CopyToSection`。</span><span class="sxs-lookup"><span data-stu-id="d5cb4-p101">Get the status of a long-running OneNote operation. This applies to operations that return the **Operation-Location** header in the response, such as `CopyNotebook`, `CopyToNotebook`, `CopyToSectionGroup`, `and CopyToSection`.</span></span>   

<span data-ttu-id="d5cb4-104">可以轮询 Operation-Location 终结点，直到 `status` 属性返回 `completed` 或 `failed`。</span><span class="sxs-lookup"><span data-stu-id="d5cb4-104">You can poll the Operation-Location endpoint until the `status` property returns `completed` or `failed`.</span></span> 

<span data-ttu-id="d5cb4-105">如果状态是 `completed`，则此 `resourceLocation` 属性包含资源终结点 URI。</span><span class="sxs-lookup"><span data-stu-id="d5cb4-105">If the status is `completed`, the `resourceLocation` property contains the resource endpoint URI.</span></span> 

<span data-ttu-id="d5cb4-106">如果状态是 `failed`，错误和 `@api.diagnostics` 属性提供错误信息。</span><span class="sxs-lookup"><span data-stu-id="d5cb4-106">If the status is `failed`, the error and `@api.diagnostics` properties provide error information.</span></span>

## <a name="permissions"></a><span data-ttu-id="d5cb4-107">权限</span><span class="sxs-lookup"><span data-stu-id="d5cb4-107">Permissions</span></span>
<span data-ttu-id="d5cb4-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="d5cb4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d5cb4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d5cb4-110">Permission type</span></span>      | <span data-ttu-id="d5cb4-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d5cb4-111">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="d5cb4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d5cb4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d5cb4-113">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5cb4-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, or Notes.ReadWrite.All</span></span>    | 
|<span data-ttu-id="d5cb4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d5cb4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5cb4-115">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d5cb4-115">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, or Notes.ReadWrite.All</span></span>    | 
|<span data-ttu-id="d5cb4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d5cb4-116">Application</span></span> | <span data-ttu-id="d5cb4-117">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5cb4-117">Notes.Read, Notes.ReadWrite, Notes.Read.All, or Notes.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d5cb4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d5cb4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/operations/{id}
GET /users/{id | userPrincipalName}/onenote/operations/{id}
GET /groups/{id}/onenote/operations/{id}
GET /sites/{id}/onenote/operations/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d5cb4-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d5cb4-119">Optional query parameters</span></span>
<span data-ttu-id="d5cb4-120">无。</span><span class="sxs-lookup"><span data-stu-id="d5cb4-120">None.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d5cb4-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="d5cb4-121">Request headers</span></span>
| <span data-ttu-id="d5cb4-122">名称</span><span class="sxs-lookup"><span data-stu-id="d5cb4-122">Name</span></span>       | <span data-ttu-id="d5cb4-123">类型</span><span class="sxs-lookup"><span data-stu-id="d5cb4-123">Type</span></span> | <span data-ttu-id="d5cb4-124">说明</span><span class="sxs-lookup"><span data-stu-id="d5cb4-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d5cb4-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5cb4-125">Authorization</span></span>  | <span data-ttu-id="d5cb4-126">string</span><span class="sxs-lookup"><span data-stu-id="d5cb4-126">string</span></span>  | <span data-ttu-id="d5cb4-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d5cb4-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d5cb4-129">接受</span><span class="sxs-lookup"><span data-stu-id="d5cb4-129">Accept</span></span> | <span data-ttu-id="d5cb4-130">string</span><span class="sxs-lookup"><span data-stu-id="d5cb4-130">string</span></span> | `application/json` | 

## <a name="request-body"></a><span data-ttu-id="d5cb4-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="d5cb4-131">Request body</span></span>
<span data-ttu-id="d5cb4-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d5cb4-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d5cb4-133">响应</span><span class="sxs-lookup"><span data-stu-id="d5cb4-133">Response</span></span>

<span data-ttu-id="d5cb4-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [onenoteOperation](../resources/onenoteoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d5cb4-134">If successful, this method returns a `200 OK` response code and [onenoteOperation](../resources/onenoteoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d5cb4-135">示例</span><span class="sxs-lookup"><span data-stu-id="d5cb4-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d5cb4-136">请求</span><span class="sxs-lookup"><span data-stu-id="d5cb4-136">Request</span></span>
<span data-ttu-id="d5cb4-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d5cb4-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_onenoteoperation"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/operations/{id}
```
##### <a name="response"></a><span data-ttu-id="d5cb4-138">响应</span><span class="sxs-lookup"><span data-stu-id="d5cb4-138">Response</span></span>
<span data-ttu-id="d5cb4-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d5cb4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteOperation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "id": "id-value",
  "status": "status-value",
  "createdDateTime": "2016-10-19T10:37:00Z",
  "lastActionDateTime": "2016-10-19T10:37:00Z",
  "resourceLocation": "resourceLocation-value",
  "resourceId": "resourceId-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get onenoteOperation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
