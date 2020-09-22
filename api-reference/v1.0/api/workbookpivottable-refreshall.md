---
title: 'workbookPivotTable: refreshAll'
description: 刷新给定工作表中的数据透视表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 9643ad87deea9425ebdf3edb4a74d71dba7a5038
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47984556"
---
# <a name="workbookpivottable-refreshall"></a><span data-ttu-id="c96d0-103">workbookPivotTable: refreshAll</span><span class="sxs-lookup"><span data-stu-id="c96d0-103">workbookPivotTable: refreshAll</span></span>

<span data-ttu-id="c96d0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c96d0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c96d0-105">刷新给定工作表中的数据透视表。</span><span class="sxs-lookup"><span data-stu-id="c96d0-105">Refreshes the PivotTable within a given worksheet.</span></span>

## <a name="permissions"></a><span data-ttu-id="c96d0-106">权限</span><span class="sxs-lookup"><span data-stu-id="c96d0-106">Permissions</span></span>
<span data-ttu-id="c96d0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c96d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c96d0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c96d0-109">Permission type</span></span>      | <span data-ttu-id="c96d0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c96d0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c96d0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c96d0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c96d0-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c96d0-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c96d0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c96d0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c96d0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c96d0-114">Not supported.</span></span>    |
|<span data-ttu-id="c96d0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c96d0-115">Application</span></span> | <span data-ttu-id="c96d0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c96d0-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c96d0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c96d0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll

```
## <a name="request-headers"></a><span data-ttu-id="c96d0-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="c96d0-118">Request headers</span></span>
| <span data-ttu-id="c96d0-119">名称</span><span class="sxs-lookup"><span data-stu-id="c96d0-119">Name</span></span>       | <span data-ttu-id="c96d0-120">说明</span><span class="sxs-lookup"><span data-stu-id="c96d0-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c96d0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c96d0-121">Authorization</span></span>  | <span data-ttu-id="c96d0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c96d0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c96d0-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c96d0-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="c96d0-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="c96d0-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c96d0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c96d0-127">Request body</span></span>

### <a name="response"></a><span data-ttu-id="c96d0-128">响应</span><span class="sxs-lookup"><span data-stu-id="c96d0-128">Response</span></span>
<span data-ttu-id="c96d0-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="c96d0-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c96d0-131">示例</span><span class="sxs-lookup"><span data-stu-id="c96d0-131">Example</span></span>
<span data-ttu-id="c96d0-132">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="c96d0-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c96d0-133">请求</span><span class="sxs-lookup"><span data-stu-id="c96d0-133">Request</span></span>
<span data-ttu-id="c96d0-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c96d0-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c96d0-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="c96d0-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refreshall"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll
```
# <a name="c"></a>[<span data-ttu-id="c96d0-136">C#</span><span class="sxs-lookup"><span data-stu-id="c96d0-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookpivottable-refreshall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c96d0-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c96d0-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookpivottable-refreshall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c96d0-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c96d0-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookpivottable-refreshall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c96d0-139">Java</span><span class="sxs-lookup"><span data-stu-id="c96d0-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookpivottable-refreshall-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c96d0-140">响应</span><span class="sxs-lookup"><span data-stu-id="c96d0-140">Response</span></span>
<span data-ttu-id="c96d0-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c96d0-141">Here is an example of the response.</span></span>
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

