---
title: 'TableSort: clear'
description: 清除表上的当前排序。尽管这不能修改表的排序，但它会清除标题按钮的状态。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: f6ee185d8d2375409b7e11a9dbfef7e5d8944087
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271790"
---
# <a name="tablesort-clear"></a><span data-ttu-id="eb564-104">TableSort: clear</span><span class="sxs-lookup"><span data-stu-id="eb564-104">TableSort: clear</span></span>

<span data-ttu-id="eb564-p102">清除表上的当前排序。尽管这不能修改表的排序，但它会清除标题按钮的状态。</span><span class="sxs-lookup"><span data-stu-id="eb564-p102">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>
## <a name="permissions"></a><span data-ttu-id="eb564-107">权限</span><span class="sxs-lookup"><span data-stu-id="eb564-107">Permissions</span></span>
<span data-ttu-id="eb564-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eb564-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb564-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="eb564-110">Permission type</span></span>      | <span data-ttu-id="eb564-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="eb564-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb564-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eb564-112">Delegated (work or school account)</span></span> | <span data-ttu-id="eb564-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eb564-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="eb564-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eb564-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb564-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="eb564-115">Not supported.</span></span>    |
|<span data-ttu-id="eb564-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="eb564-116">Application</span></span> | <span data-ttu-id="eb564-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="eb564-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb564-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eb564-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/clear

```
## <a name="request-headers"></a><span data-ttu-id="eb564-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="eb564-119">Request headers</span></span>
| <span data-ttu-id="eb564-120">名称</span><span class="sxs-lookup"><span data-stu-id="eb564-120">Name</span></span>       | <span data-ttu-id="eb564-121">说明</span><span class="sxs-lookup"><span data-stu-id="eb564-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="eb564-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb564-122">Authorization</span></span>  | <span data-ttu-id="eb564-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="eb564-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="eb564-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="eb564-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="eb564-p105">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="eb564-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb564-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="eb564-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="eb564-129">响应</span><span class="sxs-lookup"><span data-stu-id="eb564-129">Response</span></span>

<span data-ttu-id="eb564-p106">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="eb564-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb564-132">示例</span><span class="sxs-lookup"><span data-stu-id="eb564-132">Example</span></span>
<span data-ttu-id="eb564-133">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="eb564-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="eb564-134">请求</span><span class="sxs-lookup"><span data-stu-id="eb564-134">Request</span></span>
<span data-ttu-id="eb564-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="eb564-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablesort_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/clear
```

##### <a name="response"></a><span data-ttu-id="eb564-136">响应</span><span class="sxs-lookup"><span data-stu-id="eb564-136">Response</span></span>
<span data-ttu-id="eb564-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="eb564-137">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="eb564-138">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="eb564-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="eb564-139">C#</span><span class="sxs-lookup"><span data-stu-id="eb564-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/tablesort_clear-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="eb564-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="eb564-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/tablesort_clear-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="eb564-141">目标-C</span><span class="sxs-lookup"><span data-stu-id="eb564-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/tablesort_clear-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableSort: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/tablesort-clear.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/tablesort-clear.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/tablesort-clear.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
