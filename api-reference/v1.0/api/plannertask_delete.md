# <a name="delete-plannertask"></a><span data-ttu-id="222cb-101">删除 plannerTask</span><span class="sxs-lookup"><span data-stu-id="222cb-101">Delete plannerTask</span></span>

<span data-ttu-id="222cb-102">删除 **plannerTask**。</span><span class="sxs-lookup"><span data-stu-id="222cb-102">Delete **plannerTask**.</span></span>
## <a name="permissions"></a><span data-ttu-id="222cb-103">权限</span><span class="sxs-lookup"><span data-stu-id="222cb-103">Permissions</span></span>
<span data-ttu-id="222cb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="222cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="222cb-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="222cb-106">Permission type</span></span>      | <span data-ttu-id="222cb-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="222cb-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="222cb-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="222cb-108">Delegated (work or school account)</span></span> | <span data-ttu-id="222cb-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="222cb-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="222cb-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="222cb-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="222cb-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="222cb-111">Not supported.</span></span>    |
|<span data-ttu-id="222cb-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="222cb-112">Application</span></span> | <span data-ttu-id="222cb-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="222cb-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="222cb-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="222cb-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /planner/tasks/<id>
```
## <a name="request-headers"></a><span data-ttu-id="222cb-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="222cb-115">Request headers</span></span>
| <span data-ttu-id="222cb-116">名称</span><span class="sxs-lookup"><span data-stu-id="222cb-116">Name</span></span>       | <span data-ttu-id="222cb-117">说明</span><span class="sxs-lookup"><span data-stu-id="222cb-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="222cb-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="222cb-118">Authorization</span></span>  | <span data-ttu-id="222cb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="222cb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="222cb-121">If-Match</span><span class="sxs-lookup"><span data-stu-id="222cb-121">If-Match</span></span>  | <span data-ttu-id="222cb-p103">要删除的 **plannerTask** 的上次已知 ETag 值。必需。</span><span class="sxs-lookup"><span data-stu-id="222cb-p103">Last known ETag value for the **plannerTask** to be deleted. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="222cb-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="222cb-124">Request body</span></span>
<span data-ttu-id="222cb-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="222cb-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="222cb-126">响应</span><span class="sxs-lookup"><span data-stu-id="222cb-126">Response</span></span>

<span data-ttu-id="222cb-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="222cb-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="222cb-p105">此方法可以返回任何 [HTTP 状态代码](../../../concepts/errors.md)。应用应当为此方法处理的最常见的错误为 400、403、404、409 和 412 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner_overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="222cb-p105">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="222cb-132">示例</span><span class="sxs-lookup"><span data-stu-id="222cb-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="222cb-133">请求</span><span class="sxs-lookup"><span data-stu-id="222cb-133">Request</span></span>
<span data-ttu-id="222cb-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="222cb-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_plannertask"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/planner/tasks/<id>
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="
```
##### <a name="response"></a><span data-ttu-id="222cb-135">响应</span><span class="sxs-lookup"><span data-stu-id="222cb-135">Response</span></span>
<span data-ttu-id="222cb-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="222cb-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete plannerTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->