---
title: 工作簿资源类型
description: 包含相关的工作簿对象，如工作表、表、区域等。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 83f570301afe4a20aab6f77375e7a575df016d56
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870484"
---
# <a name="workbook-resource-type"></a><span data-ttu-id="2f749-103">工作簿资源类型</span><span class="sxs-lookup"><span data-stu-id="2f749-103">workbook resource type</span></span>

<span data-ttu-id="2f749-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f749-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f749-105">包含相关的工作簿对象，如工作表、表、区域等。</span><span class="sxs-lookup"><span data-stu-id="2f749-105">Contains related workbook objects such as worksheets, tables, ranges, and so on.</span></span>

## <a name="methods"></a><span data-ttu-id="2f749-106">方法</span><span class="sxs-lookup"><span data-stu-id="2f749-106">Methods</span></span>

| <span data-ttu-id="2f749-107">方法</span><span class="sxs-lookup"><span data-stu-id="2f749-107">Method</span></span>       | <span data-ttu-id="2f749-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="2f749-108">Return Type</span></span>  |<span data-ttu-id="2f749-109">说明</span><span class="sxs-lookup"><span data-stu-id="2f749-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2f749-110">创建会话</span><span class="sxs-lookup"><span data-stu-id="2f749-110">Create session</span></span>](../api/workbook-createsession.md) | [<span data-ttu-id="2f749-111">workbookSessionInfo</span><span class="sxs-lookup"><span data-stu-id="2f749-111">workbookSessionInfo</span></span>](workbooksessioninfo.md) |<span data-ttu-id="2f749-112">创建工作簿会话以启动永久或非永久会话。</span><span class="sxs-lookup"><span data-stu-id="2f749-112">Create a workbook session to start a persistent or non-persistent session.</span></span>|
|[<span data-ttu-id="2f749-113">关闭会话</span><span class="sxs-lookup"><span data-stu-id="2f749-113">Close session</span></span>](../api/workbook-closesession.md) | <span data-ttu-id="2f749-114">无</span><span class="sxs-lookup"><span data-stu-id="2f749-114">None</span></span> |<span data-ttu-id="2f749-115">关闭现有会话。</span><span class="sxs-lookup"><span data-stu-id="2f749-115">Close an existing session.</span></span>|
|[<span data-ttu-id="2f749-116">刷新会话</span><span class="sxs-lookup"><span data-stu-id="2f749-116">Refresh session</span></span>](../api/workbook-refreshsession.md) | <span data-ttu-id="2f749-117">无</span><span class="sxs-lookup"><span data-stu-id="2f749-117">None</span></span> |<span data-ttu-id="2f749-118">刷新现有会话。</span><span class="sxs-lookup"><span data-stu-id="2f749-118">Refresh an existing session.</span></span>|

