# <a name="update-plannerbucket"></a><span data-ttu-id="4ef5f-101">更新 plannerbucket</span><span class="sxs-lookup"><span data-stu-id="4ef5f-101">Update plannerbucket</span></span>

<span data-ttu-id="4ef5f-102">更新 **plannerbucket** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4ef5f-102">Update the properties of **plannerbucket** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4ef5f-103">权限</span><span class="sxs-lookup"><span data-stu-id="4ef5f-103">Permissions</span></span>
<span data-ttu-id="4ef5f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="4ef5f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4ef5f-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="4ef5f-106">Permission type</span></span>      | <span data-ttu-id="4ef5f-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4ef5f-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ef5f-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4ef5f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="4ef5f-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ef5f-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4ef5f-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4ef5f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ef5f-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="4ef5f-111">Not supported.</span></span>    |
|<span data-ttu-id="4ef5f-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="4ef5f-112">Application</span></span> | <span data-ttu-id="4ef5f-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="4ef5f-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4ef5f-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4ef5f-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/buckets/<id>
```
## <a name="optional-request-headers"></a><span data-ttu-id="4ef5f-115">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="4ef5f-115">Optional request headers</span></span>
| <span data-ttu-id="4ef5f-116">名称</span><span class="sxs-lookup"><span data-stu-id="4ef5f-116">Name</span></span>       | <span data-ttu-id="4ef5f-117">说明</span><span class="sxs-lookup"><span data-stu-id="4ef5f-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="4ef5f-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ef5f-118">Authorization</span></span>  | <span data-ttu-id="4ef5f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4ef5f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4ef5f-121">If-Match</span><span class="sxs-lookup"><span data-stu-id="4ef5f-121">If-Match</span></span>  | <span data-ttu-id="4ef5f-p103">要更新的 **plannerBucket** 的上次已知 ETag 值。必需。</span><span class="sxs-lookup"><span data-stu-id="4ef5f-p103">Last known ETag value for the **plannerBucket** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ef5f-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="4ef5f-124">Request body</span></span>
<span data-ttu-id="4ef5f-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="4ef5f-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4ef5f-128">属性</span><span class="sxs-lookup"><span data-stu-id="4ef5f-128">Property</span></span>     | <span data-ttu-id="4ef5f-129">类型</span><span class="sxs-lookup"><span data-stu-id="4ef5f-129">Type</span></span>   |<span data-ttu-id="4ef5f-130">说明</span><span class="sxs-lookup"><span data-stu-id="4ef5f-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4ef5f-131">名称</span><span class="sxs-lookup"><span data-stu-id="4ef5f-131">name</span></span>|<span data-ttu-id="4ef5f-132">String</span><span class="sxs-lookup"><span data-stu-id="4ef5f-132">String</span></span>|<span data-ttu-id="4ef5f-133">存储桶的名称。</span><span class="sxs-lookup"><span data-stu-id="4ef5f-133">Name of the bucket.</span></span>|
|<span data-ttu-id="4ef5f-134">orderHint</span><span class="sxs-lookup"><span data-stu-id="4ef5f-134">orderHint</span></span>|<span data-ttu-id="4ef5f-135">String</span><span class="sxs-lookup"><span data-stu-id="4ef5f-135">String</span></span>|<span data-ttu-id="4ef5f-p105">用于为列表视图中的此类型项目排序的提示。[此处](../resources/planner_order_hint_format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="4ef5f-p105">Hint used to order items of this type in a list view. The format is defined as outlined [here](../resources/planner_order_hint_format.md).</span></span>|
|<span data-ttu-id="4ef5f-138">planId</span><span class="sxs-lookup"><span data-stu-id="4ef5f-138">planId</span></span>|<span data-ttu-id="4ef5f-139">String</span><span class="sxs-lookup"><span data-stu-id="4ef5f-139">String</span></span>|<span data-ttu-id="4ef5f-140">此存储桶所属的计划 id。</span><span class="sxs-lookup"><span data-stu-id="4ef5f-140">Plan id to which the bucket belongs.</span></span>|

## <a name="response"></a><span data-ttu-id="4ef5f-141">响应</span><span class="sxs-lookup"><span data-stu-id="4ef5f-141">Response</span></span>

<span data-ttu-id="4ef5f-142">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [plannerBucket](../resources/plannerbucket.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4ef5f-142">If successful, this method returns a `200 OK` response code and updated [plannerBucket](../resources/plannerbucket.md) object in the response body.</span></span>

<span data-ttu-id="4ef5f-p106">此方法可以返回任何 [HTTP 状态代码](../../../concepts/errors.md)。应用应当为此方法处理的最常见的错误为 400、403、404、409 和 412 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner_overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="4ef5f-p106">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="4ef5f-146">示例</span><span class="sxs-lookup"><span data-stu-id="4ef5f-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4ef5f-147">请求</span><span class="sxs-lookup"><span data-stu-id="4ef5f-147">Request</span></span>
<span data-ttu-id="4ef5f-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4ef5f-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannerbucket"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/buckets/hsOf2dhOJkqyYYZEtdzDe2QAIUCR
Content-type: application/json
Content-length: 27
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "name": "Development"
}
```
##### <a name="response"></a><span data-ttu-id="4ef5f-149">响应</span><span class="sxs-lookup"><span data-stu-id="4ef5f-149">Response</span></span>
<span data-ttu-id="4ef5f-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4ef5f-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucket"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 245

{
  "name": "Development",
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "orderHint": "85752723360752+",
  "id": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update plannerbucket",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->