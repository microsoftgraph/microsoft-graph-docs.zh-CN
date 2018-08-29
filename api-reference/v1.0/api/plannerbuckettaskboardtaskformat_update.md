# <a name="update-plannerbuckettaskboardtaskformat"></a><span data-ttu-id="c2990-101">更新 plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="c2990-101">Update plannerBucketTaskBoardTaskFormat</span></span>

<span data-ttu-id="c2990-102">更新 **plannerBucketTaskBoardTaskFormat** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c2990-102">Update the properties of **plannerBucketTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c2990-103">权限</span><span class="sxs-lookup"><span data-stu-id="c2990-103">Permissions</span></span>
<span data-ttu-id="c2990-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="c2990-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c2990-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="c2990-106">Permission type</span></span>      | <span data-ttu-id="c2990-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c2990-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2990-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c2990-108">Delegated (work or school account)</span></span> | <span data-ttu-id="c2990-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2990-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c2990-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c2990-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2990-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="c2990-111">Not supported.</span></span>    |
|<span data-ttu-id="c2990-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="c2990-112">Application</span></span> | <span data-ttu-id="c2990-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="c2990-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c2990-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c2990-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/{id}/bucketTaskBoardFormat
```
## <a name="optional-request-headers"></a><span data-ttu-id="c2990-115">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="c2990-115">Optional request headers</span></span>
| <span data-ttu-id="c2990-116">名称</span><span class="sxs-lookup"><span data-stu-id="c2990-116">Name</span></span>       | <span data-ttu-id="c2990-117">说明</span><span class="sxs-lookup"><span data-stu-id="c2990-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="c2990-118">授权</span><span class="sxs-lookup"><span data-stu-id="c2990-118">Authorization</span></span>  | <span data-ttu-id="c2990-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c2990-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c2990-121">If-Match</span><span class="sxs-lookup"><span data-stu-id="c2990-121">If-Match</span></span>  | <span data-ttu-id="c2990-p103">要更新的 **plannerBucketTaskBoardTaskFormat** 的上次已知 ETag 值。必需。</span><span class="sxs-lookup"><span data-stu-id="c2990-p103">Last known ETag value for the **plannerBucketTaskBoardTaskFormat** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2990-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="c2990-124">Request body</span></span>
<span data-ttu-id="c2990-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="c2990-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c2990-128">属性</span><span class="sxs-lookup"><span data-stu-id="c2990-128">Property</span></span>     | <span data-ttu-id="c2990-129">类型</span><span class="sxs-lookup"><span data-stu-id="c2990-129">Type</span></span>   |<span data-ttu-id="c2990-130">说明</span><span class="sxs-lookup"><span data-stu-id="c2990-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c2990-131">orderHint</span><span class="sxs-lookup"><span data-stu-id="c2990-131">orderHint</span></span>|<span data-ttu-id="c2990-132">String</span><span class="sxs-lookup"><span data-stu-id="c2990-132">String</span></span>|<span data-ttu-id="c2990-p105">用于为任务板存储桶视图中的任务进行排序的提示。[此处](../resources/planner_order_hint_format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="c2990-p105">Hint used to order tasks in the Bucket view of the Task Board. The format is defined as outlined [here](../resources/planner_order_hint_format.md).</span></span>|

## <a name="response"></a><span data-ttu-id="c2990-135">响应</span><span class="sxs-lookup"><span data-stu-id="c2990-135">Response</span></span>

<span data-ttu-id="c2990-136">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c2990-136">If successful, this method returns a `200 OK` response code and updated [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="c2990-p106">此方法可以返回任何 [HTTP 状态代码](../../../concepts/errors.md)。应用应当为此方法处理的最常见的错误为 400、403、404、409 和 412 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner_overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="c2990-p106">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="c2990-140">示例</span><span class="sxs-lookup"><span data-stu-id="c2990-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c2990-141">请求</span><span class="sxs-lookup"><span data-stu-id="c2990-141">Request</span></span>
<span data-ttu-id="c2990-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c2990-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannerbuckettaskboardtaskformat"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/tasks/{task-id}/bucketTaskBoardFormat
Content-type: application/json
Content-length: 34
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "orderHint": "A6673H Ejkl!"
}
```
##### <a name="response"></a><span data-ttu-id="c2990-143">响应</span><span class="sxs-lookup"><span data-stu-id="c2990-143">Response</span></span>
<span data-ttu-id="c2990-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c2990-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucketTaskBoardTaskFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 68

{
  "id": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR",
  "orderHint": "C3665D"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update plannerbuckettaskboardtaskformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->