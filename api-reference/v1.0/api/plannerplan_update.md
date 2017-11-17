# <a name="update-plannerplan"></a><span data-ttu-id="4859d-101">更新 plannerplan</span><span class="sxs-lookup"><span data-stu-id="4859d-101">Update plannerplan</span></span>

<span data-ttu-id="4859d-102">更新 **plannerplan** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4859d-102">Update the properties of **plannerplan** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4859d-103">权限</span><span class="sxs-lookup"><span data-stu-id="4859d-103">Permissions</span></span>
<span data-ttu-id="4859d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="4859d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4859d-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="4859d-106">Permission type</span></span>      | <span data-ttu-id="4859d-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4859d-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4859d-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4859d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="4859d-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4859d-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4859d-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4859d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4859d-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="4859d-111">Not supported.</span></span>    |
|<span data-ttu-id="4859d-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="4859d-112">Application</span></span> | <span data-ttu-id="4859d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="4859d-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4859d-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4859d-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/plans/<id>
```
## <a name="optional-request-headers"></a><span data-ttu-id="4859d-115">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="4859d-115">Optional request headers</span></span>
| <span data-ttu-id="4859d-116">名称</span><span class="sxs-lookup"><span data-stu-id="4859d-116">Name</span></span>       | <span data-ttu-id="4859d-117">说明</span><span class="sxs-lookup"><span data-stu-id="4859d-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="4859d-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="4859d-118">Authorization</span></span>  | <span data-ttu-id="4859d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4859d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4859d-121">If-Match</span><span class="sxs-lookup"><span data-stu-id="4859d-121">If-Match</span></span>  | <span data-ttu-id="4859d-p103">要更新的 plannerPlan 的上次已知 ETag 值。必需。</span><span class="sxs-lookup"><span data-stu-id="4859d-p103">Last known ETag value for the plannerPlan to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4859d-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="4859d-124">Request body</span></span>
<span data-ttu-id="4859d-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="4859d-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4859d-128">属性</span><span class="sxs-lookup"><span data-stu-id="4859d-128">Property</span></span>     | <span data-ttu-id="4859d-129">类型</span><span class="sxs-lookup"><span data-stu-id="4859d-129">Type</span></span>   |<span data-ttu-id="4859d-130">说明</span><span class="sxs-lookup"><span data-stu-id="4859d-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4859d-131">所有者</span><span class="sxs-lookup"><span data-stu-id="4859d-131">owner</span></span>|<span data-ttu-id="4859d-132">字符串</span><span class="sxs-lookup"><span data-stu-id="4859d-132">String</span></span>|<span data-ttu-id="4859d-p105">拥有计划的[组](../resources/group.md)`id`。必须存在有效的组才能设置此字段。设置后，只能由所有者更新此字段。</span><span class="sxs-lookup"><span data-stu-id="4859d-p105">[Group](../resources/group.md) `id` by which the plan is owned. A valid group must exist before this field can be set. Once set, this can only be updated by the owner.</span></span>|
|<span data-ttu-id="4859d-136">title</span><span class="sxs-lookup"><span data-stu-id="4859d-136">title</span></span>|<span data-ttu-id="4859d-137">String</span><span class="sxs-lookup"><span data-stu-id="4859d-137">String</span></span>|<span data-ttu-id="4859d-138">计划的标题。</span><span class="sxs-lookup"><span data-stu-id="4859d-138">Title of the plan.</span></span>|

## <a name="response"></a><span data-ttu-id="4859d-139">响应</span><span class="sxs-lookup"><span data-stu-id="4859d-139">Response</span></span>

<span data-ttu-id="4859d-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [plannerPlan](../resources/plannerplan.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4859d-140">If successful, this method returns a `200 OK` response code and updated [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="4859d-p106">此方法可以返回任何 [HTTP 状态代码](../../../concepts/errors.md)。应用应当为此方法处理的最常见的错误为 400、403、404、409 和 412 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner_overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="4859d-p106">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="4859d-144">示例</span><span class="sxs-lookup"><span data-stu-id="4859d-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4859d-145">请求</span><span class="sxs-lookup"><span data-stu-id="4859d-145">Request</span></span>
<span data-ttu-id="4859d-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4859d-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannerplan"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/plans/xqQg5FS2LkCp935s-FIFm2QAFkHM
Content-type: application/json
Content-length: 29
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "title": "title-value"
}
```
##### <a name="response"></a><span data-ttu-id="4859d-147">响应</span><span class="sxs-lookup"><span data-stu-id="4859d-147">Response</span></span>
<span data-ttu-id="4859d-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4859d-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlan"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 357

{
  "createdBy": {
    "application": {
      "id": "95e27074-6c4a-447a-aa24-9d718a0b86fa"
    },
    "user": {
      "id": "ebf3b108-5234-4e22-b93d-656d7dae5874"
    }
  },
  "createdDateTime": "2015-03-30T18:36:49.2407981Z",
  "owner": "ebf3b108-5234-4e22-b93d-656d7dae5874",
  "title": "title-value",
  "id": "xqQg5FS2LkCp935s-FIFm2QAFkHM"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update plannerplan",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->