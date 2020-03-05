---
title: 'Chart: setPosition'
description: 相对于工作表上的单元格放置图表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: eff5a348f1cc4a039a03826be4ecd7ee681cff8b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42439791"
---
# <a name="chart-setposition"></a><span data-ttu-id="6018b-103">Chart: setPosition</span><span class="sxs-lookup"><span data-stu-id="6018b-103">Chart: setPosition</span></span>

<span data-ttu-id="6018b-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="6018b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6018b-105">相对于工作表上的单元格放置图表。</span><span class="sxs-lookup"><span data-stu-id="6018b-105">Positions the chart relative to cells on the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="6018b-106">权限</span><span class="sxs-lookup"><span data-stu-id="6018b-106">Permissions</span></span>
<span data-ttu-id="6018b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6018b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6018b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6018b-109">Permission type</span></span>      | <span data-ttu-id="6018b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6018b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6018b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6018b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6018b-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6018b-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6018b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6018b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6018b-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6018b-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6018b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6018b-115">Application</span></span> | <span data-ttu-id="6018b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6018b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6018b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6018b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/setPosition

```
## <a name="request-headers"></a><span data-ttu-id="6018b-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="6018b-118">Request headers</span></span>
| <span data-ttu-id="6018b-119">名称</span><span class="sxs-lookup"><span data-stu-id="6018b-119">Name</span></span>       | <span data-ttu-id="6018b-120">说明</span><span class="sxs-lookup"><span data-stu-id="6018b-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6018b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6018b-121">Authorization</span></span>  | <span data-ttu-id="6018b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6018b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6018b-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="6018b-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="6018b-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="6018b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6018b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6018b-127">Request body</span></span>
<span data-ttu-id="6018b-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="6018b-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6018b-129">参数</span><span class="sxs-lookup"><span data-stu-id="6018b-129">Parameter</span></span>    | <span data-ttu-id="6018b-130">类型</span><span class="sxs-lookup"><span data-stu-id="6018b-130">Type</span></span>   |<span data-ttu-id="6018b-131">说明</span><span class="sxs-lookup"><span data-stu-id="6018b-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6018b-132">startCell</span><span class="sxs-lookup"><span data-stu-id="6018b-132">startCell</span></span>|<span data-ttu-id="6018b-133">string</span><span class="sxs-lookup"><span data-stu-id="6018b-133">string</span></span>|<span data-ttu-id="6018b-p104">起始单元格。这是图表将移动到的位置。起始单元格为左上角或右上角的单元格，具体取决于用户的从右到左显示设置。</span><span class="sxs-lookup"><span data-stu-id="6018b-p104">The start cell. This is where the chart will be moved to. The start cell is the top-left or top-right cell, depending on the user's right-to-left display settings.</span></span>|
|<span data-ttu-id="6018b-137">endCell</span><span class="sxs-lookup"><span data-stu-id="6018b-137">endCell</span></span>|<span data-ttu-id="6018b-138">string</span><span class="sxs-lookup"><span data-stu-id="6018b-138">string</span></span>|<span data-ttu-id="6018b-p105">可选。结束单元格。如果已指定，图表的宽度和高度将设置为完全覆盖此单元格/区域。</span><span class="sxs-lookup"><span data-stu-id="6018b-p105">Optional. The end cell. If specified, the chart's width and height will be set to fully cover up this cell/range.</span></span>|

## <a name="response"></a><span data-ttu-id="6018b-142">响应</span><span class="sxs-lookup"><span data-stu-id="6018b-142">Response</span></span>

<span data-ttu-id="6018b-p106">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="6018b-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6018b-145">示例</span><span class="sxs-lookup"><span data-stu-id="6018b-145">Example</span></span>
<span data-ttu-id="6018b-146">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="6018b-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6018b-147">请求</span><span class="sxs-lookup"><span data-stu-id="6018b-147">Request</span></span>
<span data-ttu-id="6018b-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6018b-148">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6018b-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="6018b-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chart_setposition"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/setPosition
Content-type: application/json
Content-length: 66

{
  "startCell": "startCell-value",
  "endCell": "endCell-value"
}
```
# <a name="c"></a>[<span data-ttu-id="6018b-150">C#</span><span class="sxs-lookup"><span data-stu-id="6018b-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chart-setposition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6018b-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6018b-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chart-setposition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6018b-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6018b-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chart-setposition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6018b-153">响应</span><span class="sxs-lookup"><span data-stu-id="6018b-153">Response</span></span>
<span data-ttu-id="6018b-154">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6018b-154">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Chart: setPosition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
