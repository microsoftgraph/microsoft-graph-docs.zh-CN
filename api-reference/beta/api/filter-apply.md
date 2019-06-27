---
title: 'Filter: apply'
description: 在给定列中应用给定的筛选条件。
localization_priority: Normal
ms.openlocfilehash: be05c2db39a3b0eff84c62a8efec99cfceb5ff5c
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35259043"
---
# <a name="filter-apply"></a><span data-ttu-id="a8dbf-103">Filter: apply</span><span class="sxs-lookup"><span data-stu-id="a8dbf-103">Filter: apply</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8dbf-104">在给定列中应用给定的筛选条件。</span><span class="sxs-lookup"><span data-stu-id="a8dbf-104">Apply the given filter criteria on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="a8dbf-105">权限</span><span class="sxs-lookup"><span data-stu-id="a8dbf-105">Permissions</span></span>
<span data-ttu-id="a8dbf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a8dbf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8dbf-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="a8dbf-108">Permission type</span></span>      | <span data-ttu-id="a8dbf-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a8dbf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a8dbf-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a8dbf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a8dbf-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a8dbf-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a8dbf-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a8dbf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8dbf-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a8dbf-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a8dbf-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="a8dbf-114">Application</span></span> | <span data-ttu-id="a8dbf-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a8dbf-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a8dbf-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a8dbf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/apply

```
## <a name="request-headers"></a><span data-ttu-id="a8dbf-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="a8dbf-117">Request headers</span></span>
| <span data-ttu-id="a8dbf-118">名称</span><span class="sxs-lookup"><span data-stu-id="a8dbf-118">Name</span></span>       | <span data-ttu-id="a8dbf-119">说明</span><span class="sxs-lookup"><span data-stu-id="a8dbf-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a8dbf-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8dbf-120">Authorization</span></span>  | <span data-ttu-id="a8dbf-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a8dbf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a8dbf-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="a8dbf-123">Request body</span></span>
<span data-ttu-id="a8dbf-124">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="a8dbf-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a8dbf-125">参数</span><span class="sxs-lookup"><span data-stu-id="a8dbf-125">Parameter</span></span>    | <span data-ttu-id="a8dbf-126">类型</span><span class="sxs-lookup"><span data-stu-id="a8dbf-126">Type</span></span>   |<span data-ttu-id="a8dbf-127">说明</span><span class="sxs-lookup"><span data-stu-id="a8dbf-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a8dbf-128">条件</span><span class="sxs-lookup"><span data-stu-id="a8dbf-128">criteria</span></span>|<span data-ttu-id="a8dbf-129">workbookFilterCriteria</span><span class="sxs-lookup"><span data-stu-id="a8dbf-129">workbookFilterCriteria</span></span>|<span data-ttu-id="a8dbf-130">要应用的条件。</span><span class="sxs-lookup"><span data-stu-id="a8dbf-130">The criteria to apply.</span></span>|

## <a name="response"></a><span data-ttu-id="a8dbf-131">响应</span><span class="sxs-lookup"><span data-stu-id="a8dbf-131">Response</span></span>

<span data-ttu-id="a8dbf-p103">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="a8dbf-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8dbf-134">示例</span><span class="sxs-lookup"><span data-stu-id="a8dbf-134">Example</span></span>
<span data-ttu-id="a8dbf-135">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="a8dbf-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a8dbf-136">请求</span><span class="sxs-lookup"><span data-stu-id="a8dbf-136">Request</span></span>
<span data-ttu-id="a8dbf-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a8dbf-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "filter_apply"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/apply
Content-type: application/json
Content-length: 321

{
  "criteria": {
    "criterion1": "criterion1-value",
    "criterion2": "criterion2-value",
    "color": "color-value",
    "operator": {
    },
    "icon": {
      "set": "set-value",
      "index": 99
    },
    "dynamicCriteria": "dynamicCriteria-value",
    "values": {
    },
    "filterOn": "filterOn-value"
  }
}
```

##### <a name="response"></a><span data-ttu-id="a8dbf-138">响应</span><span class="sxs-lookup"><span data-stu-id="a8dbf-138">Response</span></span>
<span data-ttu-id="a8dbf-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a8dbf-139">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="a8dbf-140">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="a8dbf-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a8dbf-141">C#</span><span class="sxs-lookup"><span data-stu-id="a8dbf-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/filter_apply-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a8dbf-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="a8dbf-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/filter_apply-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a8dbf-143">目标-C</span><span class="sxs-lookup"><span data-stu-id="a8dbf-143">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/filter_apply-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Filter: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/filter-apply.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/filter-apply.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/filter-apply.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
