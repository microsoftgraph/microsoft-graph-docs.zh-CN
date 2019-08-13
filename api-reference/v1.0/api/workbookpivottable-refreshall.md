---
title: 'workbookPivotTable: refreshAll'
description: 刷新给定工作表中的数据透视表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 76689a4f5324f78fb36f3f2612d7fd2b0e09b929
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36365529"
---
# <a name="workbookpivottable-refreshall"></a><span data-ttu-id="e33d1-103">workbookPivotTable: refreshAll</span><span class="sxs-lookup"><span data-stu-id="e33d1-103">workbookPivotTable: refreshAll</span></span>

<span data-ttu-id="e33d1-104">刷新给定工作表中的数据透视表。</span><span class="sxs-lookup"><span data-stu-id="e33d1-104">Refreshes the PivotTable within a given worksheet.</span></span>

## <a name="permissions"></a><span data-ttu-id="e33d1-105">权限</span><span class="sxs-lookup"><span data-stu-id="e33d1-105">Permissions</span></span>
<span data-ttu-id="e33d1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e33d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e33d1-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e33d1-108">Permission type</span></span>      | <span data-ttu-id="e33d1-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e33d1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e33d1-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e33d1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e33d1-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e33d1-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e33d1-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e33d1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e33d1-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="e33d1-113">Not supported.</span></span>    |
|<span data-ttu-id="e33d1-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e33d1-114">Application</span></span> | <span data-ttu-id="e33d1-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e33d1-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e33d1-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e33d1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll

```
## <a name="request-headers"></a><span data-ttu-id="e33d1-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="e33d1-117">Request headers</span></span>
| <span data-ttu-id="e33d1-118">名称</span><span class="sxs-lookup"><span data-stu-id="e33d1-118">Name</span></span>       | <span data-ttu-id="e33d1-119">说明</span><span class="sxs-lookup"><span data-stu-id="e33d1-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e33d1-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e33d1-120">Authorization</span></span>  | <span data-ttu-id="e33d1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e33d1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e33d1-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e33d1-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="e33d1-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="e33d1-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e33d1-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e33d1-126">Request body</span></span>

### <a name="response"></a><span data-ttu-id="e33d1-127">响应</span><span class="sxs-lookup"><span data-stu-id="e33d1-127">Response</span></span>
<span data-ttu-id="e33d1-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="e33d1-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e33d1-130">示例</span><span class="sxs-lookup"><span data-stu-id="e33d1-130">Example</span></span>
<span data-ttu-id="e33d1-131">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="e33d1-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e33d1-132">请求</span><span class="sxs-lookup"><span data-stu-id="e33d1-132">Request</span></span>
<span data-ttu-id="e33d1-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e33d1-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e33d1-134">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="e33d1-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refreshall"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e33d1-135">C#</span><span class="sxs-lookup"><span data-stu-id="e33d1-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookpivottable-refreshall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e33d1-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e33d1-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookpivottable-refreshall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e33d1-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="e33d1-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookpivottable-refreshall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e33d1-138">Java</span><span class="sxs-lookup"><span data-stu-id="e33d1-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookpivottable-refreshall-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e33d1-139">响应</span><span class="sxs-lookup"><span data-stu-id="e33d1-139">Response</span></span>
<span data-ttu-id="e33d1-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e33d1-140">Here is an example of the response.</span></span>
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
