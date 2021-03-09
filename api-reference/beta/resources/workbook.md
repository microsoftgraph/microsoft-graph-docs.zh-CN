---
title: 工作簿资源类型
description: 包含相关的工作簿对象，如工作表、表、区域等。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 69d04f6ccd5e537c97854abcb1cf2a9c24820a87
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50575705"
---
# <a name="workbook-resource-type"></a><span data-ttu-id="3b429-103">工作簿资源类型</span><span class="sxs-lookup"><span data-stu-id="3b429-103">workbook resource type</span></span>

<span data-ttu-id="3b429-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b429-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3b429-105">包含相关的工作簿对象，如工作表、表、区域等。</span><span class="sxs-lookup"><span data-stu-id="3b429-105">Contains related workbook objects such as worksheets, tables, ranges, and so on.</span></span>

## <a name="methods"></a><span data-ttu-id="3b429-106">方法</span><span class="sxs-lookup"><span data-stu-id="3b429-106">Methods</span></span>

| <span data-ttu-id="3b429-107">方法</span><span class="sxs-lookup"><span data-stu-id="3b429-107">Method</span></span>       | <span data-ttu-id="3b429-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="3b429-108">Return Type</span></span>  |<span data-ttu-id="3b429-109">说明</span><span class="sxs-lookup"><span data-stu-id="3b429-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3b429-110">创建会话</span><span class="sxs-lookup"><span data-stu-id="3b429-110">Create session</span></span>](../api/workbook-createsession.md) | [<span data-ttu-id="3b429-111">workbookSessionInfo</span><span class="sxs-lookup"><span data-stu-id="3b429-111">workbookSessionInfo</span></span>](workbooksessioninfo.md) |<span data-ttu-id="3b429-112">创建工作簿会话以启动永久或非永久会话。</span><span class="sxs-lookup"><span data-stu-id="3b429-112">Create a workbook session to start a persistent or non-persistent session.</span></span>|
|[<span data-ttu-id="3b429-113">关闭会话</span><span class="sxs-lookup"><span data-stu-id="3b429-113">Close session</span></span>](../api/workbook-closesession.md) | <span data-ttu-id="3b429-114">无</span><span class="sxs-lookup"><span data-stu-id="3b429-114">None</span></span> |<span data-ttu-id="3b429-115">关闭现有会话。</span><span class="sxs-lookup"><span data-stu-id="3b429-115">Close an existing session.</span></span>|
|[<span data-ttu-id="3b429-116">刷新会话</span><span class="sxs-lookup"><span data-stu-id="3b429-116">Refresh session</span></span>](../api/workbook-refreshsession.md) | <span data-ttu-id="3b429-117">无</span><span class="sxs-lookup"><span data-stu-id="3b429-117">None</span></span> |<span data-ttu-id="3b429-118">刷新现有会话。</span><span class="sxs-lookup"><span data-stu-id="3b429-118">Refresh an existing session.</span></span>|

