# <a name="chartcollection-add"></a><span data-ttu-id="08924-101">ChartCollection: add</span><span class="sxs-lookup"><span data-stu-id="08924-101">ChartCollection: add</span></span>

<span data-ttu-id="08924-102">创建新图表。</span><span class="sxs-lookup"><span data-stu-id="08924-102">Creates a new chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="08924-103">权限</span><span class="sxs-lookup"><span data-stu-id="08924-103">Permissions</span></span>
<span data-ttu-id="08924-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="08924-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="08924-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="08924-106">Permission type</span></span>      | <span data-ttu-id="08924-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="08924-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08924-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="08924-108">Delegated (work or school account)</span></span> | <span data-ttu-id="08924-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="08924-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="08924-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="08924-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08924-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="08924-111">Not supported.</span></span>    |
|<span data-ttu-id="08924-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="08924-112">Application</span></span> | <span data-ttu-id="08924-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="08924-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="08924-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="08924-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/add

```
## <a name="request-headers"></a><span data-ttu-id="08924-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="08924-115">Request headers</span></span>
| <span data-ttu-id="08924-116">名称</span><span class="sxs-lookup"><span data-stu-id="08924-116">Name</span></span>       | <span data-ttu-id="08924-117">说明</span><span class="sxs-lookup"><span data-stu-id="08924-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="08924-118">授权</span><span class="sxs-lookup"><span data-stu-id="08924-118">Authorization</span></span>  | <span data-ttu-id="08924-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="08924-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="08924-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="08924-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="08924-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="08924-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="08924-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="08924-124">Request body</span></span>
<span data-ttu-id="08924-125">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="08924-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="08924-126">参数</span><span class="sxs-lookup"><span data-stu-id="08924-126">Parameter</span></span>    | <span data-ttu-id="08924-127">类型</span><span class="sxs-lookup"><span data-stu-id="08924-127">Type</span></span>   |<span data-ttu-id="08924-128">说明</span><span class="sxs-lookup"><span data-stu-id="08924-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="08924-129">类型</span><span class="sxs-lookup"><span data-stu-id="08924-129">type</span></span>|<span data-ttu-id="08924-130">字符串</span><span class="sxs-lookup"><span data-stu-id="08924-130">string</span></span>|<span data-ttu-id="08924-131">代表图表的类型。</span><span class="sxs-lookup"><span data-stu-id="08924-131">Represents the name of a chart object.</span></span>  <span data-ttu-id="08924-132">可能的值为：`ColumnClustered`、`ColumnStacked`、`ColumnStacked100`、`BarClustered`、`BarStacked`、`BarStacked100`、`LineStacked`、`LineStacked100`、`LineMarkers`、`LineMarkersStacked`、`LineMarkersStacked100`、`PieOfPie`、`etc.`。</span><span class="sxs-lookup"><span data-stu-id="08924-132">The possible values are `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, or `PieOfPie`.</span></span>|
|<span data-ttu-id="08924-133">sourceData</span><span class="sxs-lookup"><span data-stu-id="08924-133">sourceData</span></span>|<span data-ttu-id="08924-134">Json</span><span class="sxs-lookup"><span data-stu-id="08924-134">Json</span></span>|<span data-ttu-id="08924-135">对应于源数据的 Range 对象。</span><span class="sxs-lookup"><span data-stu-id="08924-135">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="08924-136">seriesBy</span><span class="sxs-lookup"><span data-stu-id="08924-136">seriesBy</span></span>|<span data-ttu-id="08924-137">字符串</span><span class="sxs-lookup"><span data-stu-id="08924-137">string</span></span>|<span data-ttu-id="08924-138">可选。</span><span class="sxs-lookup"><span data-stu-id="08924-138">Optional.</span></span> <span data-ttu-id="08924-139">设置行或列在图表上用作数据系列的方式。</span><span class="sxs-lookup"><span data-stu-id="08924-139">Returns or sets the way columns or rows are used as data series on the chart.</span></span>  <span data-ttu-id="08924-140">可取值为：`Auto`、`Columns`、`Rows`。</span><span class="sxs-lookup"><span data-stu-id="08924-140">The possible values are `Auto`, `Columns`, `Rows`, , , , , , , , , or .</span></span>|

## <a name="response"></a><span data-ttu-id="08924-141">响应</span><span class="sxs-lookup"><span data-stu-id="08924-141">Response</span></span>

<span data-ttu-id="08924-142">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [WorkbookChart](../resources/chart.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="08924-142">If successful, this method returns `200 OK` response code and [groupSetting](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08924-143">示例</span><span class="sxs-lookup"><span data-stu-id="08924-143">Example</span></span>
<span data-ttu-id="08924-144">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="08924-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="08924-145">请求</span><span class="sxs-lookup"><span data-stu-id="08924-145">Request</span></span>
<span data-ttu-id="08924-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="08924-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/add
Content-type: application/json
Content-length: 94

{
  "type": "ColumnStacked",
  "sourceData": "A1:B1",
  "seriesBy": "Auto"
}
```

##### <a name="response"></a><span data-ttu-id="08924-147">响应</span><span class="sxs-lookup"><span data-stu-id="08924-147">Response</span></span>
<span data-ttu-id="08924-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="08924-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChart"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
