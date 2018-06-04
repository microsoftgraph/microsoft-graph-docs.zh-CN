# <a name="use-workbook-functions-in-excel-with-microsoft-graph"></a><span data-ttu-id="4e648-101">通过 Microsoft Graph 使用 Excel 工作簿函数</span><span class="sxs-lookup"><span data-stu-id="4e648-101">Use workbook functions in Excel with Microsoft Graph</span></span>

<span data-ttu-id="4e648-102">可以使用以下语法调用任何工作簿函数：`POST /workbook/functions/{function-name}`。</span><span class="sxs-lookup"><span data-stu-id="4e648-102">You can invoke any workbook function by using the following syntax: `POST /workbook/functions/{function-name}`.</span></span> <span data-ttu-id="4e648-103">使用 JSON 对象提供正文中的函数参数。</span><span class="sxs-lookup"><span data-stu-id="4e648-103">You provide the function argument(s) in the body using a JSON object.</span></span> <span data-ttu-id="4e648-104">该函数产生 `value`，所有 `error` 字符串均返回到函数结果对象中。</span><span class="sxs-lookup"><span data-stu-id="4e648-104">The function's resulting `value` and any `error` strings are returned in the function result object.</span></span> <span data-ttu-id="4e648-105">`null` 的 `error` 值表示该函数执行成功。</span><span class="sxs-lookup"><span data-stu-id="4e648-105">The `error` value of `null` indicates successful execution of the function.</span></span>

