# <a name="section-copytosectiongroup"></a><span data-ttu-id="15a00-101">section: copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="15a00-101">section: copyToSectionGroup</span></span>
<span data-ttu-id="15a00-102">将分区复制到特定分区组。</span><span class="sxs-lookup"><span data-stu-id="15a00-102">Copies a section to a specific section group.</span></span>

<span data-ttu-id="15a00-103">对于 Copy 操作，请遵循异步调用模式：首先调用 Copy 操作，然后轮询该操作终结点获取结果。</span><span class="sxs-lookup"><span data-stu-id="15a00-103">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="15a00-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="15a00-104">Prerequisites</span></span>
<span data-ttu-id="15a00-105">要执行此 API，需要以下**范围**之一：</span><span class="sxs-lookup"><span data-stu-id="15a00-105">One of the following **scopes** is required to execute this API:</span></span>   

<span data-ttu-id="15a00-106">Notes.Create、Notes.ReadWrite 或 Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15a00-106">Notes.Create, Notes.ReadWrite, or Notes.ReadWrite.All</span></span> 

## <a name="http-request"></a><span data-ttu-id="15a00-107">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="15a00-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToSectionGroup
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToSectionGroup
POST /groups/{id}/onenote/sections/{id}/copyToSectionGroup
```
## <a name="request-headers"></a><span data-ttu-id="15a00-108">请求标头</span><span class="sxs-lookup"><span data-stu-id="15a00-108">Request headers</span></span>
| <span data-ttu-id="15a00-109">名称</span><span class="sxs-lookup"><span data-stu-id="15a00-109">Name</span></span>       | <span data-ttu-id="15a00-110">类型</span><span class="sxs-lookup"><span data-stu-id="15a00-110">Type</span></span> | <span data-ttu-id="15a00-111">说明</span><span class="sxs-lookup"><span data-stu-id="15a00-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="15a00-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="15a00-112">Authorization</span></span>  | <span data-ttu-id="15a00-113">string</span><span class="sxs-lookup"><span data-stu-id="15a00-113">string</span></span>  | <span data-ttu-id="15a00-p101">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="15a00-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="15a00-116">Content-Type</span><span class="sxs-lookup"><span data-stu-id="15a00-116">Content-Type</span></span> | <span data-ttu-id="15a00-117">string</span><span class="sxs-lookup"><span data-stu-id="15a00-117">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="15a00-118">请求正文</span><span class="sxs-lookup"><span data-stu-id="15a00-118">Request body</span></span>
<span data-ttu-id="15a00-119">在请求正文中，提供包含操作所需参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="15a00-119">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="15a00-120">参数</span><span class="sxs-lookup"><span data-stu-id="15a00-120">Parameter</span></span>    | <span data-ttu-id="15a00-121">类型</span><span class="sxs-lookup"><span data-stu-id="15a00-121">Type</span></span>   |<span data-ttu-id="15a00-122">说明</span><span class="sxs-lookup"><span data-stu-id="15a00-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="15a00-123">groupId</span><span class="sxs-lookup"><span data-stu-id="15a00-123">groupId</span></span>|<span data-ttu-id="15a00-124">字符串</span><span class="sxs-lookup"><span data-stu-id="15a00-124">String</span></span>|<span data-ttu-id="15a00-p102">要复制到的组的 ID。仅在复制到 Office 365 组时使用。</span><span class="sxs-lookup"><span data-stu-id="15a00-p102">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="15a00-127">id</span><span class="sxs-lookup"><span data-stu-id="15a00-127">id</span></span>|<span data-ttu-id="15a00-128">字符串</span><span class="sxs-lookup"><span data-stu-id="15a00-128">String</span></span>|<span data-ttu-id="15a00-p103">必需。目标分区组的 ID。</span><span class="sxs-lookup"><span data-stu-id="15a00-p103">Required. The id of the destination section group.</span></span> |
|<span data-ttu-id="15a00-131">renameAs</span><span class="sxs-lookup"><span data-stu-id="15a00-131">renameAs</span></span>|<span data-ttu-id="15a00-132">字符串</span><span class="sxs-lookup"><span data-stu-id="15a00-132">String</span></span>|<span data-ttu-id="15a00-p104">副本的名称。默认为现有项的名称。</span><span class="sxs-lookup"><span data-stu-id="15a00-p104">The name of the copy. Defaults to the name of the existing item.</span></span> |

<!--groupId missing-->
<!--|siteCollectionId|String||
|siteId|String||-->

## <a name="response"></a><span data-ttu-id="15a00-135">响应</span><span class="sxs-lookup"><span data-stu-id="15a00-135">Response</span></span>

<span data-ttu-id="15a00-p105">如果成功，此方法返回 `202 Accepted` 响应代码和 `Operation-Location` 标头。轮询 Operation-Location 终结点以[获取复制操作的状态](onenoteoperation_get.md)。</span><span class="sxs-lookup"><span data-stu-id="15a00-p105">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation_get.md).</span></span>

## <a name="example"></a><span data-ttu-id="15a00-138">示例</span><span class="sxs-lookup"><span data-stu-id="15a00-138">Example</span></span>
<span data-ttu-id="15a00-139">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="15a00-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="15a00-140">请求</span><span class="sxs-lookup"><span data-stu-id="15a00-140">Request</span></span>
<span data-ttu-id="15a00-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="15a00-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "section_copytosectiongroup"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/sections/{id}/copyToSectionGroup
Content-type: application/json
Content-length: 84

{
  "id": "id-value",
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```

##### <a name="response"></a><span data-ttu-id="15a00-142">响应</span><span class="sxs-lookup"><span data-stu-id="15a00-142">Response</span></span>
<span data-ttu-id="15a00-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="15a00-143">Here is an example of the response.</span></span>
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
  "description": "section: copyToSectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->