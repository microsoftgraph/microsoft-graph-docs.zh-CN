---
title: 'RangeFormat: autofitColumns'
description: 根据列中的当前数据更改当前范围的列宽，以达到最佳宽度。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 1bd731ce30ce4fcd87d2bfc542208f8252774ddf
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36412031"
---
# <a name="rangeformat-autofitcolumns"></a><span data-ttu-id="00350-103">RangeFormat: autofitColumns</span><span class="sxs-lookup"><span data-stu-id="00350-103">RangeFormat: autofitColumns</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00350-104">根据列中的当前数据更改当前范围的列宽，以达到最佳宽度。</span><span class="sxs-lookup"><span data-stu-id="00350-104">Changes the width of the columns of the current range to achieve the best fit, based on the current data in the columns.</span></span>
## <a name="permissions"></a><span data-ttu-id="00350-105">权限</span><span class="sxs-lookup"><span data-stu-id="00350-105">Permissions</span></span>
<span data-ttu-id="00350-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="00350-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00350-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="00350-108">Permission type</span></span>      | <span data-ttu-id="00350-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="00350-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="00350-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="00350-110">Delegated (work or school account)</span></span> | <span data-ttu-id="00350-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00350-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="00350-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="00350-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00350-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00350-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="00350-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="00350-114">Application</span></span> | <span data-ttu-id="00350-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="00350-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="00350-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="00350-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/format/autofitColumns
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/autofitColumns
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/autofitColumns

```
## <a name="request-headers"></a><span data-ttu-id="00350-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="00350-117">Request headers</span></span>
| <span data-ttu-id="00350-118">名称</span><span class="sxs-lookup"><span data-stu-id="00350-118">Name</span></span>       | <span data-ttu-id="00350-119">说明</span><span class="sxs-lookup"><span data-stu-id="00350-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="00350-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="00350-120">Authorization</span></span>  | <span data-ttu-id="00350-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="00350-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="00350-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="00350-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="00350-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="00350-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="00350-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="00350-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="00350-127">响应</span><span class="sxs-lookup"><span data-stu-id="00350-127">Response</span></span>

<span data-ttu-id="00350-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="00350-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00350-130">示例</span><span class="sxs-lookup"><span data-stu-id="00350-130">Example</span></span>
<span data-ttu-id="00350-131">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="00350-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="00350-132">请求</span><span class="sxs-lookup"><span data-stu-id="00350-132">Request</span></span>
<span data-ttu-id="00350-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="00350-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="00350-134">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="00350-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "rangeformat_autofitcolumns"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/format/autofitColumns
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="00350-135">C#</span><span class="sxs-lookup"><span data-stu-id="00350-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/rangeformat-autofitcolumns-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="00350-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="00350-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/rangeformat-autofitcolumns-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="00350-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="00350-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/rangeformat-autofitcolumns-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="00350-138">响应</span><span class="sxs-lookup"><span data-stu-id="00350-138">Response</span></span>
<span data-ttu-id="00350-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="00350-139">Here is an example of the response.</span></span> 
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
  "description": "RangeFormat: autofitColumns",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
