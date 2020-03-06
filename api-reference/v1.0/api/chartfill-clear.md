---
title: 'ChartFill: clear'
description: 清除图表元素的填充颜色。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 2a0af0d1f6ca706bfd723093125b0a085cc7342e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518467"
---
# <a name="chartfill-clear"></a><span data-ttu-id="cdfdd-103">ChartFill: clear</span><span class="sxs-lookup"><span data-stu-id="cdfdd-103">ChartFill: clear</span></span>

<span data-ttu-id="cdfdd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cdfdd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cdfdd-105">清除图表元素的填充颜色。</span><span class="sxs-lookup"><span data-stu-id="cdfdd-105">Clear the fill color of a chart element.</span></span>
## <a name="permissions"></a><span data-ttu-id="cdfdd-106">权限</span><span class="sxs-lookup"><span data-stu-id="cdfdd-106">Permissions</span></span>
<span data-ttu-id="cdfdd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cdfdd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdfdd-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cdfdd-109">Permission type</span></span>      | <span data-ttu-id="cdfdd-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cdfdd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cdfdd-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cdfdd-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cdfdd-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cdfdd-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cdfdd-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cdfdd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cdfdd-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="cdfdd-114">Not supported.</span></span>    |
|<span data-ttu-id="cdfdd-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="cdfdd-115">Application</span></span> | <span data-ttu-id="cdfdd-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cdfdd-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cdfdd-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cdfdd-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/format/fill/clear
POST /workbook/worksheets/{id|name}/charts/{name}/title/format/fill/clear
POST /workbook/worksheets/{id|name}/charts/{name}/legend/format/fill/clear

```
## <a name="request-headers"></a><span data-ttu-id="cdfdd-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="cdfdd-118">Request headers</span></span>
| <span data-ttu-id="cdfdd-119">名称</span><span class="sxs-lookup"><span data-stu-id="cdfdd-119">Name</span></span>       | <span data-ttu-id="cdfdd-120">说明</span><span class="sxs-lookup"><span data-stu-id="cdfdd-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cdfdd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cdfdd-121">Authorization</span></span>  | <span data-ttu-id="cdfdd-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cdfdd-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cdfdd-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="cdfdd-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="cdfdd-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="cdfdd-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cdfdd-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="cdfdd-127">Request body</span></span>
<span data-ttu-id="cdfdd-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cdfdd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cdfdd-129">响应</span><span class="sxs-lookup"><span data-stu-id="cdfdd-129">Response</span></span>

<span data-ttu-id="cdfdd-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="cdfdd-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cdfdd-132">示例</span><span class="sxs-lookup"><span data-stu-id="cdfdd-132">Example</span></span>
<span data-ttu-id="cdfdd-133">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="cdfdd-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="cdfdd-134">请求</span><span class="sxs-lookup"><span data-stu-id="cdfdd-134">Request</span></span>
<span data-ttu-id="cdfdd-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cdfdd-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cdfdd-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="cdfdd-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chartfill_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/format/fill/clear
```
# <a name="c"></a>[<span data-ttu-id="cdfdd-137">C#</span><span class="sxs-lookup"><span data-stu-id="cdfdd-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chartfill-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cdfdd-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cdfdd-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chartfill-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cdfdd-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cdfdd-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chartfill-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cdfdd-140">Java</span><span class="sxs-lookup"><span data-stu-id="cdfdd-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chartfill-clear-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="cdfdd-141">响应</span><span class="sxs-lookup"><span data-stu-id="cdfdd-141">Response</span></span>
<span data-ttu-id="cdfdd-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="cdfdd-142">Here is an example of the response.</span></span> 
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
