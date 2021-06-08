---
title: 'workbookPivotTable: refreshAll'
description: 刷新给定工作表中的数据透视表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 0b3077567710db0c4489bb25cf6a509454427379
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786430"
---
# <a name="workbookpivottable-refreshall"></a><span data-ttu-id="989f8-103">workbookPivotTable: refreshAll</span><span class="sxs-lookup"><span data-stu-id="989f8-103">workbookPivotTable: refreshAll</span></span>

<span data-ttu-id="989f8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="989f8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="989f8-105">刷新给定工作表中的数据透视表。</span><span class="sxs-lookup"><span data-stu-id="989f8-105">Refreshes the PivotTable within a given worksheet.</span></span>

## <a name="permissions"></a><span data-ttu-id="989f8-106">权限</span><span class="sxs-lookup"><span data-stu-id="989f8-106">Permissions</span></span>
<span data-ttu-id="989f8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="989f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="989f8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="989f8-109">Permission type</span></span>      | <span data-ttu-id="989f8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="989f8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="989f8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="989f8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="989f8-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="989f8-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="989f8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="989f8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="989f8-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="989f8-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="989f8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="989f8-115">Application</span></span> | <span data-ttu-id="989f8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="989f8-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="989f8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="989f8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/{id}/pivotTables/refreshAll
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id}/pivotTables/refreshAll

```
## <a name="request-headers"></a><span data-ttu-id="989f8-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="989f8-118">Request headers</span></span>
| <span data-ttu-id="989f8-119">名称</span><span class="sxs-lookup"><span data-stu-id="989f8-119">Name</span></span>       | <span data-ttu-id="989f8-120">说明</span><span class="sxs-lookup"><span data-stu-id="989f8-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="989f8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="989f8-121">Authorization</span></span>  | <span data-ttu-id="989f8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="989f8-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="989f8-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="989f8-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="989f8-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="989f8-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="989f8-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="989f8-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="989f8-128">响应</span><span class="sxs-lookup"><span data-stu-id="989f8-128">Response</span></span>

<span data-ttu-id="989f8-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="989f8-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="989f8-131">示例</span><span class="sxs-lookup"><span data-stu-id="989f8-131">Example</span></span>
<span data-ttu-id="989f8-132">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="989f8-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="989f8-133">请求</span><span class="sxs-lookup"><span data-stu-id="989f8-133">Request</span></span>
<span data-ttu-id="989f8-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="989f8-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="989f8-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="989f8-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refreshall"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll
```
# <a name="c"></a>[<span data-ttu-id="989f8-136">C#</span><span class="sxs-lookup"><span data-stu-id="989f8-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookpivottable-refreshall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="989f8-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="989f8-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookpivottable-refreshall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="989f8-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="989f8-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookpivottable-refreshall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="989f8-139">Java</span><span class="sxs-lookup"><span data-stu-id="989f8-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookpivottable-refreshall-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="989f8-140">响应</span><span class="sxs-lookup"><span data-stu-id="989f8-140">Response</span></span>
<span data-ttu-id="989f8-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="989f8-141">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response"
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