## <a name="properties"></a><span data-ttu-id="3b429-119">属性</span><span class="sxs-lookup"><span data-stu-id="3b429-119">Properties</span></span>
<span data-ttu-id="3b429-120">无。</span><span class="sxs-lookup"><span data-stu-id="3b429-120">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="3b429-121">关系</span><span class="sxs-lookup"><span data-stu-id="3b429-121">Relationships</span></span>
| <span data-ttu-id="3b429-122">关系</span><span class="sxs-lookup"><span data-stu-id="3b429-122">Relationship</span></span> | <span data-ttu-id="3b429-123">类型</span><span class="sxs-lookup"><span data-stu-id="3b429-123">Type</span></span>   |<span data-ttu-id="3b429-124">说明</span><span class="sxs-lookup"><span data-stu-id="3b429-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3b429-125">names</span><span class="sxs-lookup"><span data-stu-id="3b429-125">names</span></span>|<span data-ttu-id="3b429-126">[workbookNamedItem](workbooknameditem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3b429-126">[workbookNamedItem](workbooknameditem.md) collection</span></span> |<span data-ttu-id="3b429-p101">表示工作簿范围内的已命名项目（称为区域和常量）的集合。只读。</span><span class="sxs-lookup"><span data-stu-id="3b429-p101">Represents a collection of workbook scoped named items (named ranges and constants). Read-only.</span></span>|
|<span data-ttu-id="3b429-129">表格</span><span class="sxs-lookup"><span data-stu-id="3b429-129">tables</span></span>|<span data-ttu-id="3b429-130">[workbookTable](workbooktable.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3b429-130">[workbookTable](workbooktable.md) collection</span></span> |<span data-ttu-id="3b429-p102">表示与工作簿关联的表的集合。只读。</span><span class="sxs-lookup"><span data-stu-id="3b429-p102">Represents a collection of tables associated with the workbook. Read-only.</span></span>|
|<span data-ttu-id="3b429-133">Worksheets</span><span class="sxs-lookup"><span data-stu-id="3b429-133">worksheets</span></span>|<span data-ttu-id="3b429-134">[workbookWorksheet](workbookworksheet.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3b429-134">[workbookWorksheet](workbookworksheet.md) collection</span></span> |<span data-ttu-id="3b429-135">表示与工作簿关联的工作表的集合。</span><span class="sxs-lookup"><span data-stu-id="3b429-135">Represents a collection of worksheets associated with the workbook.</span></span> <span data-ttu-id="3b429-136">只读。</span><span class="sxs-lookup"><span data-stu-id="3b429-136">Read-only.</span></span>|
|<span data-ttu-id="3b429-137">workbbookApplication</span><span class="sxs-lookup"><span data-stu-id="3b429-137">workbbookApplication</span></span>|[<span data-ttu-id="3b429-138">workbookApplication</span><span class="sxs-lookup"><span data-stu-id="3b429-138">workbookApplication</span></span>](workbookapplication.md) |<span data-ttu-id="3b429-139">代表管理工作簿的 Excel workbookApplication。</span><span class="sxs-lookup"><span data-stu-id="3b429-139">Represents the Excel workbookApplication that manages the workbook.</span></span>|
|<span data-ttu-id="3b429-140">operations</span><span class="sxs-lookup"><span data-stu-id="3b429-140">operations</span></span>|<span data-ttu-id="3b429-141">[workbookOperation](workbookoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3b429-141">[workbookOperation](workbookoperation.md) collection</span></span>|<span data-ttu-id="3b429-142">工作簿操作的状态。</span><span class="sxs-lookup"><span data-stu-id="3b429-142">The status of Workbook operations.</span></span> <span data-ttu-id="3b429-143">不支持获取操作集合，但如果响应中返回 `Location` 标头，可以获取长时间运行操作的状态。</span><span class="sxs-lookup"><span data-stu-id="3b429-143">Getting an operation collection is not supported, but you can get the status of a long-running operation if the `Location` header is returned in the response.</span></span> <span data-ttu-id="3b429-144">只读。</span><span class="sxs-lookup"><span data-stu-id="3b429-144">Read-only.</span></span> <span data-ttu-id="3b429-145">可为空。</span><span class="sxs-lookup"><span data-stu-id="3b429-145">Nullable.</span></span>|

## <a name="functions"></a><span data-ttu-id="3b429-146">函数</span><span class="sxs-lookup"><span data-stu-id="3b429-146">Functions</span></span>

<span data-ttu-id="3b429-p105">[Excel 函数](#functions)使用 JSON 对象调用使用语法 `POST /me/drive/root/workbook/functions/{function-name}` 并在正文中提供函数自变量的工作簿函数。该函数产生 `value`，所有 `error` 字符串均返回到函数结果对象中。`null` 的 `error` 值表示该函数执行成功。</span><span class="sxs-lookup"><span data-stu-id="3b429-p105">[Excel functions](#functions): Invoke a workbook function using the syntax `POST /me/drive/root/workbook/functions/{function-name}` and providing the function argument(s) in the body using a JSON object. The function's resulting `value` and any `error` strings are returned in the function result object. The `error` value of `null` indicates successful execution of the function.</span></span> 

<span data-ttu-id="3b429-p106">受支持函数的完整列表在 [此处](https://support.office.com/en-us/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188)。请参阅特定参数名称和数据类型的函数签名。</span><span class="sxs-lookup"><span data-stu-id="3b429-p106">The complete list of supported functions are listed [here](https://support.office.com/en-us/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188). Refer to the function signature for specific parameter names and data types.</span></span>

<span data-ttu-id="3b429-152">_重要说明_：</span><span class="sxs-lookup"><span data-stu-id="3b429-152">_Important notes:_</span></span> 
* <span data-ttu-id="3b429-153">使用 range 对象（而不是范围地址字符串）提供范围输入参数。</span><span class="sxs-lookup"><span data-stu-id="3b429-153">The range input parameter is supplied using a range object instead of the range address string.</span></span>  
* <span data-ttu-id="3b429-154">与大部分 API 中使用的从 0 开始编制的索引不同，索引参数是从 1 开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="3b429-154">The index parameter is 1-indexed unlike the 0-index used in most of the APIs.</span></span> 

<span data-ttu-id="3b429-155">示例：**vlookup**</span><span class="sxs-lookup"><span data-stu-id="3b429-155">Example: **vlookup**</span></span>

<span data-ttu-id="3b429-156">在 Excel 电子表格中，`vlookup` 函数需要使用以下参数：</span><span class="sxs-lookup"><span data-stu-id="3b429-156">In an Excel spreadsheet, the `vlookup` function takes the following arguments:</span></span>

1. <span data-ttu-id="3b429-157">要查找的值（亦称为“查阅值”）。</span><span class="sxs-lookup"><span data-stu-id="3b429-157">The value you want to look up, also called the lookup value.</span></span>
2. <span data-ttu-id="3b429-158">查阅值所在的区域。</span><span class="sxs-lookup"><span data-stu-id="3b429-158">The range where the lookup value is located.</span></span> <span data-ttu-id="3b429-159">请注意，查阅值应始终位于区域中的第一列，这样 VLOOKUP 才能正常运行。</span><span class="sxs-lookup"><span data-stu-id="3b429-159">Remember that the lookup value should always be in the first column in the range for VLOOKUP to work correctly.</span></span> <span data-ttu-id="3b429-160">例如，如果查阅值位于单元格 C2，那么区域应从 C 列开始。</span><span class="sxs-lookup"><span data-stu-id="3b429-160">For example, if your lookup value is in cell C2 then your range should start with C.</span></span>
3. <span data-ttu-id="3b429-161">包含返回值的区域的列号。</span><span class="sxs-lookup"><span data-stu-id="3b429-161">The column number in the range that contains the return value.</span></span> <span data-ttu-id="3b429-162">例如，如果指定 B2: D11 作为区域，应将 B 计为第一列，将 C 计为第二列，依此类推。</span><span class="sxs-lookup"><span data-stu-id="3b429-162">For example, if you specify B2: D11 as the range, you should count B as the first column, C as the second, and so on.</span></span>
4. <span data-ttu-id="3b429-163">（可选）如果想要近似匹配，可指定 TRUE；如果想要返回值的完全匹配，则可指定 FALSE。
</span><span class="sxs-lookup"><span data-stu-id="3b429-163">Optionally, you can specify TRUE if you want an approximate match or FALSE if you want an exact match of the return value.</span></span> <span data-ttu-id="3b429-164">如果未指定，默认值始终为 TRUE 或近似匹配。</span><span class="sxs-lookup"><span data-stu-id="3b429-164">If you don't specify anything, the default value will always be TRUE or approximate match.</span></span>

<span data-ttu-id="3b429-165">在单元格中，`vlookup` 函数如下所示：</span><span class="sxs-lookup"><span data-stu-id="3b429-165">Inside a cell, the `vlookup` function looks like this:</span></span> 

<span data-ttu-id="3b429-166">=VLOOKUP(查阅值, 包含查阅值的区域, 包含返回值的区域的列号, 视需要为近似匹配指定 TRUE 或为完全匹配指定 FALSE)</span><span class="sxs-lookup"><span data-stu-id="3b429-166">=VLOOKUP(lookup value, range containing the lookup value, the column number in the range containing the return value, optionally specify TRUE for approximate match or FALSE for an exact match)</span></span>

<span data-ttu-id="3b429-167">（请参阅 [VLOOKUP Excel 函数](https://support.office.com/en-us/article/VLOOKUP-function-0bbc8083-26fe-4963-8ab8-93a18ad188a1)文档。）</span><span class="sxs-lookup"><span data-stu-id="3b429-167">(See the documentation for the [VLOOKUP Excel function](https://support.office.com/en-us/article/VLOOKUP-function-0bbc8083-26fe-4963-8ab8-93a18ad188a1).)</span></span>

<span data-ttu-id="3b429-168">下面的示例展示了如何使用 Excel REST API 调用 `vlookup`  函数，以及一个或多个输入区域。</span><span class="sxs-lookup"><span data-stu-id="3b429-168">The example below shows how to call the `vlookup` function and pass these parameters with the Excel REST API.</span></span>
<span data-ttu-id="3b429-169">请求：</span><span class="sxs-lookup"><span data-stu-id="3b429-169">Request:</span></span> 

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

<span data-ttu-id="3b429-170">响应：</span><span class="sxs-lookup"><span data-stu-id="3b429-170">Response:</span></span>

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

<span data-ttu-id="3b429-171">示例：`median`</span><span class="sxs-lookup"><span data-stu-id="3b429-171">Example: `median`</span></span>

<span data-ttu-id="3b429-172">在 Excel 电子表格中，`median` 函数需要使用一个或多个输入区域。</span><span class="sxs-lookup"><span data-stu-id="3b429-172">In an Excel spreadsheet, the `median` function takes an array of one or more input ranges.</span></span>

<span data-ttu-id="3b429-173">在单元格中，`median` 函数如以下示例所示：</span><span class="sxs-lookup"><span data-stu-id="3b429-173">Inside a cell, the `median` function looks like this example:</span></span>

<span data-ttu-id="3b429-174">=MEDIAN(A2:A6)</span><span class="sxs-lookup"><span data-stu-id="3b429-174">=MEDIAN(A2:A6)</span></span>

<span data-ttu-id="3b429-175">（请参阅 [MEDIAN Excel 函数](https://support.office.com/en-us/article/MEDIAN-function-d0916313-4753-414c-8537-ce85bdd967d2)文档。）</span><span class="sxs-lookup"><span data-stu-id="3b429-175">(See the documentation for the [MEDIAN Excel function](https://support.office.com/en-us/article/MEDIAN-function-d0916313-4753-414c-8537-ce85bdd967d2).)</span></span>

<span data-ttu-id="3b429-176">下面的示例展示了如何调用 `median` 函数，以及如何使用 Excel REST API 传递一个或多个输入区域。</span><span class="sxs-lookup"><span data-stu-id="3b429-176">The example below shows how to call the `median` function and one or more input ranges with the Excel REST API.</span></span> 

<span data-ttu-id="3b429-177">请求：</span><span class="sxs-lookup"><span data-stu-id="3b429-177">Request:</span></span> 

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

<span data-ttu-id="3b429-178">响应：</span><span class="sxs-lookup"><span data-stu-id="3b429-178">Response:</span></span>

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
## <a name="json-representation"></a><span data-ttu-id="3b429-179">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3b429-179">JSON representation</span></span>

<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
  "@odata.type": "microsoft.graph.workbook"
}-->
``` json
{
    "id": "string"
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


