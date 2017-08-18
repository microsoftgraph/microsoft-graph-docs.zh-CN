# <a name="notebook-copynotebook"></a><span data-ttu-id="429df-101">notebook: copyNotebook</span><span class="sxs-lookup"><span data-stu-id="429df-101">notebook: copyNotebook</span></span>
<span data-ttu-id="429df-p101">将笔记本复制到目标文档库中的 Notebooks 文件夹。如果该文件夹不存在，则将创建该文件夹。</span><span class="sxs-lookup"><span data-stu-id="429df-p101">Copies a notebook to the Notebooks folder in the destination Documents library. The folder is created if it doesn't exist.</span></span>

<span data-ttu-id="429df-104">对于 Copy 操作，请遵循异步调用模式：首先调用 Copy 操作，然后轮询该操作终结点获取结果。</span><span class="sxs-lookup"><span data-stu-id="429df-104">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="429df-105">先决条件</span><span class="sxs-lookup"><span data-stu-id="429df-105">Prerequisites</span></span>
<span data-ttu-id="429df-106">要执行此 API，需要以下**范围**之一：</span><span class="sxs-lookup"><span data-stu-id="429df-106">One of the following **scopes** is required to execute this API:</span></span>   

<span data-ttu-id="429df-107">Notes.Create、Notes.ReadWrite 或 Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="429df-107">Notes.Create, Notes.ReadWrite, or Notes.ReadWrite.All</span></span> 

## <a name="http-request"></a><span data-ttu-id="429df-108">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="429df-108">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/copyNotebook
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/copyNotebook
POST /groups/{id}/onenote/notebooks/{id}/copyNotebook
```
## <a name="request-headers"></a><span data-ttu-id="429df-109">请求标头</span><span class="sxs-lookup"><span data-stu-id="429df-109">Request headers</span></span>
| <span data-ttu-id="429df-110">名称</span><span class="sxs-lookup"><span data-stu-id="429df-110">Name</span></span>       | <span data-ttu-id="429df-111">类型</span><span class="sxs-lookup"><span data-stu-id="429df-111">Type</span></span> | <span data-ttu-id="429df-112">说明</span><span class="sxs-lookup"><span data-stu-id="429df-112">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="429df-113">Authorization</span><span class="sxs-lookup"><span data-stu-id="429df-113">Authorization</span></span>  | <span data-ttu-id="429df-114">string</span><span class="sxs-lookup"><span data-stu-id="429df-114">string</span></span>  | <span data-ttu-id="429df-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="429df-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="429df-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="429df-117">Content-Type</span></span> | <span data-ttu-id="429df-118">string</span><span class="sxs-lookup"><span data-stu-id="429df-118">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="429df-119">请求正文</span><span class="sxs-lookup"><span data-stu-id="429df-119">Request body</span></span>
<span data-ttu-id="429df-p103">在请求正文中，提供包含操作所需参数的 JSON 对象。如果无需任何参数，则可以发送空的正文。</span><span class="sxs-lookup"><span data-stu-id="429df-p103">In the request body, provide a JSON object that contains the parameters that your operation needs. It's okay to send an empty body if none are needed.</span></span>

| <span data-ttu-id="429df-122">参数</span><span class="sxs-lookup"><span data-stu-id="429df-122">Parameter</span></span>    | <span data-ttu-id="429df-123">类型</span><span class="sxs-lookup"><span data-stu-id="429df-123">Type</span></span>   |<span data-ttu-id="429df-124">说明</span><span class="sxs-lookup"><span data-stu-id="429df-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="429df-125">groupId</span><span class="sxs-lookup"><span data-stu-id="429df-125">groupId</span></span>|<span data-ttu-id="429df-126">字符串</span><span class="sxs-lookup"><span data-stu-id="429df-126">String</span></span>|<span data-ttu-id="429df-p104">要复制到的组的 ID。仅在复制到 Office 365 组时使用。</span><span class="sxs-lookup"><span data-stu-id="429df-p104">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="429df-129">renameAs</span><span class="sxs-lookup"><span data-stu-id="429df-129">renameAs</span></span>|<span data-ttu-id="429df-130">字符串</span><span class="sxs-lookup"><span data-stu-id="429df-130">String</span></span>|<span data-ttu-id="429df-p105">副本的名称。默认为现有项的名称。</span><span class="sxs-lookup"><span data-stu-id="429df-p105">The name of the copy. Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="429df-133">响应</span><span class="sxs-lookup"><span data-stu-id="429df-133">Response</span></span>

<span data-ttu-id="429df-p106">如果成功，此方法返回 `202 Accepted` 响应代码和 `Operation-Location` 标头。轮询 Operation-Location 终结点以[获取复制操作的状态](onenoteOperation_get.md)。</span><span class="sxs-lookup"><span data-stu-id="429df-p106">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteOperation_get.md).</span></span>

## <a name="example"></a><span data-ttu-id="429df-136">示例</span><span class="sxs-lookup"><span data-stu-id="429df-136">Example</span></span>
<span data-ttu-id="429df-137">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="429df-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="429df-138">请求</span><span class="sxs-lookup"><span data-stu-id="429df-138">Request</span></span>
<span data-ttu-id="429df-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="429df-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "notebook_copynotebook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/copyNotebook
Content-type: application/json
Content-length: 108

{
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```

##### <a name="response"></a><span data-ttu-id="429df-140">响应</span><span class="sxs-lookup"><span data-stu-id="429df-140">Response</span></span>
<span data-ttu-id="429df-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="429df-141">Here is an example of the response.</span></span>
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
  "description": "notebook: copyNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
