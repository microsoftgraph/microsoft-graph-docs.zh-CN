# <a name="update-chartdatalabels"></a><span data-ttu-id="781a0-101">更新 chartdatalabels</span><span class="sxs-lookup"><span data-stu-id="781a0-101">Update chartdatalabels</span></span>

<span data-ttu-id="781a0-102">更新 chartdatalabels 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="781a0-102">Update the properties of chartdatalabels object.</span></span>
## <a name="permissions"></a><span data-ttu-id="781a0-103">权限</span><span class="sxs-lookup"><span data-stu-id="781a0-103">Permissions</span></span>
<span data-ttu-id="781a0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="781a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="781a0-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="781a0-106">Permission type</span></span>      | <span data-ttu-id="781a0-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="781a0-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="781a0-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="781a0-108">Delegated (work or school account)</span></span> | <span data-ttu-id="781a0-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="781a0-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="781a0-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="781a0-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="781a0-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="781a0-111">Not supported.</span></span>    |
|<span data-ttu-id="781a0-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="781a0-112">Application</span></span> | <span data-ttu-id="781a0-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="781a0-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="781a0-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="781a0-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/dataLabels
```
## <a name="optional-request-headers"></a><span data-ttu-id="781a0-115">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="781a0-115">Optional request headers</span></span>
| <span data-ttu-id="781a0-116">名称</span><span class="sxs-lookup"><span data-stu-id="781a0-116">Name</span></span>       | <span data-ttu-id="781a0-117">说明</span><span class="sxs-lookup"><span data-stu-id="781a0-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="781a0-118">授权</span><span class="sxs-lookup"><span data-stu-id="781a0-118">Authorization</span></span>  | <span data-ttu-id="781a0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="781a0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="781a0-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="781a0-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="781a0-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="781a0-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="781a0-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="781a0-124">Request body</span></span>
<span data-ttu-id="781a0-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="781a0-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="781a0-128">属性</span><span class="sxs-lookup"><span data-stu-id="781a0-128">Property</span></span>     | <span data-ttu-id="781a0-129">类型</span><span class="sxs-lookup"><span data-stu-id="781a0-129">Type</span></span>   |<span data-ttu-id="781a0-130">说明</span><span class="sxs-lookup"><span data-stu-id="781a0-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="781a0-131">职位</span><span class="sxs-lookup"><span data-stu-id="781a0-131">position</span></span>|<span data-ttu-id="781a0-132">字符串</span><span class="sxs-lookup"><span data-stu-id="781a0-132">string</span></span>|<span data-ttu-id="781a0-133">表示数据标签位置的 DataLabelPosition 值。</span><span class="sxs-lookup"><span data-stu-id="781a0-133">DataLabelPosition value that represents the position of the data label. Possible values are: , , , , , , , , , , .</span></span> <span data-ttu-id="781a0-134">可取值为：`None`、`Center`、`InsideEnd`、`InsideBase`、`OutsideEnd`、`Left`、`Right`、`Top`、`Bottom`、`BestFit`、`Callout`。</span><span class="sxs-lookup"><span data-stu-id="781a0-134">The possible values are `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`, or .</span></span>|
|<span data-ttu-id="781a0-135">分隔符</span><span class="sxs-lookup"><span data-stu-id="781a0-135">separator</span></span>|<span data-ttu-id="781a0-136">字符串</span><span class="sxs-lookup"><span data-stu-id="781a0-136">string</span></span>|<span data-ttu-id="781a0-137">表示用于图表中数据标签的分隔符的字符串。</span><span class="sxs-lookup"><span data-stu-id="781a0-137">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="781a0-138">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="781a0-138">showBubbleSize</span></span>|<span data-ttu-id="781a0-139">布尔</span><span class="sxs-lookup"><span data-stu-id="781a0-139">boolean</span></span>|<span data-ttu-id="781a0-140">表示数据标签气泡大小是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="781a0-140">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="781a0-141">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="781a0-141">showCategoryName</span></span>|<span data-ttu-id="781a0-142">布尔</span><span class="sxs-lookup"><span data-stu-id="781a0-142">boolean</span></span>|<span data-ttu-id="781a0-143">表示数据标签类别名称是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="781a0-143">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="781a0-144">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="781a0-144">showLegendKey</span></span>|<span data-ttu-id="781a0-145">布尔</span><span class="sxs-lookup"><span data-stu-id="781a0-145">boolean</span></span>|<span data-ttu-id="781a0-146">表示数据标签图例标示是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="781a0-146">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="781a0-147">showPercentage</span><span class="sxs-lookup"><span data-stu-id="781a0-147">showPercentage</span></span>|<span data-ttu-id="781a0-148">布尔</span><span class="sxs-lookup"><span data-stu-id="781a0-148">boolean</span></span>|<span data-ttu-id="781a0-149">表示数据标签百分比是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="781a0-149">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="781a0-150">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="781a0-150">showSeriesName</span></span>|<span data-ttu-id="781a0-151">布尔</span><span class="sxs-lookup"><span data-stu-id="781a0-151">boolean</span></span>|<span data-ttu-id="781a0-152">表示数据标签系列名称是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="781a0-152">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="781a0-153">showValue</span><span class="sxs-lookup"><span data-stu-id="781a0-153">showValue</span></span>|<span data-ttu-id="781a0-154">布尔</span><span class="sxs-lookup"><span data-stu-id="781a0-154">boolean</span></span>|<span data-ttu-id="781a0-155">表示数据标签值是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="781a0-155">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="response"></a><span data-ttu-id="781a0-156">响应</span><span class="sxs-lookup"><span data-stu-id="781a0-156">Response</span></span>

<span data-ttu-id="781a0-157">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [WorkbookChartDataLabels](../resources/chartdatalabels.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="781a0-157">If successful, this method returns a `200 OK` response code and updated [plannerTaskDetails](../resources/chartdatalabels.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="781a0-158">示例</span><span class="sxs-lookup"><span data-stu-id="781a0-158">Example</span></span>
##### <a name="request"></a><span data-ttu-id="781a0-159">请求</span><span class="sxs-lookup"><span data-stu-id="781a0-159">Request</span></span>
<span data-ttu-id="781a0-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="781a0-160">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartdatalabels"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/dataLabels
Content-type: application/json
Content-length: 134

{
  "position": "position-value",
  "showValue": true,
  "showSeriesName": true,
  "showCategoryName": true,
  "showLegendKey": true
}
```
##### <a name="response"></a><span data-ttu-id="781a0-161">响应</span><span class="sxs-lookup"><span data-stu-id="781a0-161">Response</span></span>
<span data-ttu-id="781a0-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="781a0-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartDataLabels"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 134

{
  "position": "position-value",
  "showValue": true,
  "showSeriesName": true,
  "showCategoryName": true,
  "showLegendKey": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartdatalabels",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->