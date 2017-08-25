# <a name="section-copytosectiongroup"></a><span data-ttu-id="673c4-101">section: copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="673c4-101">section: copyToSectionGroup</span></span>
<span data-ttu-id="673c4-102">将分区复制到特定分区组。</span><span class="sxs-lookup"><span data-stu-id="673c4-102">Copies a section to a specific section group.</span></span>

<span data-ttu-id="673c4-103">对于 Copy 操作，请遵循异步调用模式：首先调用 Copy 操作，然后轮询该操作终结点获取结果。</span><span class="sxs-lookup"><span data-stu-id="673c4-103">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="673c4-104">权限</span><span class="sxs-lookup"><span data-stu-id="673c4-104">Permissions</span></span>
<span data-ttu-id="673c4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="673c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="673c4-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="673c4-107">Permission type</span></span>      | <span data-ttu-id="673c4-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="673c4-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="673c4-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="673c4-109">Delegated (work or school account)</span></span> | <span data-ttu-id="673c4-110">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="673c4-110">Notes.Create, Notes.ReadWrite, or Notes.ReadWrite.All</span></span>    | 
|<span data-ttu-id="673c4-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="673c4-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="673c4-112">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="673c4-112">Notes.Create, Notes.ReadWrite, or Notes.ReadWrite.All</span></span>    | 
|<span data-ttu-id="673c4-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="673c4-113">Application</span></span> | <span data-ttu-id="673c4-114">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="673c4-114">Notes.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="673c4-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="673c4-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToSectionGroup
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToSectionGroup
POST /groups/{id}/onenote/sections/{id}/copyToSectionGroup
```
## <a name="request-headers"></a><span data-ttu-id="673c4-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="673c4-116">Request headers</span></span>
| <span data-ttu-id="673c4-117">名称</span><span class="sxs-lookup"><span data-stu-id="673c4-117">Name</span></span>       | <span data-ttu-id="673c4-118">类型</span><span class="sxs-lookup"><span data-stu-id="673c4-118">Type</span></span> | <span data-ttu-id="673c4-119">说明</span><span class="sxs-lookup"><span data-stu-id="673c4-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="673c4-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="673c4-120">Authorization</span></span>  | <span data-ttu-id="673c4-121">string</span><span class="sxs-lookup"><span data-stu-id="673c4-121">string</span></span>  | <span data-ttu-id="673c4-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="673c4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="673c4-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="673c4-124">Content-Type</span></span> | <span data-ttu-id="673c4-125">string</span><span class="sxs-lookup"><span data-stu-id="673c4-125">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="673c4-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="673c4-126">Request body</span></span>
<span data-ttu-id="673c4-127">在请求正文中，提供包含操作所需参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="673c4-127">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="673c4-128">参数</span><span class="sxs-lookup"><span data-stu-id="673c4-128">Parameter</span></span>    | <span data-ttu-id="673c4-129">类型</span><span class="sxs-lookup"><span data-stu-id="673c4-129">Type</span></span>   |<span data-ttu-id="673c4-130">说明</span><span class="sxs-lookup"><span data-stu-id="673c4-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="673c4-131">groupId</span><span class="sxs-lookup"><span data-stu-id="673c4-131">groupId</span></span>|<span data-ttu-id="673c4-132">字符串</span><span class="sxs-lookup"><span data-stu-id="673c4-132">String</span></span>|<span data-ttu-id="673c4-p103">要复制到的组的 ID。仅在复制到 Office 365 组时使用。</span><span class="sxs-lookup"><span data-stu-id="673c4-p103">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="673c4-135">id</span><span class="sxs-lookup"><span data-stu-id="673c4-135">id</span></span>|<span data-ttu-id="673c4-136">字符串</span><span class="sxs-lookup"><span data-stu-id="673c4-136">String</span></span>|<span data-ttu-id="673c4-p104">必需。目标分区组的 ID。</span><span class="sxs-lookup"><span data-stu-id="673c4-p104">Required. The id of the destination section group.</span></span> |
|<span data-ttu-id="673c4-139">renameAs</span><span class="sxs-lookup"><span data-stu-id="673c4-139">renameAs</span></span>|<span data-ttu-id="673c4-140">字符串</span><span class="sxs-lookup"><span data-stu-id="673c4-140">String</span></span>|<span data-ttu-id="673c4-p105">副本的名称。默认为现有项的名称。</span><span class="sxs-lookup"><span data-stu-id="673c4-p105">The name of the copy. Defaults to the name of the existing item.</span></span> |

<!--groupId missing-->
<!--|siteCollectionId|String||
|siteId|String||-->

## <a name="response"></a><span data-ttu-id="673c4-143">响应</span><span class="sxs-lookup"><span data-stu-id="673c4-143">Response</span></span>

<span data-ttu-id="673c4-p106">如果成功，此方法返回 `202 Accepted` 响应代码和 `Operation-Location` 标头。轮询 Operation-Location 终结点以[获取复制操作的状态](onenoteoperation_get.md)。</span><span class="sxs-lookup"><span data-stu-id="673c4-p106">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation_get.md).</span></span>

## <a name="example"></a><span data-ttu-id="673c4-146">示例</span><span class="sxs-lookup"><span data-stu-id="673c4-146">Example</span></span>
<span data-ttu-id="673c4-147">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="673c4-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="673c4-148">请求</span><span class="sxs-lookup"><span data-stu-id="673c4-148">Request</span></span>
<span data-ttu-id="673c4-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="673c4-149">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="673c4-150">响应</span><span class="sxs-lookup"><span data-stu-id="673c4-150">Response</span></span>
<span data-ttu-id="673c4-151">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="673c4-151">Here is an example of the response.</span></span>
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