# <a name="workbook-resource-type"></a><span data-ttu-id="bae6e-101">工作簿资源类型</span><span class="sxs-lookup"><span data-stu-id="bae6e-101">Workbook resource type</span></span>

<span data-ttu-id="bae6e-102">工作簿是顶级对象，它包含相关 workbook 对象，例如工作表、表、范围等。</span><span class="sxs-lookup"><span data-stu-id="bae6e-102">Workbook is the top level object which contains related workbook objects such as worksheets, tables, ranges, etc.</span></span>

## <a name="properties"></a><span data-ttu-id="bae6e-103">属性</span><span class="sxs-lookup"><span data-stu-id="bae6e-103">Properties</span></span>
<span data-ttu-id="bae6e-104">无</span><span class="sxs-lookup"><span data-stu-id="bae6e-104">None</span></span>

## <a name="methods"></a><span data-ttu-id="bae6e-105">方法</span><span class="sxs-lookup"><span data-stu-id="bae6e-105">Methods</span></span>

| <span data-ttu-id="bae6e-106">方法</span><span class="sxs-lookup"><span data-stu-id="bae6e-106">Method</span></span>       | <span data-ttu-id="bae6e-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="bae6e-107">Return Type</span></span>  |<span data-ttu-id="bae6e-108">说明</span><span class="sxs-lookup"><span data-stu-id="bae6e-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bae6e-109">Create Session</span><span class="sxs-lookup"><span data-stu-id="bae6e-109">Create Session</span></span>](../api/workbook_createsession.md) | [<span data-ttu-id="bae6e-110">workbookSessionInfo</span><span class="sxs-lookup"><span data-stu-id="bae6e-110">workbookSessionInfo</span></span>](workbooksessioninfo.md) |<span data-ttu-id="bae6e-111">创建工作簿会话以启动永久或非永久会话。</span><span class="sxs-lookup"><span data-stu-id="bae6e-111">Create a workbook session to start a persistent or non-persistent session.</span></span>|
|[<span data-ttu-id="bae6e-112">Close Session</span><span class="sxs-lookup"><span data-stu-id="bae6e-112">Close Session</span></span>](../api/workbook_closesession.md) | <span data-ttu-id="bae6e-113">无</span><span class="sxs-lookup"><span data-stu-id="bae6e-113">None</span></span> |<span data-ttu-id="bae6e-114">关闭现有会话。</span><span class="sxs-lookup"><span data-stu-id="bae6e-114">Close an existing session.</span></span>|
|[<span data-ttu-id="bae6e-115">Refresh Session</span><span class="sxs-lookup"><span data-stu-id="bae6e-115">Refresh Session</span></span>](../api/workbook_refreshsession.md) | <span data-ttu-id="bae6e-116">无</span><span class="sxs-lookup"><span data-stu-id="bae6e-116">None</span></span> |<span data-ttu-id="bae6e-117">刷新现有会话。</span><span class="sxs-lookup"><span data-stu-id="bae6e-117">Refresh an existing session.</span></span>|