## <a name="properties"></a><span data-ttu-id="2f749-119">属性</span><span class="sxs-lookup"><span data-stu-id="2f749-119">Properties</span></span>
<span data-ttu-id="2f749-120">无。</span><span class="sxs-lookup"><span data-stu-id="2f749-120">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="2f749-121">关系</span><span class="sxs-lookup"><span data-stu-id="2f749-121">Relationships</span></span>
| <span data-ttu-id="2f749-122">关系</span><span class="sxs-lookup"><span data-stu-id="2f749-122">Relationship</span></span> | <span data-ttu-id="2f749-123">类型</span><span class="sxs-lookup"><span data-stu-id="2f749-123">Type</span></span>   |<span data-ttu-id="2f749-124">说明</span><span class="sxs-lookup"><span data-stu-id="2f749-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2f749-125">names</span><span class="sxs-lookup"><span data-stu-id="2f749-125">names</span></span>|<span data-ttu-id="2f749-126">[workbookNamedItem](workbooknameditem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2f749-126">[workbookNamedItem](workbooknameditem.md) collection</span></span> |<span data-ttu-id="2f749-127">代表工作簿范围内命名项目的集合， (范围和常量) 。</span><span class="sxs-lookup"><span data-stu-id="2f749-127">Represents a collection of workbooks scoped named items (named ranges and constants).</span></span> <span data-ttu-id="2f749-128">只读。</span><span class="sxs-lookup"><span data-stu-id="2f749-128">Read-only.</span></span>|
|<span data-ttu-id="2f749-129">表格</span><span class="sxs-lookup"><span data-stu-id="2f749-129">tables</span></span>|<span data-ttu-id="2f749-130">[workbookTable](workbooktable.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2f749-130">[workbookTable](workbooktable.md) collection</span></span> |<span data-ttu-id="2f749-p102">表示与工作簿关联的表的集合。只读。</span><span class="sxs-lookup"><span data-stu-id="2f749-p102">Represents a collection of tables associated with the workbook. Read-only.</span></span>|
|<span data-ttu-id="2f749-133">Worksheets</span><span class="sxs-lookup"><span data-stu-id="2f749-133">worksheets</span></span>|<span data-ttu-id="2f749-134">[workbookWorksheet](workbookworksheet.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2f749-134">[workbookWorksheet](workbookworksheet.md) collection</span></span> |<span data-ttu-id="2f749-p103">表示与工作簿关联的工作表的集合。只读。</span><span class="sxs-lookup"><span data-stu-id="2f749-p103">Represents a collection of worksheets associated with the workbook. Read-only.</span></span>|
|<span data-ttu-id="2f749-137">workbbookApplication</span><span class="sxs-lookup"><span data-stu-id="2f749-137">workbbookApplication</span></span>|[<span data-ttu-id="2f749-138">workbookApplication</span><span class="sxs-lookup"><span data-stu-id="2f749-138">workbookApplication</span></span>](workbookapplication.md) |<span data-ttu-id="2f749-139">表示Excel工作簿的工作簿应用程序。</span><span class="sxs-lookup"><span data-stu-id="2f749-139">Represents the Excel workbookApplication that manages the workbook.</span></span>|
|<span data-ttu-id="2f749-140">operations</span><span class="sxs-lookup"><span data-stu-id="2f749-140">operations</span></span>|<span data-ttu-id="2f749-141">[workbookOperation](workbookoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2f749-141">[workbookOperation](workbookoperation.md) collection</span></span>|<span data-ttu-id="2f749-142">工作簿操作的状态。</span><span class="sxs-lookup"><span data-stu-id="2f749-142">The status of Workbook operations.</span></span> <span data-ttu-id="2f749-143">不支持获取操作集合，但如果响应中返回 `Location` 标头，可以获取长时间运行操作的状态。</span><span class="sxs-lookup"><span data-stu-id="2f749-143">Getting an operation collection is not supported, but you can get the status of a long-running operation if the `Location` header is returned in the response.</span></span> <span data-ttu-id="2f749-144">只读。</span><span class="sxs-lookup"><span data-stu-id="2f749-144">Read-only.</span></span> <span data-ttu-id="2f749-145">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="2f749-145">Nullable.</span></span>|

## <a name="functions"></a><span data-ttu-id="2f749-146">函数</span><span class="sxs-lookup"><span data-stu-id="2f749-146">Functions</span></span>

<span data-ttu-id="2f749-p105">[Excel 函数](#functions)使用 JSON 对象调用使用语法 `POST /me/drive/root/workbook/functions/{function-name}` 并在正文中提供函数自变量的工作簿函数。该函数产生 `value`，所有 `error` 字符串均返回到函数结果对象中。`null` 的 `error` 值表示该函数执行成功。</span><span class="sxs-lookup"><span data-stu-id="2f749-p105">[Excel functions](#functions): Invoke a workbook function using the syntax `POST /me/drive/root/workbook/functions/{function-name}` and providing the function argument(s) in the body using a JSON object. The function's resulting `value` and any `error` strings are returned in the function result object. The `error` value of `null` indicates successful execution of the function.</span></span> 

<span data-ttu-id="2f749-p106">受支持函数的完整列表在 [此处](https://support.office.com/en-us/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188)。请参阅特定参数名称和数据类型的函数签名。</span><span class="sxs-lookup"><span data-stu-id="2f749-p106">The complete list of supported functions are listed [here](https://support.office.com/en-us/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188). Refer to the function signature for specific parameter names and data types.</span></span>

<span data-ttu-id="2f749-152">_重要说明_：</span><span class="sxs-lookup"><span data-stu-id="2f749-152">_Important notes:_</span></span> 
* <span data-ttu-id="2f749-153">使用 range 对象（而不是范围地址字符串）提供范围输入参数。</span><span class="sxs-lookup"><span data-stu-id="2f749-153">The range input parameter is supplied using a range object instead of the range address string.</span></span>  
* <span data-ttu-id="2f749-154">与大部分 API 中使用的从 0 开始编制的索引不同，索引参数是从 1 开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="2f749-154">The index parameter is 1-indexed unlike the 0-index used in most of the APIs.</span></span> 

<span data-ttu-id="2f749-155">示例：**vlookup**</span><span class="sxs-lookup"><span data-stu-id="2f749-155">Example: **vlookup**</span></span>

<span data-ttu-id="2f749-156">在 Excel 电子表格中，`vlookup` 函数需要使用以下参数：</span><span class="sxs-lookup"><span data-stu-id="2f749-156">In an Excel spreadsheet, the `vlookup` function takes the following arguments:</span></span>

1. <span data-ttu-id="2f749-157">要查找的值（亦称为“查阅值”）。</span><span class="sxs-lookup"><span data-stu-id="2f749-157">The value you want to look up, also called the lookup value.</span></span>
2. <span data-ttu-id="2f749-158">查阅值所在的区域。</span><span class="sxs-lookup"><span data-stu-id="2f749-158">The range where the lookup value is located.</span></span> <span data-ttu-id="2f749-159">请注意，查阅值应始终位于区域中的第一列，这样 VLOOKUP 才能正常运行。</span><span class="sxs-lookup"><span data-stu-id="2f749-159">Remember that the lookup value should always be in the first column in the range for VLOOKUP to work correctly.</span></span> <span data-ttu-id="2f749-160">例如，如果查阅值位于单元格 C2，那么区域应从 C 列开始。</span><span class="sxs-lookup"><span data-stu-id="2f749-160">For example, if your lookup value is in cell C2 then your range should start with C.</span></span>
3. <span data-ttu-id="2f749-161">包含返回值的区域的列号。</span><span class="sxs-lookup"><span data-stu-id="2f749-161">The column number in the range that contains the return value.</span></span> <span data-ttu-id="2f749-162">例如，如果指定 B2: D11 作为区域，应将 B 计为第一列，将 C 计为第二列，依此类推。</span><span class="sxs-lookup"><span data-stu-id="2f749-162">For example, if you specify B2: D11 as the range, you should count B as the first column, C as the second, and so on.</span></span>
4. <span data-ttu-id="2f749-163">（可选）如果想要近似匹配，可指定 TRUE；如果想要返回值的完全匹配，则可指定 FALSE。
</span><span class="sxs-lookup"><span data-stu-id="2f749-163">Optionally, you can specify TRUE if you want an approximate match or FALSE if you want an exact match of the return value.</span></span> <span data-ttu-id="2f749-164">如果未指定，默认值始终为 TRUE 或近似匹配。</span><span class="sxs-lookup"><span data-stu-id="2f749-164">If you don't specify anything, the default value will always be TRUE or approximate match.</span></span>

<span data-ttu-id="2f749-165">在单元格中，`vlookup` 函数如下所示：</span><span class="sxs-lookup"><span data-stu-id="2f749-165">Inside a cell, the `vlookup` function looks like this:</span></span> 

<span data-ttu-id="2f749-166">=VLOOKUP(查阅值, 包含查阅值的区域, 包含返回值的区域的列号, 视需要为近似匹配指定 TRUE 或为完全匹配指定 FALSE)</span><span class="sxs-lookup"><span data-stu-id="2f749-166">=VLOOKUP(lookup value, range containing the lookup value, the column number in the range containing the return value, optionally specify TRUE for approximate match or FALSE for an exact match)</span></span>

<span data-ttu-id="2f749-167">（请参阅 [VLOOKUP Excel 函数](https://support.office.com/en-us/article/VLOOKUP-function-0bbc8083-26fe-4963-8ab8-93a18ad188a1)文档。）</span><span class="sxs-lookup"><span data-stu-id="2f749-167">(See the documentation for the [VLOOKUP Excel function](https://support.office.com/en-us/article/VLOOKUP-function-0bbc8083-26fe-4963-8ab8-93a18ad188a1).)</span></span>

<span data-ttu-id="2f749-168">下面的示例展示了如何使用 Excel REST API 调用 `vlookup`  函数，以及一个或多个输入区域。</span><span class="sxs-lookup"><span data-stu-id="2f749-168">The example below shows how to call the `vlookup` function and pass these parameters with the Excel REST API.</span></span>
<span data-ttu-id="2f749-169">请求：</span><span class="sxs-lookup"><span data-stu-id="2f749-169">Request:</span></span> 

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

<span data-ttu-id="2f749-170">响应：</span><span class="sxs-lookup"><span data-stu-id="2f749-170">Response:</span></span>

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

<span data-ttu-id="2f749-171">示例：`median`</span><span class="sxs-lookup"><span data-stu-id="2f749-171">Example: `median`</span></span>

<span data-ttu-id="2f749-172">在 Excel 电子表格中，`median` 函数需要使用一个或多个输入区域。</span><span class="sxs-lookup"><span data-stu-id="2f749-172">In an Excel spreadsheet, the `median` function takes an array of one or more input ranges.</span></span>

<span data-ttu-id="2f749-173">在单元格中，`median` 函数如以下示例所示：</span><span class="sxs-lookup"><span data-stu-id="2f749-173">Inside a cell, the `median` function looks like this example:</span></span>

<span data-ttu-id="2f749-174">=MEDIAN(A2:A6)</span><span class="sxs-lookup"><span data-stu-id="2f749-174">=MEDIAN(A2:A6)</span></span>

<span data-ttu-id="2f749-175">（请参阅 [MEDIAN Excel 函数](https://support.office.com/en-us/article/MEDIAN-function-d0916313-4753-414c-8537-ce85bdd967d2)文档。）</span><span class="sxs-lookup"><span data-stu-id="2f749-175">(See the documentation for the [MEDIAN Excel function](https://support.office.com/en-us/article/MEDIAN-function-d0916313-4753-414c-8537-ce85bdd967d2).)</span></span>

<span data-ttu-id="2f749-176">下面的示例展示了如何调用 `median` 函数，以及如何使用 Excel REST API 传递一个或多个输入区域。</span><span class="sxs-lookup"><span data-stu-id="2f749-176">The example below shows how to call the `median` function and one or more input ranges with the Excel REST API.</span></span> 

<span data-ttu-id="2f749-177">请求：</span><span class="sxs-lookup"><span data-stu-id="2f749-177">Request:</span></span> 

```http 
POST https://graph.microsoft.com/beta/me/drive/root:/book1.xlsx:/workbook/functions/median
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{
   "values":[
      {
         "address":"Sheet2!A1:A5"
      },
      {
         "address":"Sheet2!B1:B5"
      }
   ]
}
```

<span data-ttu-id="2f749-178">响应：</span><span class="sxs-lookup"><span data-stu-id="2f749-178">Response:</span></span>

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
## <a name="json-representation"></a><span data-ttu-id="2f749-179">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2f749-179">JSON representation</span></span>

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


