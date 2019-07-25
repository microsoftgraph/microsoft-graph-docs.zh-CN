---
title: 'ChartFill: setSolidColor'
description: 将图表元素的填充格式设置为统一颜色。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: ad5c8ed36fd541756e281ec03de13bf157aaa005
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35864050"
---
# <a name="chartfill-setsolidcolor"></a><span data-ttu-id="d84f5-103">ChartFill: setSolidColor</span><span class="sxs-lookup"><span data-stu-id="d84f5-103">ChartFill: setSolidColor</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d84f5-104">将图表元素的填充格式设置为统一颜色。</span><span class="sxs-lookup"><span data-stu-id="d84f5-104">Sets the fill formatting of a chart element to a uniform color.</span></span>
## <a name="permissions"></a><span data-ttu-id="d84f5-105">权限</span><span class="sxs-lookup"><span data-stu-id="d84f5-105">Permissions</span></span>
<span data-ttu-id="d84f5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d84f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d84f5-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="d84f5-108">Permission type</span></span>      | <span data-ttu-id="d84f5-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d84f5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d84f5-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d84f5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d84f5-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d84f5-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d84f5-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d84f5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d84f5-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d84f5-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d84f5-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="d84f5-114">Application</span></span> | <span data-ttu-id="d84f5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d84f5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d84f5-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d84f5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/format/fill/setSolidColor
POST /workbook/worksheets/{id|name}/charts/{name}/title/format/fill/setSolidColor
POST /workbook/worksheets/{id|name}/charts/{name}/legend/format/fill/setSolidColor

```
## <a name="request-headers"></a><span data-ttu-id="d84f5-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="d84f5-117">Request headers</span></span>
| <span data-ttu-id="d84f5-118">名称</span><span class="sxs-lookup"><span data-stu-id="d84f5-118">Name</span></span>       | <span data-ttu-id="d84f5-119">说明</span><span class="sxs-lookup"><span data-stu-id="d84f5-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d84f5-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="d84f5-120">Authorization</span></span>  | <span data-ttu-id="d84f5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d84f5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d84f5-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d84f5-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="d84f5-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="d84f5-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d84f5-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d84f5-126">Request body</span></span>
<span data-ttu-id="d84f5-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="d84f5-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d84f5-128">参数</span><span class="sxs-lookup"><span data-stu-id="d84f5-128">Parameter</span></span>    | <span data-ttu-id="d84f5-129">类型</span><span class="sxs-lookup"><span data-stu-id="d84f5-129">Type</span></span>   |<span data-ttu-id="d84f5-130">说明</span><span class="sxs-lookup"><span data-stu-id="d84f5-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d84f5-131">color</span><span class="sxs-lookup"><span data-stu-id="d84f5-131">color</span></span>|<span data-ttu-id="d84f5-132">string</span><span class="sxs-lookup"><span data-stu-id="d84f5-132">string</span></span>|<span data-ttu-id="d84f5-133">表示窗体 #RRGGBB（例如“FFA500”）的边框线条颜色或作为已命名的 HTML 颜色（例如“orange”）的 HTML 颜色代码。</span><span class="sxs-lookup"><span data-stu-id="d84f5-133">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|

## <a name="response"></a><span data-ttu-id="d84f5-134">响应</span><span class="sxs-lookup"><span data-stu-id="d84f5-134">Response</span></span>

<span data-ttu-id="d84f5-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="d84f5-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d84f5-137">示例</span><span class="sxs-lookup"><span data-stu-id="d84f5-137">Example</span></span>
<span data-ttu-id="d84f5-138">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="d84f5-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d84f5-139">请求</span><span class="sxs-lookup"><span data-stu-id="d84f5-139">Request</span></span>
<span data-ttu-id="d84f5-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d84f5-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d84f5-141">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="d84f5-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chartfill_setsolidcolor"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/format/fill/setSolidColor
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d84f5-142">C#</span><span class="sxs-lookup"><span data-stu-id="d84f5-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chartfill-setsolidcolor-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d84f5-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="d84f5-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chartfill-setsolidcolor-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d84f5-144">目标-C</span><span class="sxs-lookup"><span data-stu-id="d84f5-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chartfill-setsolidcolor-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d84f5-145">Java</span><span class="sxs-lookup"><span data-stu-id="d84f5-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chartfill-setsolidcolor-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d84f5-146">响应</span><span class="sxs-lookup"><span data-stu-id="d84f5-146">Response</span></span>
<span data-ttu-id="d84f5-147">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d84f5-147">Here is an example of the response.</span></span> 
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
  "description": "ChartFill: setSolidColor",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
