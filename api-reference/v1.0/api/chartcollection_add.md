# <a name="chartcollection-add"></a><span data-ttu-id="24749-101">ChartCollection: add</span><span class="sxs-lookup"><span data-stu-id="24749-101">ChartCollection: add</span></span>

<span data-ttu-id="24749-102">创建新图表。</span><span class="sxs-lookup"><span data-stu-id="24749-102">Creates a new chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="24749-103">权限</span><span class="sxs-lookup"><span data-stu-id="24749-103">Permissions</span></span>
<span data-ttu-id="24749-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="24749-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="24749-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="24749-106">Permission type</span></span>      | <span data-ttu-id="24749-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="24749-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="24749-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="24749-108">Delegated (work or school account)</span></span> | <span data-ttu-id="24749-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="24749-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="24749-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="24749-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24749-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="24749-111">Not supported.</span></span>    |
|<span data-ttu-id="24749-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="24749-112">Application</span></span> | <span data-ttu-id="24749-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="24749-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="24749-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="24749-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/add

```
## <a name="request-headers"></a><span data-ttu-id="24749-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="24749-115">Request headers</span></span>
| <span data-ttu-id="24749-116">名称</span><span class="sxs-lookup"><span data-stu-id="24749-116">Name</span></span>       | <span data-ttu-id="24749-117">说明</span><span class="sxs-lookup"><span data-stu-id="24749-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="24749-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="24749-118">Authorization</span></span>  | <span data-ttu-id="24749-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="24749-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="24749-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="24749-121">Request body</span></span>
<span data-ttu-id="24749-122">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="24749-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="24749-123">参数</span><span class="sxs-lookup"><span data-stu-id="24749-123">Parameter</span></span>    | <span data-ttu-id="24749-124">类型</span><span class="sxs-lookup"><span data-stu-id="24749-124">Type</span></span>   |<span data-ttu-id="24749-125">说明</span><span class="sxs-lookup"><span data-stu-id="24749-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="24749-126">type</span><span class="sxs-lookup"><span data-stu-id="24749-126">type</span></span>|<span data-ttu-id="24749-127">string</span><span class="sxs-lookup"><span data-stu-id="24749-127">string</span></span>|<span data-ttu-id="24749-p103">表示图表的类型。可能的值是：`ColumnClustered`、`ColumnStacked`、`ColumnStacked100`、`BarClustered`、`BarStacked`、`BarStacked100`、`LineStacked`、`LineStacked100`、`LineMarkers`、`LineMarkersStacked`、`LineMarkersStacked100`、`PieOfPie`、`etc.`。</span><span class="sxs-lookup"><span data-stu-id="24749-p103">Represents the type of a chart.  Possible values are: `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, `PieOfPie`, `etc.`.</span></span>|
|<span data-ttu-id="24749-130">sourceData</span><span class="sxs-lookup"><span data-stu-id="24749-130">sourceData</span></span>|<span data-ttu-id="24749-131">string</span><span class="sxs-lookup"><span data-stu-id="24749-131">string</span></span>|<span data-ttu-id="24749-132">对应于源数据的 Range 对象。</span><span class="sxs-lookup"><span data-stu-id="24749-132">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="24749-133">seriesBy</span><span class="sxs-lookup"><span data-stu-id="24749-133">seriesBy</span></span>|<span data-ttu-id="24749-134">string</span><span class="sxs-lookup"><span data-stu-id="24749-134">string</span></span>|<span data-ttu-id="24749-p104">可选。指定列或行在图表上用作数据系列的方式。可能的值是：`Auto`、`Columns`、`Rows`。</span><span class="sxs-lookup"><span data-stu-id="24749-p104">Optional. Specifies the way columns or rows are used as data series on the chart.  Possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="24749-138">响应</span><span class="sxs-lookup"><span data-stu-id="24749-138">Response</span></span>

<span data-ttu-id="24749-139">如果成功，此方法在响应正文中返回 `200, OK` 响应代码和 [Chart](../resources/chart.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="24749-139">If successful, this method returns `200, OK` response code and [Chart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24749-140">示例</span><span class="sxs-lookup"><span data-stu-id="24749-140">Example</span></span>
<span data-ttu-id="24749-141">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="24749-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="24749-142">请求</span><span class="sxs-lookup"><span data-stu-id="24749-142">Request</span></span>
<span data-ttu-id="24749-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="24749-143">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="24749-144">响应</span><span class="sxs-lookup"><span data-stu-id="24749-144">Response</span></span>
<span data-ttu-id="24749-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="24749-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chart"
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
