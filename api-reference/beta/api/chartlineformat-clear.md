---
title: 'ChartLineFormat: clear'
description: 清除图表元素的线条格式。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 9f0fc8a4f429ec0e3b05b452e2bff3abb177458f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42439231"
---
# <a name="chartlineformat-clear"></a><span data-ttu-id="324db-103">ChartLineFormat: clear</span><span class="sxs-lookup"><span data-stu-id="324db-103">ChartLineFormat: clear</span></span>

<span data-ttu-id="324db-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="324db-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="324db-105">清除图表元素的线条格式。</span><span class="sxs-lookup"><span data-stu-id="324db-105">Clear the line format of a chart element.</span></span>
## <a name="permissions"></a><span data-ttu-id="324db-106">权限</span><span class="sxs-lookup"><span data-stu-id="324db-106">Permissions</span></span>
<span data-ttu-id="324db-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="324db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="324db-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="324db-109">Permission type</span></span>      | <span data-ttu-id="324db-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="324db-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="324db-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="324db-111">Delegated (work or school account)</span></span> | <span data-ttu-id="324db-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="324db-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="324db-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="324db-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="324db-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="324db-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="324db-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="324db-115">Application</span></span> | <span data-ttu-id="324db-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="324db-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="324db-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="324db-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/format/line/clear
POST /workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/format/line/clear
POST /workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/majorgridlines/format/line/clear

```
## <a name="request-headers"></a><span data-ttu-id="324db-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="324db-118">Request headers</span></span>
| <span data-ttu-id="324db-119">名称</span><span class="sxs-lookup"><span data-stu-id="324db-119">Name</span></span>       | <span data-ttu-id="324db-120">说明</span><span class="sxs-lookup"><span data-stu-id="324db-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="324db-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="324db-121">Authorization</span></span>  | <span data-ttu-id="324db-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="324db-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="324db-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="324db-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="324db-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="324db-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="324db-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="324db-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="324db-128">响应</span><span class="sxs-lookup"><span data-stu-id="324db-128">Response</span></span>

<span data-ttu-id="324db-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="324db-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="324db-131">示例</span><span class="sxs-lookup"><span data-stu-id="324db-131">Example</span></span>
<span data-ttu-id="324db-132">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="324db-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="324db-133">请求</span><span class="sxs-lookup"><span data-stu-id="324db-133">Request</span></span>
<span data-ttu-id="324db-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="324db-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="324db-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="324db-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chartlineformat_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/format/line/clear
```
# <a name="c"></a>[<span data-ttu-id="324db-136">C#</span><span class="sxs-lookup"><span data-stu-id="324db-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chartlineformat-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="324db-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="324db-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chartlineformat-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="324db-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="324db-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chartlineformat-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="324db-139">响应</span><span class="sxs-lookup"><span data-stu-id="324db-139">Response</span></span>
<span data-ttu-id="324db-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="324db-140">Here is an example of the response.</span></span> 
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
  "description": "ChartLineFormat: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
