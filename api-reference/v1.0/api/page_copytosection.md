# <a name="page-copytosection"></a><span data-ttu-id="acb0c-101">page: copyToSection</span><span class="sxs-lookup"><span data-stu-id="acb0c-101">page: copyToSection</span></span>
<span data-ttu-id="acb0c-102">将页面复制到特定分区。</span><span class="sxs-lookup"><span data-stu-id="acb0c-102">Copies a page to a specific section.</span></span>

<span data-ttu-id="acb0c-103">对于 Copy 操作，请遵循异步调用模式：首先调用 Copy 操作，然后轮询该操作终结点获取结果。</span><span class="sxs-lookup"><span data-stu-id="acb0c-103">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="acb0c-104">权限</span><span class="sxs-lookup"><span data-stu-id="acb0c-104">Permissions</span></span>
<span data-ttu-id="acb0c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="acb0c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="acb0c-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="acb0c-107">Permission type</span></span>      | <span data-ttu-id="acb0c-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="acb0c-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="acb0c-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="acb0c-109">Delegated (work or school account)</span></span> | <span data-ttu-id="acb0c-110">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="acb0c-110">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="acb0c-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="acb0c-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="acb0c-112">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="acb0c-112">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="acb0c-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="acb0c-113">Application</span></span> | <span data-ttu-id="acb0c-114">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="acb0c-114">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="acb0c-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="acb0c-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/pages/{id}/copyToSection
POST /users/{id | userPrincipalName}/onenote/pages/{id}/copyToSection
POST /groups/{id}/onenote/pages/{id}/copyToSection
```
## <a name="request-headers"></a><span data-ttu-id="acb0c-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="acb0c-116">Request headers</span></span>
| <span data-ttu-id="acb0c-117">名称</span><span class="sxs-lookup"><span data-stu-id="acb0c-117">Name</span></span>       | <span data-ttu-id="acb0c-118">类型</span><span class="sxs-lookup"><span data-stu-id="acb0c-118">Type</span></span> | <span data-ttu-id="acb0c-119">说明</span><span class="sxs-lookup"><span data-stu-id="acb0c-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="acb0c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="acb0c-120">Authorization</span></span>  | <span data-ttu-id="acb0c-121">string</span><span class="sxs-lookup"><span data-stu-id="acb0c-121">string</span></span>  | <span data-ttu-id="acb0c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="acb0c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="acb0c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="acb0c-124">Content-Type</span></span> | <span data-ttu-id="acb0c-125">string</span><span class="sxs-lookup"><span data-stu-id="acb0c-125">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="acb0c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="acb0c-126">Request body</span></span>
<span data-ttu-id="acb0c-127">在请求正文中，提供包含操作所需参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="acb0c-127">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="acb0c-128">参数</span><span class="sxs-lookup"><span data-stu-id="acb0c-128">Parameter</span></span>    | <span data-ttu-id="acb0c-129">类型</span><span class="sxs-lookup"><span data-stu-id="acb0c-129">Type</span></span>   |<span data-ttu-id="acb0c-130">说明</span><span class="sxs-lookup"><span data-stu-id="acb0c-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="acb0c-131">groupId</span><span class="sxs-lookup"><span data-stu-id="acb0c-131">groupId</span></span>|<span data-ttu-id="acb0c-132">字符串</span><span class="sxs-lookup"><span data-stu-id="acb0c-132">String</span></span>|<span data-ttu-id="acb0c-p103">要复制到的组的 ID。仅在复制到 Office 365 组时使用。</span><span class="sxs-lookup"><span data-stu-id="acb0c-p103">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="acb0c-135">id</span><span class="sxs-lookup"><span data-stu-id="acb0c-135">id</span></span>|<span data-ttu-id="acb0c-136">String</span><span class="sxs-lookup"><span data-stu-id="acb0c-136">String</span></span>|<span data-ttu-id="acb0c-p104">必需。目标分区的 ID。</span><span class="sxs-lookup"><span data-stu-id="acb0c-p104">Required. The id of the destination section.</span></span>|

## <a name="response"></a><span data-ttu-id="acb0c-139">响应</span><span class="sxs-lookup"><span data-stu-id="acb0c-139">Response</span></span>

<span data-ttu-id="acb0c-p105">如果成功，此方法返回 `202 Accepted` 响应代码和 `Operation-Location` 标头。轮询 Operation-Location 终结点以[获取复制操作的状态](onenoteoperation_get.md)。</span><span class="sxs-lookup"><span data-stu-id="acb0c-p105">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation_get.md).</span></span>

## <a name="example"></a><span data-ttu-id="acb0c-142">示例</span><span class="sxs-lookup"><span data-stu-id="acb0c-142">Example</span></span>
<span data-ttu-id="acb0c-143">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="acb0c-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="acb0c-144">请求</span><span class="sxs-lookup"><span data-stu-id="acb0c-144">Request</span></span>
<span data-ttu-id="acb0c-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="acb0c-145">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="acb0c-146">响应</span><span class="sxs-lookup"><span data-stu-id="acb0c-146">Response</span></span>
<span data-ttu-id="acb0c-147">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="acb0c-147">Here is an example of the response.</span></span>
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