<span data-ttu-id="4e648-106">受支持函数的完整列表位于[此处](https://support.office.com/zh-CN/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188)。</span><span class="sxs-lookup"><span data-stu-id="4e648-106">The complete list of supported functions are listed [here](https://support.office.com/zh-CN/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188).</span></span> <span data-ttu-id="4e648-107">请参阅特定参数名称和数据类型的函数签名。</span><span class="sxs-lookup"><span data-stu-id="4e648-107">Refer to the function signature for specific parameter names and data types.</span></span>

<span data-ttu-id="4e648-108">_重要说明_：</span><span class="sxs-lookup"><span data-stu-id="4e648-108">_Important notes:_</span></span>
* <span data-ttu-id="4e648-109">使用 range 对象（而不是范围地址字符串）提供范围输入参数。</span><span class="sxs-lookup"><span data-stu-id="4e648-109">The range input parameter is supplied using a range object instead of the range address string.</span></span>  
* <span data-ttu-id="4e648-110">与大部分 API 中使用的从 0 开始编制的索引不同，索引参数是从 1 开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="4e648-110">The index parameter is 1-indexed unlike the 0-index used in most of the APIs.</span></span>

<span data-ttu-id="4e648-111">示例：**vlookup**</span><span class="sxs-lookup"><span data-stu-id="4e648-111">Example: **vlookup**</span></span>

<span data-ttu-id="4e648-112">在 Excel 电子表格中，`vlookup` 函数需要使用以下参数：</span><span class="sxs-lookup"><span data-stu-id="4e648-112">In an Excel spreadsheet, the `vlookup` function takes the following arguments:</span></span>

1. <span data-ttu-id="4e648-113">lookup_value****（必需）要查找的值。</span><span class="sxs-lookup"><span data-stu-id="4e648-113">**lookup_value** (required) The value you want to look up.</span></span>
2. <span data-ttu-id="4e648-114">table_array**table_array**（必需）查阅值所在的单元格的区域。</span><span class="sxs-lookup"><span data-stu-id="4e648-114">**table_array** (required) The range of cells where the lookup value is located.</span></span> <span data-ttu-id="4e648-115">请注意，查阅值应始终位于区域中的第一列，这样 VLOOKUP 才能正常运行。</span><span class="sxs-lookup"><span data-stu-id="4e648-115">Remember that the lookup value should always be in the first column in the range for VLOOKUP to work correctly.</span></span> <span data-ttu-id="4e648-116">例如，如果查阅值位于单元格 C2，那么区域应从 C 列开始。</span><span class="sxs-lookup"><span data-stu-id="4e648-116">For example, if your lookup value is in cell C2 then your range should start with C.</span></span>
3. <span data-ttu-id="4e648-117">col_index_num****（必需）包含返回值的区域的列号。</span><span class="sxs-lookup"><span data-stu-id="4e648-117">The column number in the range that contains the return value.</span></span> <span data-ttu-id="4e648-118">例如，如果指定 B2: D11 作为区域，应将 B 计为第一列，将 C 计为第二列，依此类推。</span><span class="sxs-lookup"><span data-stu-id="4e648-118">For example, if you specify B2: D11 as the range, you should count B as the first column, C as the second, and so on.</span></span>
4. <span data-ttu-id="4e648-119">range_lookup****（可选）一个逻辑值，指定希望 VLOOKUP**** 查找近似匹配还是精确的匹配。</span><span class="sxs-lookup"><span data-stu-id="4e648-119">**range_lookup** (optional) The logical value that specifies whether you want **VLOOKUP** to find an approximate or an exact match.</span></span> <span data-ttu-id="4e648-120">如果想要近似匹配，可指定 TRUE****；如果想要返回值的完全匹配，则可指定 FALSE****。</span><span class="sxs-lookup"><span data-stu-id="4e648-120">Optionally, you can specify TRUE if you want an approximate match or FALSE if you want an exact match of the return value.</span></span> <span data-ttu-id="4e648-121">如果未指定，默认值始终为 TRUE 或近似匹配。</span><span class="sxs-lookup"><span data-stu-id="4e648-121">If you don't specify anything, the default value will always be TRUE or approximate match.</span></span>

<span data-ttu-id="4e648-122">在单元格中，`vlookup` 函数如下所示：</span><span class="sxs-lookup"><span data-stu-id="4e648-122">Inside a cell, the `vlookup` function looks like this:</span></span>

<span data-ttu-id="4e648-123">=VLOOKUP(查阅值, 包含查阅值的区域, 包含返回值的区域的列号, 视需要为近似匹配指定 TRUE 或为完全匹配指定 FALSE)</span><span class="sxs-lookup"><span data-stu-id="4e648-123">=VLOOKUP(lookup value, range containing the lookup value, the column number in the range containing the return value, optionally specify TRUE for approximate match or FALSE for an exact match)</span></span>

<span data-ttu-id="4e648-124">（请参阅 [VLOOKUP Excel 函数](https://support.office.com/zh-CN/article/VLOOKUP-function-0bbc8083-26fe-4963-8ab8-93a18ad188a1)文档。）</span><span class="sxs-lookup"><span data-stu-id="4e648-124">(See the documentation for the [VLOOKUP Excel function](https://support.office.com/zh-CN/article/VLOOKUP-function-0bbc8083-26fe-4963-8ab8-93a18ad188a1).)</span></span>


##### <a name="request"></a><span data-ttu-id="4e648-125">请求:</span><span class="sxs-lookup"><span data-stu-id="4e648-125">Request:</span></span>
<span data-ttu-id="4e648-126">下面的示例展示了如何使用 Excel REST API 调用 `vlookup` 函数和传递这些参数。</span><span class="sxs-lookup"><span data-stu-id="4e648-126">The example below shows how to call the `vlookup` function and pass these parameters with the Excel REST API.</span></span>

```http
POST https://graph.microsoft.com/beta/me/drive/root:/book1.xlsx:/workbook/functions/vlookup
content-type: Application/Json
authorization: Bearer {access-token}
workbook-session-id: {session-id}

{
    "lookupValue": "Temperature",
    "tableArray": { "Address": "Sheet1!E1:G5" },
    "colIndexNum": 2,
    "rangeLookup": false
}
```

##### <a name="response"></a><span data-ttu-id="4e648-127">响应</span><span class="sxs-lookup"><span data-stu-id="4e648-127">Response</span></span>

```http
HTTP code: 200 OK
content-type: application/json;odata.metadata

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#workbookFunctionResult",
    "@odata.type": "#microsoft.graph.workbookFunctionResult",
    "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/root/workbook/functions/vlookup()",
    "error": null,
    "value": "28.3"
}
```

<span data-ttu-id="4e648-128">示例：`median`</span><span class="sxs-lookup"><span data-stu-id="4e648-128">Example: `median`</span></span>

<span data-ttu-id="4e648-129">在 Excel 电子表格中，`median` 函数需要使用一个或多个输入区域。</span><span class="sxs-lookup"><span data-stu-id="4e648-129">In an Excel spreadsheet, the `median` function takes an array of one or more input ranges.</span></span>

<span data-ttu-id="4e648-130">在单元格中，`median` 函数如以下示例所示：</span><span class="sxs-lookup"><span data-stu-id="4e648-130">Inside a cell, the `median` function looks like this example:</span></span>

<span data-ttu-id="4e648-131">=MEDIAN(A2:A6)</span><span class="sxs-lookup"><span data-stu-id="4e648-131">=MEDIAN(A2:A6)</span></span>

<span data-ttu-id="4e648-132">（请参阅 [MEDIAN Excel 函数](https://support.office.com/zh-CN/article/MEDIAN-function-d0916313-4753-414c-8537-ce85bdd967d2)文档。）</span><span class="sxs-lookup"><span data-stu-id="4e648-132">(See the documentation for the [MEDIAN Excel function](https://support.office.com/zh-CN/article/MEDIAN-function-d0916313-4753-414c-8537-ce85bdd967d2).)</span></span>

##### <a name="request"></a><span data-ttu-id="4e648-133">请求</span><span class="sxs-lookup"><span data-stu-id="4e648-133">Request</span></span>
<span data-ttu-id="4e648-134">下面的示例展示了如何使用 Excel REST API 调用 `median` 函数和一个或多个输入区域。</span><span class="sxs-lookup"><span data-stu-id="4e648-134">The example below shows how to call the `median` function and one or more input ranges with the Excel REST API.</span></span>

```http
POST https://graph.microsoft.com/beta/me/drive/root:/book1.xlsx:/workbook/functions/median
content-type: Application/Json
authorization: Bearer {access-token}
workbook-session-id: {session-id}

{
"values" :  [
        { "address": "Sheet2!A1:A5" },
        { "address": "Sheet2!B1:B5" },
      ]
}
```

##### <a name="response"></a><span data-ttu-id="4e648-135">响应</span><span class="sxs-lookup"><span data-stu-id="4e648-135">Response</span></span>

```http
HTTP code: 200 OK
content-type: application/json;odata.metadata

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#workbookFunctionResult",
  "@odata.type": "#microsoft.graph.workbookFunctionResult",
  "@odata.id": "/users('2abcad6a-2fca-4b6e-9577-e358a757d77d')/drive/root/workbook/functions/median()",
  "error": null,
  "value": 30
}
```

## <a name="see-also"></a><span data-ttu-id="4e648-136">另请参阅</span><span class="sxs-lookup"><span data-stu-id="4e648-136">See also</span></span>
* [<span data-ttu-id="4e648-137">通过 Microsoft Graph 管理 Excel 会话</span><span class="sxs-lookup"><span data-stu-id="4e648-137">Manage sessions in Excel with Microsoft Graph</span></span>](excel-manage-sessions.md)
* [<span data-ttu-id="4e648-138">使用 Microsoft Graph 编写 Excel 工作簿</span><span class="sxs-lookup"><span data-stu-id="4e648-138">Write to an Excel workbook using Microsoft Graph</span></span>](excel-write-to-workbook.md)
* [<span data-ttu-id="4e648-139">通过 Microsoft Graph 更新 Excel 区域的格式</span><span class="sxs-lookup"><span data-stu-id="4e648-139">Update a range’s format in Excel with Microsoft Graph</span></span>](excel-update-range-format.md)
* [<span data-ttu-id="4e648-140">通过 Microsoft Graph 显示 Excel 图表图像</span><span class="sxs-lookup"><span data-stu-id="4e648-140">Display a chart image in Excel with Microsoft Graph</span></span>](excel-display-chart-image.md)
* [<span data-ttu-id="4e648-141">使用 Excel REST API</span><span class="sxs-lookup"><span data-stu-id="4e648-141">Use the Excel REST API</span></span>](../api-reference/v1.0/resources/excel.md)
