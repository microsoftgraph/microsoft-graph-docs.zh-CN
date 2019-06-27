---
title: 'Range: clear'
description: 清除范围值、格式、填充、边框等。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: c14aa5a042f88c6e28c4a7c48a3a1d134ff7d700
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35276067"
---
# <a name="range-clear"></a><span data-ttu-id="dd611-103">Range: clear</span><span class="sxs-lookup"><span data-stu-id="dd611-103">Range: clear</span></span>

<span data-ttu-id="dd611-104">清除范围值、格式、填充、边框等。</span><span class="sxs-lookup"><span data-stu-id="dd611-104">Clear range values, format, fill, border, etc.</span></span>
## <a name="permissions"></a><span data-ttu-id="dd611-105">权限</span><span class="sxs-lookup"><span data-stu-id="dd611-105">Permissions</span></span>
<span data-ttu-id="dd611-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dd611-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd611-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="dd611-108">Permission type</span></span>      | <span data-ttu-id="dd611-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dd611-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd611-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dd611-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dd611-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd611-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dd611-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dd611-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd611-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="dd611-113">Not supported.</span></span>    |
|<span data-ttu-id="dd611-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="dd611-114">Application</span></span> | <span data-ttu-id="dd611-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="dd611-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dd611-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dd611-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/clear
POST /workbook/worksheets/{id|name}/range(address='<address>')/clear
POST /workbook/tables/{id|name}/columns/{id|name}/range/clear

```
## <a name="request-headers"></a><span data-ttu-id="dd611-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="dd611-117">Request headers</span></span>
| <span data-ttu-id="dd611-118">名称</span><span class="sxs-lookup"><span data-stu-id="dd611-118">Name</span></span>       | <span data-ttu-id="dd611-119">说明</span><span class="sxs-lookup"><span data-stu-id="dd611-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="dd611-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd611-120">Authorization</span></span>  | <span data-ttu-id="dd611-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dd611-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dd611-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="dd611-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="dd611-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="dd611-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd611-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="dd611-126">Request body</span></span>
<span data-ttu-id="dd611-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="dd611-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="dd611-128">参数</span><span class="sxs-lookup"><span data-stu-id="dd611-128">Parameter</span></span>    | <span data-ttu-id="dd611-129">类型</span><span class="sxs-lookup"><span data-stu-id="dd611-129">Type</span></span>   |<span data-ttu-id="dd611-130">说明</span><span class="sxs-lookup"><span data-stu-id="dd611-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dd611-131">applyTo</span><span class="sxs-lookup"><span data-stu-id="dd611-131">applyTo</span></span>|<span data-ttu-id="dd611-132">字符串</span><span class="sxs-lookup"><span data-stu-id="dd611-132">string</span></span>|<span data-ttu-id="dd611-133">可选。</span><span class="sxs-lookup"><span data-stu-id="dd611-133">Optional.</span></span> <span data-ttu-id="dd611-134">确定清除操作的类型。</span><span class="sxs-lookup"><span data-stu-id="dd611-134">Determines the type of clear action.</span></span>  <span data-ttu-id="dd611-135">可能的值包括 `All`、`Formats`、`Contents`。</span><span class="sxs-lookup"><span data-stu-id="dd611-135">The possible values are: `All`, `Formats`, `Contents`.</span></span>|

## <a name="response"></a><span data-ttu-id="dd611-136">响应</span><span class="sxs-lookup"><span data-stu-id="dd611-136">Response</span></span>

<span data-ttu-id="dd611-p105">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="dd611-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd611-139">示例</span><span class="sxs-lookup"><span data-stu-id="dd611-139">Example</span></span>
<span data-ttu-id="dd611-140">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="dd611-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="dd611-141">请求</span><span class="sxs-lookup"><span data-stu-id="dd611-141">Request</span></span>
<span data-ttu-id="dd611-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dd611-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/clear
Content-type: application/json
Content-length: 32

{
  "applyTo": "applyTo-value"
}
```

##### <a name="response"></a><span data-ttu-id="dd611-143">响应</span><span class="sxs-lookup"><span data-stu-id="dd611-143">Response</span></span>
<span data-ttu-id="dd611-144">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="dd611-144">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="dd611-145">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="dd611-145">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="dd611-146">C#</span><span class="sxs-lookup"><span data-stu-id="dd611-146">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/range_clear-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dd611-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="dd611-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/range_clear-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="dd611-148">目标-C</span><span class="sxs-lookup"><span data-stu-id="dd611-148">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/range_clear-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/range-clear.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/range-clear.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/range-clear.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
