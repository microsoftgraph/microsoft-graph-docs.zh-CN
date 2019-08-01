---
title: 'ChartFill: clear'
description: 清除图表元素的填充颜色。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 6af09d536c543dd8d5c157490c368eca905ebe07
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36003593"
---
# <a name="chartfill-clear"></a><span data-ttu-id="fc77b-103">ChartFill: clear</span><span class="sxs-lookup"><span data-stu-id="fc77b-103">ChartFill: clear</span></span>

<span data-ttu-id="fc77b-104">清除图表元素的填充颜色。</span><span class="sxs-lookup"><span data-stu-id="fc77b-104">Clear the fill color of a chart element.</span></span>
## <a name="permissions"></a><span data-ttu-id="fc77b-105">权限</span><span class="sxs-lookup"><span data-stu-id="fc77b-105">Permissions</span></span>
<span data-ttu-id="fc77b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fc77b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc77b-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="fc77b-108">Permission type</span></span>      | <span data-ttu-id="fc77b-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fc77b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc77b-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fc77b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fc77b-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fc77b-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fc77b-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fc77b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc77b-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="fc77b-113">Not supported.</span></span>    |
|<span data-ttu-id="fc77b-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="fc77b-114">Application</span></span> | <span data-ttu-id="fc77b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="fc77b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc77b-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fc77b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/format/fill/clear
POST /workbook/worksheets/{id|name}/charts/{name}/title/format/fill/clear
POST /workbook/worksheets/{id|name}/charts/{name}/legend/format/fill/clear

```
## <a name="request-headers"></a><span data-ttu-id="fc77b-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="fc77b-117">Request headers</span></span>
| <span data-ttu-id="fc77b-118">名称</span><span class="sxs-lookup"><span data-stu-id="fc77b-118">Name</span></span>       | <span data-ttu-id="fc77b-119">说明</span><span class="sxs-lookup"><span data-stu-id="fc77b-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fc77b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc77b-120">Authorization</span></span>  | <span data-ttu-id="fc77b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fc77b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fc77b-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="fc77b-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="fc77b-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="fc77b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc77b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="fc77b-126">Request body</span></span>
<span data-ttu-id="fc77b-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fc77b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fc77b-128">响应</span><span class="sxs-lookup"><span data-stu-id="fc77b-128">Response</span></span>

<span data-ttu-id="fc77b-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="fc77b-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc77b-131">示例</span><span class="sxs-lookup"><span data-stu-id="fc77b-131">Example</span></span>
<span data-ttu-id="fc77b-132">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="fc77b-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fc77b-133">请求</span><span class="sxs-lookup"><span data-stu-id="fc77b-133">Request</span></span>
<span data-ttu-id="fc77b-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fc77b-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fc77b-135">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="fc77b-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chartfill_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/format/fill/clear
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fc77b-136">C#</span><span class="sxs-lookup"><span data-stu-id="fc77b-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chartfill-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fc77b-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="fc77b-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chartfill-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fc77b-138">目标-C</span><span class="sxs-lookup"><span data-stu-id="fc77b-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chartfill-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="fc77b-139">Java</span><span class="sxs-lookup"><span data-stu-id="fc77b-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chartfill-clear-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="fc77b-140">响应</span><span class="sxs-lookup"><span data-stu-id="fc77b-140">Response</span></span>
<span data-ttu-id="fc77b-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="fc77b-141">Here is an example of the response.</span></span> 
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
  "description": "ChartFill: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
