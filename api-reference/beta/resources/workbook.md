---
title: 工作簿资源类型
description: 工作簿是顶级对象，它包含相关 workbook 对象，例如工作表、表、范围等。
localization_priority: Normal
ms.openlocfilehash: 9479c6888dc27fd595db2313ab6a88617410530f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806795"
---
# <a name="workbook-resource-type"></a><span data-ttu-id="3f6e1-103">工作簿资源类型</span><span class="sxs-lookup"><span data-stu-id="3f6e1-103">Workbook resource type</span></span>

<span data-ttu-id="3f6e1-104">工作簿是顶级对象，它包含相关 workbook 对象，例如工作表、表、范围等。</span><span class="sxs-lookup"><span data-stu-id="3f6e1-104">Workbook is the top level object which contains related workbook objects such as worksheets, tables, ranges, etc.</span></span>

## <a name="properties"></a><span data-ttu-id="3f6e1-105">属性</span><span class="sxs-lookup"><span data-stu-id="3f6e1-105">Properties</span></span>
<span data-ttu-id="3f6e1-106">无</span><span class="sxs-lookup"><span data-stu-id="3f6e1-106">None</span></span>

## <a name="methods"></a><span data-ttu-id="3f6e1-107">方法</span><span class="sxs-lookup"><span data-stu-id="3f6e1-107">Methods</span></span>

| <span data-ttu-id="3f6e1-108">方法</span><span class="sxs-lookup"><span data-stu-id="3f6e1-108">Method</span></span>       | <span data-ttu-id="3f6e1-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="3f6e1-109">Return Type</span></span>  |<span data-ttu-id="3f6e1-110">说明</span><span class="sxs-lookup"><span data-stu-id="3f6e1-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3f6e1-111">Create Session</span><span class="sxs-lookup"><span data-stu-id="3f6e1-111">Create Session</span></span>](../api/workbook-createsession.md) | [<span data-ttu-id="3f6e1-112">workbookSessionInfo</span><span class="sxs-lookup"><span data-stu-id="3f6e1-112">workbookSessionInfo</span></span>](workbooksessioninfo.md) |<span data-ttu-id="3f6e1-113">创建工作簿会话以启动永久或非永久会话。</span><span class="sxs-lookup"><span data-stu-id="3f6e1-113">Create a workbook session to start a persistent or non-persistent session.</span></span>|
|[<span data-ttu-id="3f6e1-114">Close Session</span><span class="sxs-lookup"><span data-stu-id="3f6e1-114">Close Session</span></span>](../api/workbook-closesession.md) | <span data-ttu-id="3f6e1-115">无</span><span class="sxs-lookup"><span data-stu-id="3f6e1-115">None</span></span> |<span data-ttu-id="3f6e1-116">关闭现有会话。</span><span class="sxs-lookup"><span data-stu-id="3f6e1-116">Close an existing session.</span></span>|
|[<span data-ttu-id="3f6e1-117">Refresh Session</span><span class="sxs-lookup"><span data-stu-id="3f6e1-117">Refresh Session</span></span>](../api/workbook-refreshsession.md) | <span data-ttu-id="3f6e1-118">无</span><span class="sxs-lookup"><span data-stu-id="3f6e1-118">None</span></span> |<span data-ttu-id="3f6e1-119">刷新现有会话。</span><span class="sxs-lookup"><span data-stu-id="3f6e1-119">Refresh an existing session.</span></span>|