## <a name="relationships"></a><span data-ttu-id="bae6e-118">关系</span><span class="sxs-lookup"><span data-stu-id="bae6e-118">Relationships</span></span>
| <span data-ttu-id="bae6e-119">关系</span><span class="sxs-lookup"><span data-stu-id="bae6e-119">Relationship</span></span> | <span data-ttu-id="bae6e-120">类型</span><span class="sxs-lookup"><span data-stu-id="bae6e-120">Type</span></span>   |<span data-ttu-id="bae6e-121">说明</span><span class="sxs-lookup"><span data-stu-id="bae6e-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bae6e-122">names</span><span class="sxs-lookup"><span data-stu-id="bae6e-122">names</span></span>|<span data-ttu-id="bae6e-123">[NamedItem](nameditem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bae6e-123">[NamedItem](nameditem.md) collection</span></span>|<span data-ttu-id="bae6e-p101">表示工作簿范围内的已命名项目（称为区域和常量）的集合。只读。</span><span class="sxs-lookup"><span data-stu-id="bae6e-p101">Represents a collection of workbook scoped named items (named ranges and constants). Read-only.</span></span>|
|<span data-ttu-id="bae6e-126">表格</span><span class="sxs-lookup"><span data-stu-id="bae6e-126">tables</span></span>|<span data-ttu-id="bae6e-127">[Table](table.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bae6e-127">[Table](table.md) collection</span></span>|<span data-ttu-id="bae6e-p102">表示与工作簿关联的表的集合。只读。</span><span class="sxs-lookup"><span data-stu-id="bae6e-p102">Represents a collection of tables associated with the workbook. Read-only.</span></span>|
|<span data-ttu-id="bae6e-130">Worksheets</span><span class="sxs-lookup"><span data-stu-id="bae6e-130">worksheets</span></span>|<span data-ttu-id="bae6e-131">[Worksheet](worksheet.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bae6e-131">[Worksheet](worksheet.md) collection</span></span>|<span data-ttu-id="bae6e-p103">表示与工作簿关联的工作表的集合。只读。</span><span class="sxs-lookup"><span data-stu-id="bae6e-p103">Represents a collection of worksheets associated with the workbook. Read-only.</span></span>|

## <a name="functions"></a><span data-ttu-id="bae6e-134">函数</span><span class="sxs-lookup"><span data-stu-id="bae6e-134">Functions</span></span>

<span data-ttu-id="bae6e-135">[Excel 函数](#functions)使用 JSON 对象调用使用语法 `POST /workbook/functions/{function-name}` 并在正文中提供函数自变量的工作簿函数。</span><span class="sxs-lookup"><span data-stu-id="bae6e-135">[Excel functions](#functions): Invoke a workbook function using the syntax `POST /workbook/functions/{function-name}` and providing the function argument(s) in the body using a JSON object.</span></span> <span data-ttu-id="bae6e-136">该函数产生 `value`，所有 `error` 字符串均返回到函数结果对象中。</span><span class="sxs-lookup"><span data-stu-id="bae6e-136">The function's resulting `value` and any `error` strings are returned in the function result object.</span></span> <span data-ttu-id="bae6e-137">`null` 的 `error` 值表示该函数执行成功。</span><span class="sxs-lookup"><span data-stu-id="bae6e-137">The `error` value of `null` indicates successful execution of the function.</span></span> 

<span data-ttu-id="bae6e-138">受支持函数的完整列表位于[此处](https://support.office.com/en-us/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188)。</span><span class="sxs-lookup"><span data-stu-id="bae6e-138">The complete list of supported functions are listed [here](https://support.office.com/en-us/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188).</span></span> <span data-ttu-id="bae6e-139">请参阅特定参数名称和数据类型的函数签名。</span><span class="sxs-lookup"><span data-stu-id="bae6e-139">Refer to the function signature for specific parameter names and data types.</span></span>

<span data-ttu-id="bae6e-140">_重要说明_：</span><span class="sxs-lookup"><span data-stu-id="bae6e-140">_Important notes:_</span></span> 
* <span data-ttu-id="bae6e-141">使用 range 对象（而不是范围地址字符串）提供范围输入参数。</span><span class="sxs-lookup"><span data-stu-id="bae6e-141">The range input parameter is supplied using a range object instead of the range address string.</span></span>  
* <span data-ttu-id="bae6e-142">与大部分 API 中使用的从 0 开始的索引不同，索引参数从 1 开始索引。</span><span class="sxs-lookup"><span data-stu-id="bae6e-142">The index parameter is 1-indexed unlike the 0-index used in most of the APIs.</span></span> 

<span data-ttu-id="bae6e-143">示例：</span><span class="sxs-lookup"><span data-stu-id="bae6e-143">Example:</span></span> 

<span data-ttu-id="bae6e-144">在下面的示例中，通过传递查阅值、输入范围和要返回的值调用 `vlookup` 函数。</span><span class="sxs-lookup"><span data-stu-id="bae6e-144">In the below example, `vlookup` function is called by passing lookup value, input range and the value to be returned.</span></span> 

<span data-ttu-id="bae6e-145">请求：</span><span class="sxs-lookup"><span data-stu-id="bae6e-145">Request:</span></span> 

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

<span data-ttu-id="bae6e-146">响应：</span><span class="sxs-lookup"><span data-stu-id="bae6e-146">Response:</span></span>

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

<span data-ttu-id="bae6e-147">示例：</span><span class="sxs-lookup"><span data-stu-id="bae6e-147">Example:</span></span> 

<span data-ttu-id="bae6e-148">在下面的示例中，通过传递数组中输入范围调用 `median` 函数。</span><span class="sxs-lookup"><span data-stu-id="bae6e-148">In the below example, `median` function is called by passing the input range(s) in an array.</span></span> 

<span data-ttu-id="bae6e-149">请求：</span><span class="sxs-lookup"><span data-stu-id="bae6e-149">Request:</span></span> 

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

<span data-ttu-id="bae6e-150">响应：</span><span class="sxs-lookup"><span data-stu-id="bae6e-150">Response:</span></span>

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Workbook resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
