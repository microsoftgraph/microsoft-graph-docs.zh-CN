# <a name="worksheet-usedrange"></a><span data-ttu-id="e2fee-101">Worksheet:UsedRange</span><span class="sxs-lookup"><span data-stu-id="e2fee-101">Worksheet: UsedRange</span></span>

<span data-ttu-id="e2fee-p101">使用的区域是包含分配了值或格式化的任何单元格的最小区域。如果工作表为空，此函数将返回左上角的单元格。</span><span class="sxs-lookup"><span data-stu-id="e2fee-p101">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e2fee-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="e2fee-104">Prerequisites</span></span>
<span data-ttu-id="e2fee-105">要执行此 API，需要以下**范围**：</span><span class="sxs-lookup"><span data-stu-id="e2fee-105">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="e2fee-106">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e2fee-106">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="e2fee-107">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e2fee-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/UsedRange

```

## <a name="optional-request-parameter"></a><span data-ttu-id="e2fee-108">可选的请求参数</span><span class="sxs-lookup"><span data-stu-id="e2fee-108">Optional request parameter</span></span>
<span data-ttu-id="e2fee-109">在请求 URL 中，提供可选的查询参数。</span><span class="sxs-lookup"><span data-stu-id="e2fee-109">In the request URL, provide an optional query parameter.</span></span>

| <span data-ttu-id="e2fee-110">参数</span><span class="sxs-lookup"><span data-stu-id="e2fee-110">Parameter</span></span>    | <span data-ttu-id="e2fee-111">类型</span><span class="sxs-lookup"><span data-stu-id="e2fee-111">Type</span></span>   |<span data-ttu-id="e2fee-112">说明</span><span class="sxs-lookup"><span data-stu-id="e2fee-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e2fee-113">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="e2fee-113">valuesOnly</span></span>|<span data-ttu-id="e2fee-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2fee-114">Boolean</span></span>|<span data-ttu-id="e2fee-p102">可选。仅将具有值的单元格视为已使用的单元格（忽略格式）。</span><span class="sxs-lookup"><span data-stu-id="e2fee-p102">Optional. Considers only cells with values as used cells (ignores formatting).</span></span>|


## <a name="request-headers"></a><span data-ttu-id="e2fee-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="e2fee-117">Request headers</span></span>
| <span data-ttu-id="e2fee-118">名称</span><span class="sxs-lookup"><span data-stu-id="e2fee-118">Name</span></span>       | <span data-ttu-id="e2fee-119">说明</span><span class="sxs-lookup"><span data-stu-id="e2fee-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e2fee-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2fee-120">Authorization</span></span>  | <span data-ttu-id="e2fee-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e2fee-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="e2fee-123">响应</span><span class="sxs-lookup"><span data-stu-id="e2fee-123">Response</span></span>

<span data-ttu-id="e2fee-124">如果成功，此方法在响应正文中返回 `200, OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e2fee-124">If successful, this method returns `200, OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2fee-125">示例</span><span class="sxs-lookup"><span data-stu-id="e2fee-125">Example</span></span>
<span data-ttu-id="e2fee-126">下面的示例展示了如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="e2fee-126">Here is an example that shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e2fee-127">请求</span><span class="sxs-lookup"><span data-stu-id="e2fee-127">Request</span></span>
<span data-ttu-id="e2fee-128">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e2fee-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_usedrange"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/UsedRange(valuesOnly=true)
Content-type: application/json

```

##### <a name="response"></a><span data-ttu-id="e2fee-129">响应</span><span class="sxs-lookup"><span data-stu-id="e2fee-129">Response</span></span>
<span data-ttu-id="e2fee-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e2fee-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet: UsedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
