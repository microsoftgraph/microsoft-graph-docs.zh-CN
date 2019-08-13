---
title: 'Range: clear'
description: 清除范围值、格式、填充、边框等。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 4de19d90731c79fb85ad3e307e59652da98a81cd
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36375651"
---
# <a name="range-clear"></a><span data-ttu-id="2e4bf-103">Range: clear</span><span class="sxs-lookup"><span data-stu-id="2e4bf-103">Range: clear</span></span>

<span data-ttu-id="2e4bf-104">清除范围值、格式、填充、边框等。</span><span class="sxs-lookup"><span data-stu-id="2e4bf-104">Clear range values, format, fill, border, etc.</span></span>
## <a name="permissions"></a><span data-ttu-id="2e4bf-105">权限</span><span class="sxs-lookup"><span data-stu-id="2e4bf-105">Permissions</span></span>
<span data-ttu-id="2e4bf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2e4bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e4bf-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="2e4bf-108">Permission type</span></span>      | <span data-ttu-id="2e4bf-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2e4bf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2e4bf-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2e4bf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2e4bf-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2e4bf-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2e4bf-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2e4bf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e4bf-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="2e4bf-113">Not supported.</span></span>    |
|<span data-ttu-id="2e4bf-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="2e4bf-114">Application</span></span> | <span data-ttu-id="2e4bf-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2e4bf-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2e4bf-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2e4bf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/clear
POST /workbook/worksheets/{id|name}/range(address='<address>')/clear
POST /workbook/tables/{id|name}/columns/{id|name}/range/clear

```
## <a name="request-headers"></a><span data-ttu-id="2e4bf-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="2e4bf-117">Request headers</span></span>
| <span data-ttu-id="2e4bf-118">名称</span><span class="sxs-lookup"><span data-stu-id="2e4bf-118">Name</span></span>       | <span data-ttu-id="2e4bf-119">说明</span><span class="sxs-lookup"><span data-stu-id="2e4bf-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2e4bf-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e4bf-120">Authorization</span></span>  | <span data-ttu-id="2e4bf-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2e4bf-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2e4bf-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2e4bf-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="2e4bf-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="2e4bf-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e4bf-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2e4bf-126">Request body</span></span>
<span data-ttu-id="2e4bf-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="2e4bf-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2e4bf-128">参数</span><span class="sxs-lookup"><span data-stu-id="2e4bf-128">Parameter</span></span>    | <span data-ttu-id="2e4bf-129">类型</span><span class="sxs-lookup"><span data-stu-id="2e4bf-129">Type</span></span>   |<span data-ttu-id="2e4bf-130">说明</span><span class="sxs-lookup"><span data-stu-id="2e4bf-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2e4bf-131">applyTo</span><span class="sxs-lookup"><span data-stu-id="2e4bf-131">applyTo</span></span>|<span data-ttu-id="2e4bf-132">字符串</span><span class="sxs-lookup"><span data-stu-id="2e4bf-132">string</span></span>|<span data-ttu-id="2e4bf-133">可选。</span><span class="sxs-lookup"><span data-stu-id="2e4bf-133">Optional.</span></span> <span data-ttu-id="2e4bf-134">确定清除操作的类型。</span><span class="sxs-lookup"><span data-stu-id="2e4bf-134">Determines the type of clear action.</span></span>  <span data-ttu-id="2e4bf-135">可能的值包括 `All`、`Formats`、`Contents`。</span><span class="sxs-lookup"><span data-stu-id="2e4bf-135">The possible values are: `All`, `Formats`, `Contents`.</span></span>|

## <a name="response"></a><span data-ttu-id="2e4bf-136">响应</span><span class="sxs-lookup"><span data-stu-id="2e4bf-136">Response</span></span>

<span data-ttu-id="2e4bf-p105">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="2e4bf-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e4bf-139">示例</span><span class="sxs-lookup"><span data-stu-id="2e4bf-139">Example</span></span>
<span data-ttu-id="2e4bf-140">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="2e4bf-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2e4bf-141">请求</span><span class="sxs-lookup"><span data-stu-id="2e4bf-141">Request</span></span>
<span data-ttu-id="2e4bf-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2e4bf-142">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2e4bf-143">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="2e4bf-143">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="2e4bf-144">C#</span><span class="sxs-lookup"><span data-stu-id="2e4bf-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2e4bf-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2e4bf-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2e4bf-146">目标-C</span><span class="sxs-lookup"><span data-stu-id="2e4bf-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2e4bf-147">Java</span><span class="sxs-lookup"><span data-stu-id="2e4bf-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-clear-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2e4bf-148">响应</span><span class="sxs-lookup"><span data-stu-id="2e4bf-148">Response</span></span>
<span data-ttu-id="2e4bf-149">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="2e4bf-149">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
