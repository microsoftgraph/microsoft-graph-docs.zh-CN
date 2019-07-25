---
title: 'workbookPivotTable: refreshAll'
description: 刷新给定工作表中的数据透视表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 20f9acf22911a216f9fdaf0ef0307c05c90c2655
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35886921"
---
# <a name="workbookpivottable-refreshall"></a><span data-ttu-id="c2f3c-103">workbookPivotTable: refreshAll</span><span class="sxs-lookup"><span data-stu-id="c2f3c-103">workbookPivotTable: refreshAll</span></span>

<span data-ttu-id="c2f3c-104">刷新给定工作表中的数据透视表。</span><span class="sxs-lookup"><span data-stu-id="c2f3c-104">Refreshes the PivotTable within a given worksheet.</span></span>

## <a name="permissions"></a><span data-ttu-id="c2f3c-105">权限</span><span class="sxs-lookup"><span data-stu-id="c2f3c-105">Permissions</span></span>
<span data-ttu-id="c2f3c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c2f3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2f3c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c2f3c-108">Permission type</span></span>      | <span data-ttu-id="c2f3c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c2f3c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2f3c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c2f3c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c2f3c-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c2f3c-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c2f3c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c2f3c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2f3c-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="c2f3c-113">Not supported.</span></span>    |
|<span data-ttu-id="c2f3c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c2f3c-114">Application</span></span> | <span data-ttu-id="c2f3c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c2f3c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c2f3c-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c2f3c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll

```
## <a name="request-headers"></a><span data-ttu-id="c2f3c-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="c2f3c-117">Request headers</span></span>
| <span data-ttu-id="c2f3c-118">名称</span><span class="sxs-lookup"><span data-stu-id="c2f3c-118">Name</span></span>       | <span data-ttu-id="c2f3c-119">说明</span><span class="sxs-lookup"><span data-stu-id="c2f3c-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c2f3c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2f3c-120">Authorization</span></span>  | <span data-ttu-id="c2f3c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c2f3c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c2f3c-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c2f3c-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="c2f3c-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="c2f3c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2f3c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c2f3c-126">Request body</span></span>

### <a name="response"></a><span data-ttu-id="c2f3c-127">响应</span><span class="sxs-lookup"><span data-stu-id="c2f3c-127">Response</span></span>
<span data-ttu-id="c2f3c-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="c2f3c-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2f3c-130">示例</span><span class="sxs-lookup"><span data-stu-id="c2f3c-130">Example</span></span>
<span data-ttu-id="c2f3c-131">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="c2f3c-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c2f3c-132">请求</span><span class="sxs-lookup"><span data-stu-id="c2f3c-132">Request</span></span>
<span data-ttu-id="c2f3c-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c2f3c-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c2f3c-134">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="c2f3c-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refreshall"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c2f3c-135">C#</span><span class="sxs-lookup"><span data-stu-id="c2f3c-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookpivottable-refreshall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c2f3c-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="c2f3c-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookpivottable-refreshall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c2f3c-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="c2f3c-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookpivottable-refreshall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c2f3c-138">Java</span><span class="sxs-lookup"><span data-stu-id="c2f3c-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookpivottable-refreshall-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c2f3c-139">响应</span><span class="sxs-lookup"><span data-stu-id="c2f3c-139">Response</span></span>
<span data-ttu-id="c2f3c-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c2f3c-140">Here is an example of the response.</span></span>
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
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
