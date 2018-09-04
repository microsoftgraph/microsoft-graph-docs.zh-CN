# <a name="update-charttitle"></a><span data-ttu-id="40dba-101">更新 charttitle</span><span class="sxs-lookup"><span data-stu-id="40dba-101">Update charttitle</span></span>

<span data-ttu-id="40dba-102">更新 charttitle 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="40dba-102">Update the properties of charttitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="40dba-103">权限</span><span class="sxs-lookup"><span data-stu-id="40dba-103">Permissions</span></span>
<span data-ttu-id="40dba-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="40dba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="40dba-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="40dba-106">Permission type</span></span>      | <span data-ttu-id="40dba-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="40dba-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="40dba-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="40dba-108">Delegated (work or school account)</span></span> | <span data-ttu-id="40dba-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="40dba-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="40dba-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="40dba-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40dba-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="40dba-111">Not supported.</span></span>    |
|<span data-ttu-id="40dba-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="40dba-112">Application</span></span> | <span data-ttu-id="40dba-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="40dba-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="40dba-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="40dba-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/title
```
## <a name="optional-request-headers"></a><span data-ttu-id="40dba-115">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="40dba-115">Optional request headers</span></span>
| <span data-ttu-id="40dba-116">名称</span><span class="sxs-lookup"><span data-stu-id="40dba-116">Name</span></span>       | <span data-ttu-id="40dba-117">说明</span><span class="sxs-lookup"><span data-stu-id="40dba-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="40dba-118">授权</span><span class="sxs-lookup"><span data-stu-id="40dba-118">Authorization</span></span>  | <span data-ttu-id="40dba-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="40dba-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="40dba-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="40dba-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="40dba-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="40dba-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="40dba-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="40dba-124">Request body</span></span>
<span data-ttu-id="40dba-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="40dba-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="40dba-128">属性</span><span class="sxs-lookup"><span data-stu-id="40dba-128">Property</span></span>     | <span data-ttu-id="40dba-129">类型</span><span class="sxs-lookup"><span data-stu-id="40dba-129">Type</span></span>   |<span data-ttu-id="40dba-130">说明</span><span class="sxs-lookup"><span data-stu-id="40dba-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="40dba-131">overlay</span><span class="sxs-lookup"><span data-stu-id="40dba-131">overlay</span></span>|<span data-ttu-id="40dba-132">boolean</span><span class="sxs-lookup"><span data-stu-id="40dba-132">boolean</span></span>|<span data-ttu-id="40dba-133">表示图表标题是否将叠加在图表上的布尔值。</span><span class="sxs-lookup"><span data-stu-id="40dba-133">Boolean value representing if the chart title will overlay the chart or not.</span></span>|
|<span data-ttu-id="40dba-134">text</span><span class="sxs-lookup"><span data-stu-id="40dba-134">text</span></span>|<span data-ttu-id="40dba-135">string</span><span class="sxs-lookup"><span data-stu-id="40dba-135">string</span></span>|<span data-ttu-id="40dba-136">表示图表的标题文本。</span><span class="sxs-lookup"><span data-stu-id="40dba-136">Represents the title text of a chart.</span></span>|
|<span data-ttu-id="40dba-137">visible</span><span class="sxs-lookup"><span data-stu-id="40dba-137">visible</span></span>|<span data-ttu-id="40dba-138">boolean</span><span class="sxs-lookup"><span data-stu-id="40dba-138">boolean</span></span>|<span data-ttu-id="40dba-139">表示 chart title 对象的可见性的布尔值。</span><span class="sxs-lookup"><span data-stu-id="40dba-139">A boolean value the represents the visibility of a chart title object.</span></span>|

## <a name="response"></a><span data-ttu-id="40dba-140">响应</span><span class="sxs-lookup"><span data-stu-id="40dba-140">Response</span></span>

<span data-ttu-id="40dba-141">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [WorkbookChartTitle](../resources/charttitle.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="40dba-141">If successful, this method returns a `200 OK` response code and updated [plannerTaskDetails](../resources/charttitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="40dba-142">示例</span><span class="sxs-lookup"><span data-stu-id="40dba-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="40dba-143">请求</span><span class="sxs-lookup"><span data-stu-id="40dba-143">Request</span></span>
<span data-ttu-id="40dba-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="40dba-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_charttitle"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/title
Content-type: application/json
Content-length: 64

{
  "overlay": true,
  "text": "text-value",
  "visible": true
}
```
##### <a name="response"></a><span data-ttu-id="40dba-145">响应</span><span class="sxs-lookup"><span data-stu-id="40dba-145">Response</span></span>
<span data-ttu-id="40dba-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="40dba-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartTitle"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 64

{
  "overlay": true,
  "text": "text-value",
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update charttitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->