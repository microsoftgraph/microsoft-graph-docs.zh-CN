---
title: 'workbookApplication: 计算'
description: 重新计算 Excel 中当前打开的所有工作簿。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 653fd377e59570948716c5e663c2802e729e673a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35269816"
---
# <a name="workbookapplication-calculate"></a><span data-ttu-id="1e55e-103">workbookApplication: 计算</span><span class="sxs-lookup"><span data-stu-id="1e55e-103">workbookApplication: calculate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e55e-104">重新计算 Excel 中当前打开的所有工作簿。</span><span class="sxs-lookup"><span data-stu-id="1e55e-104">Recalculate all currently opened workbooks in Excel.</span></span>
## <a name="permissions"></a><span data-ttu-id="1e55e-105">权限</span><span class="sxs-lookup"><span data-stu-id="1e55e-105">Permissions</span></span>
<span data-ttu-id="1e55e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1e55e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e55e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="1e55e-108">Permission type</span></span>      | <span data-ttu-id="1e55e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1e55e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e55e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1e55e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1e55e-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="1e55e-111">Not supported.</span></span>    |
|<span data-ttu-id="1e55e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1e55e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e55e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="1e55e-113">Not supported.</span></span>    |
|<span data-ttu-id="1e55e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="1e55e-114">Application</span></span> | <span data-ttu-id="1e55e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1e55e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1e55e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1e55e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/application/calculate

```
## <a name="request-headers"></a><span data-ttu-id="1e55e-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="1e55e-117">Request headers</span></span>
| <span data-ttu-id="1e55e-118">名称</span><span class="sxs-lookup"><span data-stu-id="1e55e-118">Name</span></span>       | <span data-ttu-id="1e55e-119">说明</span><span class="sxs-lookup"><span data-stu-id="1e55e-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1e55e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e55e-120">Authorization</span></span>  | <span data-ttu-id="1e55e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1e55e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1e55e-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="1e55e-123">Request body</span></span>
<span data-ttu-id="1e55e-124">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="1e55e-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1e55e-125">参数</span><span class="sxs-lookup"><span data-stu-id="1e55e-125">Parameter</span></span>    | <span data-ttu-id="1e55e-126">类型</span><span class="sxs-lookup"><span data-stu-id="1e55e-126">Type</span></span>   |<span data-ttu-id="1e55e-127">说明</span><span class="sxs-lookup"><span data-stu-id="1e55e-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1e55e-128">calculationType</span><span class="sxs-lookup"><span data-stu-id="1e55e-128">calculationType</span></span>|<span data-ttu-id="1e55e-129">string</span><span class="sxs-lookup"><span data-stu-id="1e55e-129">string</span></span>|<span data-ttu-id="1e55e-130">指定要使用的计算类型。</span><span class="sxs-lookup"><span data-stu-id="1e55e-130">Specifies the calculation type to use.</span></span>  <span data-ttu-id="1e55e-131">可取值为：`Recalculate`、`Full`、`FullRebuild`。</span><span class="sxs-lookup"><span data-stu-id="1e55e-131">Possible values are: `Recalculate`, `Full`, `FullRebuild`.</span></span>|

## <a name="response"></a><span data-ttu-id="1e55e-132">响应</span><span class="sxs-lookup"><span data-stu-id="1e55e-132">Response</span></span>

<span data-ttu-id="1e55e-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="1e55e-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e55e-135">示例</span><span class="sxs-lookup"><span data-stu-id="1e55e-135">Example</span></span>
<span data-ttu-id="1e55e-136">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="1e55e-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1e55e-137">请求</span><span class="sxs-lookup"><span data-stu-id="1e55e-137">Request</span></span>
<span data-ttu-id="1e55e-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1e55e-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookApplication_calculate"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/application/calculate
Content-type: application/json
Content-length: 48

{
  "calculationType": "calculationType-value"
}
```

##### <a name="response"></a><span data-ttu-id="1e55e-139">响应</span><span class="sxs-lookup"><span data-stu-id="1e55e-139">Response</span></span>
<span data-ttu-id="1e55e-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1e55e-140">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->

```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="1e55e-141">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="1e55e-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1e55e-142">C#</span><span class="sxs-lookup"><span data-stu-id="1e55e-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/workbookApplication_calculate-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1e55e-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="1e55e-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/workbookApplication_calculate-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="1e55e-144">目标-C</span><span class="sxs-lookup"><span data-stu-id="1e55e-144">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/workbookApplication_calculate-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "workbookApplication: calculate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/workbookapplication-calculate.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/workbookapplication-calculate.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/workbookapplication-calculate.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
