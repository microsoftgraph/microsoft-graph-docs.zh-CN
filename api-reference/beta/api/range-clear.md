---
title: 'Range: clear'
description: 清除范围值、格式、填充、边框等。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 743b26a826db6ecef062e74f64e72f6d55b3b75b
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50577140"
---
# <a name="range-clear"></a><span data-ttu-id="720cc-103">Range: clear</span><span class="sxs-lookup"><span data-stu-id="720cc-103">Range: clear</span></span>

<span data-ttu-id="720cc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="720cc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="720cc-105">清除范围值、格式、填充、边框等。</span><span class="sxs-lookup"><span data-stu-id="720cc-105">Clear range values, format, fill, border, etc.</span></span>
## <a name="permissions"></a><span data-ttu-id="720cc-106">权限</span><span class="sxs-lookup"><span data-stu-id="720cc-106">Permissions</span></span>
<span data-ttu-id="720cc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="720cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="720cc-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="720cc-109">Permission type</span></span>      | <span data-ttu-id="720cc-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="720cc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="720cc-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="720cc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="720cc-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="720cc-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="720cc-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="720cc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="720cc-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="720cc-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="720cc-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="720cc-115">Application</span></span> | <span data-ttu-id="720cc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="720cc-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="720cc-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="720cc-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/names/{name}/range/clear
POST /me/drive/root:/{item-path}:/workbook/names/{name}/range/clear
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/clear
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/clear
POST /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/clear
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/clear

```
## <a name="request-headers"></a><span data-ttu-id="720cc-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="720cc-118">Request headers</span></span>
| <span data-ttu-id="720cc-119">名称</span><span class="sxs-lookup"><span data-stu-id="720cc-119">Name</span></span>       | <span data-ttu-id="720cc-120">说明</span><span class="sxs-lookup"><span data-stu-id="720cc-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="720cc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="720cc-121">Authorization</span></span>  | <span data-ttu-id="720cc-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="720cc-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="720cc-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="720cc-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="720cc-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="720cc-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="720cc-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="720cc-127">Request body</span></span>
<span data-ttu-id="720cc-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="720cc-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="720cc-129">参数</span><span class="sxs-lookup"><span data-stu-id="720cc-129">Parameter</span></span>    | <span data-ttu-id="720cc-130">类型</span><span class="sxs-lookup"><span data-stu-id="720cc-130">Type</span></span>   |<span data-ttu-id="720cc-131">说明</span><span class="sxs-lookup"><span data-stu-id="720cc-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="720cc-132">applyTo</span><span class="sxs-lookup"><span data-stu-id="720cc-132">applyTo</span></span>|<span data-ttu-id="720cc-133">string</span><span class="sxs-lookup"><span data-stu-id="720cc-133">string</span></span>|<span data-ttu-id="720cc-p104">可选。确定清除操作的类型。可能的值是：`All`、`Formats`、`Contents`。</span><span class="sxs-lookup"><span data-stu-id="720cc-p104">Optional. Determines the type of clear action.  Possible values are: `All`, `Formats`, `Contents`.</span></span>|

## <a name="response"></a><span data-ttu-id="720cc-137">响应</span><span class="sxs-lookup"><span data-stu-id="720cc-137">Response</span></span>

<span data-ttu-id="720cc-p105">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="720cc-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="720cc-140">示例</span><span class="sxs-lookup"><span data-stu-id="720cc-140">Example</span></span>
<span data-ttu-id="720cc-141">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="720cc-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="720cc-142">请求</span><span class="sxs-lookup"><span data-stu-id="720cc-142">Request</span></span>
<span data-ttu-id="720cc-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="720cc-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="720cc-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="720cc-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "range_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/clear
Content-type: application/json
Content-length: 32

{
  "applyTo": "applyTo-value"
}
```
# <a name="c"></a>[<span data-ttu-id="720cc-145">C#</span><span class="sxs-lookup"><span data-stu-id="720cc-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="720cc-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="720cc-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="720cc-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="720cc-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="720cc-148">Java</span><span class="sxs-lookup"><span data-stu-id="720cc-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-clear-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="720cc-149">响应</span><span class="sxs-lookup"><span data-stu-id="720cc-149">Response</span></span>
<span data-ttu-id="720cc-150">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="720cc-150">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Range: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


