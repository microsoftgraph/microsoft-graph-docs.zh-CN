# <a name="page-copytosection"></a><span data-ttu-id="aa705-101">page: copyToSection</span><span class="sxs-lookup"><span data-stu-id="aa705-101">page: copyToSection</span></span>
<span data-ttu-id="aa705-102">将页面复制到特定分区。</span><span class="sxs-lookup"><span data-stu-id="aa705-102">Copies a page to a specific section.</span></span>

<span data-ttu-id="aa705-103">对于 Copy 操作，请遵循异步调用模式：首先调用 Copy 操作，然后轮询该操作终结点获取结果。</span><span class="sxs-lookup"><span data-stu-id="aa705-103">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aa705-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="aa705-104">Prerequisites</span></span>
<span data-ttu-id="aa705-105">要执行此 API，需要以下**范围**之一：</span><span class="sxs-lookup"><span data-stu-id="aa705-105">One of the following **scopes** is required to execute this API:</span></span>   

<span data-ttu-id="aa705-106">Notes.Create、Notes.ReadWrite 或 Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa705-106">Notes.Create, Notes.ReadWrite, or Notes.ReadWrite.All</span></span>  

## <a name="http-request"></a><span data-ttu-id="aa705-107">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aa705-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/pages/{id}/copyToSection
POST /users/{id | userPrincipalName}/onenote/pages/{id}/copyToSection
POST /groups/{id}/onenote/pages/{id}/copyToSection
```
## <a name="request-headers"></a><span data-ttu-id="aa705-108">请求标头</span><span class="sxs-lookup"><span data-stu-id="aa705-108">Request headers</span></span>
| <span data-ttu-id="aa705-109">名称</span><span class="sxs-lookup"><span data-stu-id="aa705-109">Name</span></span>       | <span data-ttu-id="aa705-110">类型</span><span class="sxs-lookup"><span data-stu-id="aa705-110">Type</span></span> | <span data-ttu-id="aa705-111">说明</span><span class="sxs-lookup"><span data-stu-id="aa705-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="aa705-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa705-112">Authorization</span></span>  | <span data-ttu-id="aa705-113">string</span><span class="sxs-lookup"><span data-stu-id="aa705-113">string</span></span>  | <span data-ttu-id="aa705-p101">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="aa705-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="aa705-116">Content-Type</span><span class="sxs-lookup"><span data-stu-id="aa705-116">Content-Type</span></span> | <span data-ttu-id="aa705-117">string</span><span class="sxs-lookup"><span data-stu-id="aa705-117">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="aa705-118">请求正文</span><span class="sxs-lookup"><span data-stu-id="aa705-118">Request body</span></span>
<span data-ttu-id="aa705-119">在请求正文中，提供包含操作所需参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="aa705-119">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="aa705-120">参数</span><span class="sxs-lookup"><span data-stu-id="aa705-120">Parameter</span></span>    | <span data-ttu-id="aa705-121">类型</span><span class="sxs-lookup"><span data-stu-id="aa705-121">Type</span></span>   |<span data-ttu-id="aa705-122">说明</span><span class="sxs-lookup"><span data-stu-id="aa705-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aa705-123">groupId</span><span class="sxs-lookup"><span data-stu-id="aa705-123">groupId</span></span>|<span data-ttu-id="aa705-124">字符串</span><span class="sxs-lookup"><span data-stu-id="aa705-124">String</span></span>|<span data-ttu-id="aa705-p102">要复制到的组的 ID。仅在复制到 Office 365 组时使用。</span><span class="sxs-lookup"><span data-stu-id="aa705-p102">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="aa705-127">id</span><span class="sxs-lookup"><span data-stu-id="aa705-127">id</span></span>|<span data-ttu-id="aa705-128">String</span><span class="sxs-lookup"><span data-stu-id="aa705-128">String</span></span>|<span data-ttu-id="aa705-p103">必需。目标分区的 ID。</span><span class="sxs-lookup"><span data-stu-id="aa705-p103">Required. The id of the destination section.</span></span>|

## <a name="response"></a><span data-ttu-id="aa705-131">响应</span><span class="sxs-lookup"><span data-stu-id="aa705-131">Response</span></span>

<span data-ttu-id="aa705-p104">如果成功，此方法返回 `202 Accepted` 响应代码和 `Operation-Location` 标头。轮询 Operation-Location 终结点以[获取复制操作的状态](onenoteoperation_get.md)。</span><span class="sxs-lookup"><span data-stu-id="aa705-p104">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation_get.md).</span></span>

## <a name="example"></a><span data-ttu-id="aa705-134">示例</span><span class="sxs-lookup"><span data-stu-id="aa705-134">Example</span></span>
<span data-ttu-id="aa705-135">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="aa705-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="aa705-136">请求</span><span class="sxs-lookup"><span data-stu-id="aa705-136">Request</span></span>
<span data-ttu-id="aa705-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="aa705-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "page_copytosection"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/pages/{id}/copyToSection
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "groupId": "groupId-value"
}
```

##### <a name="response"></a><span data-ttu-id="aa705-138">响应</span><span class="sxs-lookup"><span data-stu-id="aa705-138">Response</span></span>
<span data-ttu-id="aa705-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="aa705-139">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteOperation"
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page: copyToSection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->