## <a name="relationships"></a><span data-ttu-id="3f6e1-120">关系</span><span class="sxs-lookup"><span data-stu-id="3f6e1-120">Relationships</span></span>
| <span data-ttu-id="3f6e1-121">关系</span><span class="sxs-lookup"><span data-stu-id="3f6e1-121">Relationship</span></span> | <span data-ttu-id="3f6e1-122">类型</span><span class="sxs-lookup"><span data-stu-id="3f6e1-122">Type</span></span>   |<span data-ttu-id="3f6e1-123">说明</span><span class="sxs-lookup"><span data-stu-id="3f6e1-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3f6e1-124">names</span><span class="sxs-lookup"><span data-stu-id="3f6e1-124">names</span></span>|<span data-ttu-id="3f6e1-125">[NamedItem](nameditem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3f6e1-125">[NamedItem](nameditem.md) collection</span></span>|<span data-ttu-id="3f6e1-p101">表示工作簿范围内的已命名项目（称为区域和常量）的集合。只读。</span><span class="sxs-lookup"><span data-stu-id="3f6e1-p101">Represents a collection of workbook scoped named items (named ranges and constants). Read-only.</span></span>|
|<span data-ttu-id="3f6e1-128">表格</span><span class="sxs-lookup"><span data-stu-id="3f6e1-128">tables</span></span>|<span data-ttu-id="3f6e1-129">[Table](table.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3f6e1-129">[Table](table.md) collection</span></span>|<span data-ttu-id="3f6e1-p102">表示与工作簿关联的表的集合。只读。</span><span class="sxs-lookup"><span data-stu-id="3f6e1-p102">Represents a collection of tables associated with the workbook. Read-only.</span></span>|
|<span data-ttu-id="3f6e1-132">Worksheets</span><span class="sxs-lookup"><span data-stu-id="3f6e1-132">worksheets</span></span>|<span data-ttu-id="3f6e1-133">[Worksheet](worksheet.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3f6e1-133">[Worksheet](worksheet.md) collection</span></span>|<span data-ttu-id="3f6e1-p103">表示与工作簿关联的工作表的集合。只读。</span><span class="sxs-lookup"><span data-stu-id="3f6e1-p103">Represents a collection of worksheets associated with the workbook. Read-only.</span></span>|

## <a name="functions"></a><span data-ttu-id="3f6e1-136">函数</span><span class="sxs-lookup"><span data-stu-id="3f6e1-136">Functions</span></span>

<span data-ttu-id="3f6e1-p104">[Excel 函数](#functions)使用 JSON 对象调用使用语法 `POST /workbook/functions/{function-name}` 并在正文中提供函数自变量的工作簿函数。该函数产生 `value`，所有 `error` 字符串均返回到函数结果对象中。`null` 的 `error` 值表示该函数执行成功。</span><span class="sxs-lookup"><span data-stu-id="3f6e1-p104">[Excel functions](#functions): Invoke a workbook function using the syntax `POST /workbook/functions/{function-name}` and providing the function argument(s) in the body using a JSON object. The function's resulting `value` and any `error` strings are returned in the function result object. The `error` value of `null` indicates successful execution of the function.</span></span> 

<span data-ttu-id="3f6e1-p105">受支持函数的完整列表在[此处](https://support.office.com/en-us/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188)。请参阅特定参数名称和数据类型的函数签名。</span><span class="sxs-lookup"><span data-stu-id="3f6e1-p105">The complete list of supported functions are listed [here](https://support.office.com/en-us/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188). Refer to the function signature for specific parameter names and data types.</span></span>

<span data-ttu-id="3f6e1-142">_重要说明_：</span><span class="sxs-lookup"><span data-stu-id="3f6e1-142">_Important notes:_</span></span> 
* <span data-ttu-id="3f6e1-143">使用 range 对象（而不是范围地址字符串）提供范围输入参数。</span><span class="sxs-lookup"><span data-stu-id="3f6e1-143">The range input parameter is supplied using a range object instead of the range address string.</span></span>  
* <span data-ttu-id="3f6e1-144">与大部分 API 中使用的从 0 开始编制的索引不同，索引参数是从 1 开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="3f6e1-144">The index parameter is 1-indexed unlike the 0-index used in most of the APIs.</span></span> 

<span data-ttu-id="3f6e1-145">示例：**vlookup**</span><span class="sxs-lookup"><span data-stu-id="3f6e1-145">Example: **vlookup**</span></span>

<span data-ttu-id="3f6e1-146">在 Excel 电子表格中，`vlookup` 函数需要使用以下参数：</span><span class="sxs-lookup"><span data-stu-id="3f6e1-146">In an Excel spreadsheet, the `vlookup` function takes the following arguments:</span></span>

1. <span data-ttu-id="3f6e1-147">要查找的值（亦称为“查阅值”）。</span><span class="sxs-lookup"><span data-stu-id="3f6e1-147">The value you want to look up, also called the lookup value.</span></span>
2. <span data-ttu-id="3f6e1-148">查阅值所在的区域。</span><span class="sxs-lookup"><span data-stu-id="3f6e1-148">The range where the lookup value is located.</span></span> <span data-ttu-id="3f6e1-149">请注意，查阅值应始终位于区域中的第一列，这样 VLOOKUP 才能正常运行。</span><span class="sxs-lookup"><span data-stu-id="3f6e1-149">Remember that the lookup value should always be in the first column in the range for VLOOKUP to work correctly.</span></span> <span data-ttu-id="3f6e1-150">例如，如果查阅值位于单元格 C2，那么区域应从 C 列开始。</span><span class="sxs-lookup"><span data-stu-id="3f6e1-150">For example, if your lookup value is in cell C2 then your range should start with C.</span></span>
3. <span data-ttu-id="3f6e1-151">包含返回值的区域的列号。</span><span class="sxs-lookup"><span data-stu-id="3f6e1-151">The column number in the range that contains the return value.</span></span> <span data-ttu-id="3f6e1-152">例如，如果指定 B2: D11 作为区域，应将 B 计为第一列，将 C 计为第二列，依此类推。</span><span class="sxs-lookup"><span data-stu-id="3f6e1-152">For example, if you specify B2: D11 as the range, you should count B as the first column, C as the second, and so on.</span></span>
4. <span data-ttu-id="3f6e1-153">（可选）如果想要近似匹配，可指定 TRUE；如果想要返回值的完全匹配，则可指定 FALSE。
</span><span class="sxs-lookup"><span data-stu-id="3f6e1-153">Optionally, you can specify TRUE if you want an approximate match or FALSE if you want an exact match of the return value.</span></span> <span data-ttu-id="3f6e1-154">如果未指定，默认值始终为 TRUE 或近似匹配。</span><span class="sxs-lookup"><span data-stu-id="3f6e1-154">If you don't specify anything, the default value will always be TRUE or approximate match.</span></span>

<span data-ttu-id="3f6e1-155">在单元格中，`vlookup` 函数如下所示：</span><span class="sxs-lookup"><span data-stu-id="3f6e1-155">Inside a cell, the `vlookup` function looks like this:</span></span> 

<span data-ttu-id="3f6e1-156">=VLOOKUP(查阅值, 包含查阅值的区域, 包含返回值的区域的列号, 视需要为近似匹配指定 TRUE 或为完全匹配指定 FALSE)</span><span class="sxs-lookup"><span data-stu-id="3f6e1-156">=VLOOKUP(lookup value, range containing the lookup value, the column number in the range containing the return value, optionally specify TRUE for approximate match or FALSE for an exact match)</span></span>

<span data-ttu-id="3f6e1-157">（请参阅 [VLOOKUP Excel 函数](https://support.office.com/en-us/article/VLOOKUP-function-0bbc8083-26fe-4963-8ab8-93a18ad188a1)文档。）</span><span class="sxs-lookup"><span data-stu-id="3f6e1-157">(See the documentation for the [VLOOKUP Excel function](https://support.office.com/en-us/article/VLOOKUP-function-0bbc8083-26fe-4963-8ab8-93a18ad188a1).)</span></span>

<span data-ttu-id="3f6e1-158">下面的示例展示了如何使用 Excel REST API 调用 `vlookup`  函数，以及一个或多个输入区域。</span><span class="sxs-lookup"><span data-stu-id="3f6e1-158">The example below shows how to call the `vlookup` function and pass these parameters with the Excel REST API.</span></span>
<span data-ttu-id="3f6e1-159">请求：</span><span class="sxs-lookup"><span data-stu-id="3f6e1-159">Request:</span></span> 

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

<span data-ttu-id="3f6e1-160">响应：</span><span class="sxs-lookup"><span data-stu-id="3f6e1-160">Response:</span></span>

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

<span data-ttu-id="3f6e1-161">示例：`median`</span><span class="sxs-lookup"><span data-stu-id="3f6e1-161">Example: `median`</span></span>

<span data-ttu-id="3f6e1-162">在 Excel 电子表格中，`median` 函数需要使用一个或多个输入区域。</span><span class="sxs-lookup"><span data-stu-id="3f6e1-162">In an Excel spreadsheet, the `median` function takes an array of one or more input ranges.</span></span>

<span data-ttu-id="3f6e1-163">在单元格中，`median` 函数如以下示例所示：</span><span class="sxs-lookup"><span data-stu-id="3f6e1-163">Inside a cell, the `median` function looks like this example:</span></span>

<span data-ttu-id="3f6e1-164">=MEDIAN(A2:A6)</span><span class="sxs-lookup"><span data-stu-id="3f6e1-164">=MEDIAN(A2:A6)</span></span>

<span data-ttu-id="3f6e1-165">（请参阅 [MEDIAN Excel 函数](https://support.office.com/en-us/article/MEDIAN-function-d0916313-4753-414c-8537-ce85bdd967d2)文档。）</span><span class="sxs-lookup"><span data-stu-id="3f6e1-165">(See the documentation for the [MEDIAN Excel function](https://support.office.com/en-us/article/MEDIAN-function-d0916313-4753-414c-8537-ce85bdd967d2).)</span></span>

<span data-ttu-id="3f6e1-166">下面的示例展示了如何调用 `median` 函数，以及如何使用 Excel REST API 传递一个或多个输入区域。</span><span class="sxs-lookup"><span data-stu-id="3f6e1-166">The example below shows how to call the `median` function and one or more input ranges with the Excel REST API.</span></span> 

<span data-ttu-id="3f6e1-167">请求：</span><span class="sxs-lookup"><span data-stu-id="3f6e1-167">Request:</span></span> 

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

<span data-ttu-id="3f6e1-168">响应：</span><span class="sxs-lookup"><span data-stu-id="3f6e1-168">Response:</span></span>

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
