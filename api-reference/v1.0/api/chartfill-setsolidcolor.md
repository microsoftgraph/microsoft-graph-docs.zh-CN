---
title: 'ChartFill: setSolidColor'
description: 将图表元素的填充格式设置为统一颜色。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 4f230d15f66e7a56e43328c9f71d5b70230b9d58
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36003565"
---
# <a name="chartfill-setsolidcolor"></a><span data-ttu-id="6bc7d-103">ChartFill: setSolidColor</span><span class="sxs-lookup"><span data-stu-id="6bc7d-103">ChartFill: setSolidColor</span></span>

<span data-ttu-id="6bc7d-104">将图表元素的填充格式设置为统一颜色。</span><span class="sxs-lookup"><span data-stu-id="6bc7d-104">Sets the fill formatting of a chart element to a uniform color.</span></span>
## <a name="permissions"></a><span data-ttu-id="6bc7d-105">权限</span><span class="sxs-lookup"><span data-stu-id="6bc7d-105">Permissions</span></span>
<span data-ttu-id="6bc7d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6bc7d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6bc7d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="6bc7d-108">Permission type</span></span>      | <span data-ttu-id="6bc7d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6bc7d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6bc7d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6bc7d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6bc7d-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6bc7d-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6bc7d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6bc7d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6bc7d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="6bc7d-113">Not supported.</span></span>    |
|<span data-ttu-id="6bc7d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="6bc7d-114">Application</span></span> | <span data-ttu-id="6bc7d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6bc7d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6bc7d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6bc7d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/format/fill/setSolidColor
POST /workbook/worksheets/{id|name}/charts/{name}/title/format/fill/setSolidColor
POST /workbook/worksheets/{id|name}/charts/{name}/legend/format/fill/setSolidColor

```
## <a name="request-headers"></a><span data-ttu-id="6bc7d-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="6bc7d-117">Request headers</span></span>
| <span data-ttu-id="6bc7d-118">名称</span><span class="sxs-lookup"><span data-stu-id="6bc7d-118">Name</span></span>       | <span data-ttu-id="6bc7d-119">说明</span><span class="sxs-lookup"><span data-stu-id="6bc7d-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6bc7d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="6bc7d-120">Authorization</span></span>  | <span data-ttu-id="6bc7d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6bc7d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6bc7d-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="6bc7d-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="6bc7d-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="6bc7d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6bc7d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6bc7d-126">Request body</span></span>
<span data-ttu-id="6bc7d-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="6bc7d-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6bc7d-128">参数</span><span class="sxs-lookup"><span data-stu-id="6bc7d-128">Parameter</span></span>    | <span data-ttu-id="6bc7d-129">类型</span><span class="sxs-lookup"><span data-stu-id="6bc7d-129">Type</span></span>   |<span data-ttu-id="6bc7d-130">说明</span><span class="sxs-lookup"><span data-stu-id="6bc7d-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6bc7d-131">color</span><span class="sxs-lookup"><span data-stu-id="6bc7d-131">color</span></span>|<span data-ttu-id="6bc7d-132">string</span><span class="sxs-lookup"><span data-stu-id="6bc7d-132">string</span></span>|<span data-ttu-id="6bc7d-133">表示窗体 #RRGGBB（例如“FFA500”）的边框线条颜色或作为已命名的 HTML 颜色（例如“orange”）的 HTML 颜色代码。</span><span class="sxs-lookup"><span data-stu-id="6bc7d-133">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|

## <a name="response"></a><span data-ttu-id="6bc7d-134">响应</span><span class="sxs-lookup"><span data-stu-id="6bc7d-134">Response</span></span>

<span data-ttu-id="6bc7d-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="6bc7d-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6bc7d-137">示例</span><span class="sxs-lookup"><span data-stu-id="6bc7d-137">Example</span></span>
<span data-ttu-id="6bc7d-138">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="6bc7d-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6bc7d-139">请求</span><span class="sxs-lookup"><span data-stu-id="6bc7d-139">Request</span></span>
<span data-ttu-id="6bc7d-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6bc7d-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6bc7d-141">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="6bc7d-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chartfill_setsolidcolor"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/format/fill/setSolidColor
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6bc7d-142">C#</span><span class="sxs-lookup"><span data-stu-id="6bc7d-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chartfill-setsolidcolor-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6bc7d-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="6bc7d-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chartfill-setsolidcolor-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6bc7d-144">目标-C</span><span class="sxs-lookup"><span data-stu-id="6bc7d-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chartfill-setsolidcolor-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6bc7d-145">Java</span><span class="sxs-lookup"><span data-stu-id="6bc7d-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chartfill-setsolidcolor-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6bc7d-146">响应</span><span class="sxs-lookup"><span data-stu-id="6bc7d-146">Response</span></span>
<span data-ttu-id="6bc7d-147">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6bc7d-147">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartFill: setSolidColor",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
