---
title: 'Chart: setPosition'
description: 相对于工作表上的单元格放置图表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 77e9718ce7d03292c6cee60d3face2c216e11b88
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36003810"
---
# <a name="chart-setposition"></a><span data-ttu-id="e7a37-103">Chart: setPosition</span><span class="sxs-lookup"><span data-stu-id="e7a37-103">Chart: setPosition</span></span>

<span data-ttu-id="e7a37-104">相对于工作表上的单元格放置图表。</span><span class="sxs-lookup"><span data-stu-id="e7a37-104">Positions the chart relative to cells on the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="e7a37-105">权限</span><span class="sxs-lookup"><span data-stu-id="e7a37-105">Permissions</span></span>
<span data-ttu-id="e7a37-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e7a37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7a37-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e7a37-108">Permission type</span></span>      | <span data-ttu-id="e7a37-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e7a37-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e7a37-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e7a37-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e7a37-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e7a37-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e7a37-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e7a37-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7a37-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="e7a37-113">Not supported.</span></span>    |
|<span data-ttu-id="e7a37-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e7a37-114">Application</span></span> | <span data-ttu-id="e7a37-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e7a37-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e7a37-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e7a37-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/setPosition

```
## <a name="request-headers"></a><span data-ttu-id="e7a37-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="e7a37-117">Request headers</span></span>
| <span data-ttu-id="e7a37-118">名称</span><span class="sxs-lookup"><span data-stu-id="e7a37-118">Name</span></span>       | <span data-ttu-id="e7a37-119">说明</span><span class="sxs-lookup"><span data-stu-id="e7a37-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e7a37-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7a37-120">Authorization</span></span>  | <span data-ttu-id="e7a37-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e7a37-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e7a37-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e7a37-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="e7a37-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="e7a37-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7a37-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e7a37-126">Request body</span></span>
<span data-ttu-id="e7a37-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="e7a37-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e7a37-128">参数</span><span class="sxs-lookup"><span data-stu-id="e7a37-128">Parameter</span></span>    | <span data-ttu-id="e7a37-129">类型</span><span class="sxs-lookup"><span data-stu-id="e7a37-129">Type</span></span>   |<span data-ttu-id="e7a37-130">说明</span><span class="sxs-lookup"><span data-stu-id="e7a37-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e7a37-131">startCell</span><span class="sxs-lookup"><span data-stu-id="e7a37-131">startCell</span></span>|<span data-ttu-id="e7a37-132">Json</span><span class="sxs-lookup"><span data-stu-id="e7a37-132">Json</span></span>|<span data-ttu-id="e7a37-p104">起始单元格。这是图表将移动到的位置。起始单元格为左上角或右上角的单元格，具体取决于用户的从右到左显示设置。</span><span class="sxs-lookup"><span data-stu-id="e7a37-p104">The start cell. This is where the chart will be moved to. The start cell is the top-left or top-right cell, depending on the user's right-to-left display settings.</span></span>|
|<span data-ttu-id="e7a37-136">endCell</span><span class="sxs-lookup"><span data-stu-id="e7a37-136">endCell</span></span>|<span data-ttu-id="e7a37-137">Json</span><span class="sxs-lookup"><span data-stu-id="e7a37-137">Json</span></span>|<span data-ttu-id="e7a37-p105">可选。结束单元格。如果已指定，图表的宽度和高度将设置为完全覆盖此单元格/区域。</span><span class="sxs-lookup"><span data-stu-id="e7a37-p105">Optional. The end cell. If specified, the chart's width and height will be set to fully cover up this cell/range.</span></span>|

## <a name="response"></a><span data-ttu-id="e7a37-141">响应</span><span class="sxs-lookup"><span data-stu-id="e7a37-141">Response</span></span>

<span data-ttu-id="e7a37-p106">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="e7a37-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7a37-144">示例</span><span class="sxs-lookup"><span data-stu-id="e7a37-144">Example</span></span>
<span data-ttu-id="e7a37-145">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="e7a37-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e7a37-146">请求</span><span class="sxs-lookup"><span data-stu-id="e7a37-146">Request</span></span>
<span data-ttu-id="e7a37-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e7a37-147">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e7a37-148">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="e7a37-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chart_setposition"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/setPosition
Content-type: application/json
Content-length: 66

{
  "startCell": "startCell-value",
  "endCell": "endCell-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e7a37-149">C#</span><span class="sxs-lookup"><span data-stu-id="e7a37-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chart-setposition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e7a37-150">Javascript</span><span class="sxs-lookup"><span data-stu-id="e7a37-150">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chart-setposition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e7a37-151">目标-C</span><span class="sxs-lookup"><span data-stu-id="e7a37-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chart-setposition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e7a37-152">Java</span><span class="sxs-lookup"><span data-stu-id="e7a37-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chart-setposition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e7a37-153">响应</span><span class="sxs-lookup"><span data-stu-id="e7a37-153">Response</span></span>
<span data-ttu-id="e7a37-154">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e7a37-154">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chart: setPosition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
