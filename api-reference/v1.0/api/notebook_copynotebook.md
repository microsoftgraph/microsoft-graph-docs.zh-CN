# <a name="notebook-copynotebook"></a><span data-ttu-id="43bfa-101">notebook: copyNotebook</span><span class="sxs-lookup"><span data-stu-id="43bfa-101">notebook: copyNotebook</span></span>
<span data-ttu-id="43bfa-p101">将笔记本复制到目标文档库中的 Notebooks 文件夹。如果该文件夹不存在，则将创建该文件夹。</span><span class="sxs-lookup"><span data-stu-id="43bfa-p101">Copies a notebook to the Notebooks folder in the destination Documents library. The folder is created if it doesn't exist.</span></span>

<span data-ttu-id="43bfa-104">对于 Copy 操作，请遵循异步调用模式：首先调用 Copy 操作，然后轮询该操作终结点获取结果。</span><span class="sxs-lookup"><span data-stu-id="43bfa-104">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="43bfa-105">权限</span><span class="sxs-lookup"><span data-stu-id="43bfa-105">Permissions</span></span>
<span data-ttu-id="43bfa-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="43bfa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="43bfa-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="43bfa-108">Permission type</span></span>      | <span data-ttu-id="43bfa-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="43bfa-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="43bfa-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="43bfa-110">Delegated (work or school account)</span></span> | <span data-ttu-id="43bfa-111">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43bfa-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="43bfa-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="43bfa-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="43bfa-113">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="43bfa-113">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="43bfa-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="43bfa-114">Application</span></span> | <span data-ttu-id="43bfa-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43bfa-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="43bfa-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="43bfa-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/copyNotebook
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/copyNotebook
POST /groups/{id}/onenote/notebooks/{id}/copyNotebook
```
## <a name="request-headers"></a><span data-ttu-id="43bfa-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="43bfa-117">Request headers</span></span>
| <span data-ttu-id="43bfa-118">名称</span><span class="sxs-lookup"><span data-stu-id="43bfa-118">Name</span></span>       | <span data-ttu-id="43bfa-119">类型</span><span class="sxs-lookup"><span data-stu-id="43bfa-119">Type</span></span> | <span data-ttu-id="43bfa-120">说明</span><span class="sxs-lookup"><span data-stu-id="43bfa-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="43bfa-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="43bfa-121">Authorization</span></span>  | <span data-ttu-id="43bfa-122">string</span><span class="sxs-lookup"><span data-stu-id="43bfa-122">string</span></span>  | <span data-ttu-id="43bfa-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="43bfa-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="43bfa-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="43bfa-125">Content-Type</span></span> | <span data-ttu-id="43bfa-126">string</span><span class="sxs-lookup"><span data-stu-id="43bfa-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="43bfa-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="43bfa-127">Request body</span></span>
<span data-ttu-id="43bfa-p104">在请求正文中，提供包含操作所需参数的 JSON 对象。如果无需任何参数，则可以发送空的正文。</span><span class="sxs-lookup"><span data-stu-id="43bfa-p104">In the request body, provide a JSON object that contains the parameters that your operation needs. It's okay to send an empty body if none are needed.</span></span>

| <span data-ttu-id="43bfa-130">参数</span><span class="sxs-lookup"><span data-stu-id="43bfa-130">Parameter</span></span>    | <span data-ttu-id="43bfa-131">类型</span><span class="sxs-lookup"><span data-stu-id="43bfa-131">Type</span></span>   |<span data-ttu-id="43bfa-132">说明</span><span class="sxs-lookup"><span data-stu-id="43bfa-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="43bfa-133">groupId</span><span class="sxs-lookup"><span data-stu-id="43bfa-133">groupId</span></span>|<span data-ttu-id="43bfa-134">字符串</span><span class="sxs-lookup"><span data-stu-id="43bfa-134">String</span></span>|<span data-ttu-id="43bfa-p105">要复制到的组的 ID。仅在复制到 Office 365 组时使用。</span><span class="sxs-lookup"><span data-stu-id="43bfa-p105">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="43bfa-137">renameAs</span><span class="sxs-lookup"><span data-stu-id="43bfa-137">renameAs</span></span>|<span data-ttu-id="43bfa-138">字符串</span><span class="sxs-lookup"><span data-stu-id="43bfa-138">String</span></span>|<span data-ttu-id="43bfa-p106">副本的名称。默认为现有项的名称。</span><span class="sxs-lookup"><span data-stu-id="43bfa-p106">The name of the copy. Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="43bfa-141">响应</span><span class="sxs-lookup"><span data-stu-id="43bfa-141">Response</span></span>

<span data-ttu-id="43bfa-p107">如果成功，此方法返回 `202 Accepted` 响应代码和 `Operation-Location` 标头。轮询 Operation-Location 终结点以[获取复制操作的状态](onenoteOperation_get.md)。</span><span class="sxs-lookup"><span data-stu-id="43bfa-p107">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteOperation_get.md).</span></span>

## <a name="example"></a><span data-ttu-id="43bfa-144">示例</span><span class="sxs-lookup"><span data-stu-id="43bfa-144">Example</span></span>
<span data-ttu-id="43bfa-145">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="43bfa-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="43bfa-146">请求</span><span class="sxs-lookup"><span data-stu-id="43bfa-146">Request</span></span>
<span data-ttu-id="43bfa-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="43bfa-147">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="43bfa-148">响应</span><span class="sxs-lookup"><span data-stu-id="43bfa-148">Response</span></span>
<span data-ttu-id="43bfa-149">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="43bfa-149">Here is an example of the response.</span></span>
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
