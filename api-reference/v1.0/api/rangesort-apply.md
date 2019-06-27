---
title: 'RangeSort: apply'
description: 执行排序操作。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 6bd71fd26d7a81e09ca73a5393c6532ff3d5c842
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35275437"
---
# <a name="rangesort-apply"></a><span data-ttu-id="7050b-103">RangeSort: apply</span><span class="sxs-lookup"><span data-stu-id="7050b-103">RangeSort: apply</span></span>

<span data-ttu-id="7050b-104">执行排序操作。</span><span class="sxs-lookup"><span data-stu-id="7050b-104">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="7050b-105">权限</span><span class="sxs-lookup"><span data-stu-id="7050b-105">Permissions</span></span>
<span data-ttu-id="7050b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7050b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7050b-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="7050b-108">Permission type</span></span>      | <span data-ttu-id="7050b-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7050b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7050b-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7050b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7050b-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7050b-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7050b-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7050b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7050b-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="7050b-113">Not supported.</span></span>    |
|<span data-ttu-id="7050b-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="7050b-114">Application</span></span> | <span data-ttu-id="7050b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7050b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7050b-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7050b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/sort/apply
POST /workbook/worksheets/{id|name}/range(address='<address>')/sort/apply
POST /workbook/tables/{id|name}/columns/{id|name}/range/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="7050b-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="7050b-117">Request headers</span></span>
| <span data-ttu-id="7050b-118">名称</span><span class="sxs-lookup"><span data-stu-id="7050b-118">Name</span></span>       | <span data-ttu-id="7050b-119">说明</span><span class="sxs-lookup"><span data-stu-id="7050b-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7050b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7050b-120">Authorization</span></span>  | <span data-ttu-id="7050b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7050b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7050b-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7050b-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="7050b-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="7050b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7050b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="7050b-126">Request body</span></span>
<span data-ttu-id="7050b-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="7050b-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7050b-128">参数</span><span class="sxs-lookup"><span data-stu-id="7050b-128">Parameter</span></span>    | <span data-ttu-id="7050b-129">类型</span><span class="sxs-lookup"><span data-stu-id="7050b-129">Type</span></span>   |<span data-ttu-id="7050b-130">说明</span><span class="sxs-lookup"><span data-stu-id="7050b-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7050b-131">域</span><span class="sxs-lookup"><span data-stu-id="7050b-131">fields</span></span>|<span data-ttu-id="7050b-132">WorkbookSortField 集合</span><span class="sxs-lookup"><span data-stu-id="7050b-132">WorkbookSortField collection</span></span>|<span data-ttu-id="7050b-133">要用作排序依据的条件列表。</span><span class="sxs-lookup"><span data-stu-id="7050b-133">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="7050b-134">matchCase</span><span class="sxs-lookup"><span data-stu-id="7050b-134">matchCase</span></span>|<span data-ttu-id="7050b-135">boolean</span><span class="sxs-lookup"><span data-stu-id="7050b-135">boolean</span></span>|<span data-ttu-id="7050b-p104">可选。是否让大小写对字符串排序产生影响。</span><span class="sxs-lookup"><span data-stu-id="7050b-p104">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="7050b-138">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="7050b-138">hasHeaders</span></span>|<span data-ttu-id="7050b-139">布尔</span><span class="sxs-lookup"><span data-stu-id="7050b-139">boolean</span></span>|<span data-ttu-id="7050b-p105">可选。该区域是否有标头。</span><span class="sxs-lookup"><span data-stu-id="7050b-p105">Optional. Whether the range has a header.</span></span>|
|<span data-ttu-id="7050b-142">orientation</span><span class="sxs-lookup"><span data-stu-id="7050b-142">orientation</span></span>|<span data-ttu-id="7050b-143">字符串</span><span class="sxs-lookup"><span data-stu-id="7050b-143">string</span></span>|<span data-ttu-id="7050b-144">可选。</span><span class="sxs-lookup"><span data-stu-id="7050b-144">Optional.</span></span> <span data-ttu-id="7050b-145">该操作是对行还是列排序。</span><span class="sxs-lookup"><span data-stu-id="7050b-145">Whether the operation is sorting rows or columns.</span></span>  <span data-ttu-id="7050b-146">可能的值为: `Rows`、 `Columns`。</span><span class="sxs-lookup"><span data-stu-id="7050b-146">The possible values are: `Rows`, `Columns`.</span></span>|
|<span data-ttu-id="7050b-147">方法</span><span class="sxs-lookup"><span data-stu-id="7050b-147">method</span></span>|<span data-ttu-id="7050b-148">字符串</span><span class="sxs-lookup"><span data-stu-id="7050b-148">string</span></span>|<span data-ttu-id="7050b-149">可选。</span><span class="sxs-lookup"><span data-stu-id="7050b-149">Optional.</span></span> <span data-ttu-id="7050b-150">用于中文字符的排序方法。</span><span class="sxs-lookup"><span data-stu-id="7050b-150">The ordering method used for Chinese characters.</span></span>  <span data-ttu-id="7050b-151">可能的值为: `PinYin`、 `StrokeCount`。</span><span class="sxs-lookup"><span data-stu-id="7050b-151">The possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="7050b-152">响应</span><span class="sxs-lookup"><span data-stu-id="7050b-152">Response</span></span>

<span data-ttu-id="7050b-p108">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="7050b-p108">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7050b-155">示例</span><span class="sxs-lookup"><span data-stu-id="7050b-155">Example</span></span>
<span data-ttu-id="7050b-156">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="7050b-156">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7050b-157">请求</span><span class="sxs-lookup"><span data-stu-id="7050b-157">Request</span></span>
<span data-ttu-id="7050b-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7050b-158">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangesort_apply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/sort/apply
Content-type: application/json
Content-length: 358

{
  "fields": [
    {
      "key": 99,
      "sortOn": "sortOn-value",
      "ascending": true,
      "color": "color-value",
      "dataOption": "dataOption-value",
      "icon": {
        "set": "set-value",
        "index": 99
      }
    }
  ],
  "matchCase": true,
  "hasHeaders": true,
  "orientation": "orientation-value",
  "method": "method-value"
}
```

##### <a name="response"></a><span data-ttu-id="7050b-159">响应</span><span class="sxs-lookup"><span data-stu-id="7050b-159">Response</span></span>
<span data-ttu-id="7050b-160">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7050b-160">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="7050b-161">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="7050b-161">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7050b-162">C#</span><span class="sxs-lookup"><span data-stu-id="7050b-162">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/rangesort_apply-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7050b-163">Javascript</span><span class="sxs-lookup"><span data-stu-id="7050b-163">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/rangesort_apply-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="7050b-164">目标-C</span><span class="sxs-lookup"><span data-stu-id="7050b-164">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/rangesort_apply-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeSort: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/rangesort-apply.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/rangesort-apply.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/rangesort-apply.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
