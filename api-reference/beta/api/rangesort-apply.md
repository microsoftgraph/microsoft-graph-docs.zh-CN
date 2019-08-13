---
title: 'RangeSort: apply'
description: 执行排序操作。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: be589136a321e2d840c502cddba9906bd948226f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36308750"
---
# <a name="rangesort-apply"></a><span data-ttu-id="19ced-103">RangeSort: apply</span><span class="sxs-lookup"><span data-stu-id="19ced-103">RangeSort: apply</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19ced-104">执行排序操作。</span><span class="sxs-lookup"><span data-stu-id="19ced-104">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="19ced-105">权限</span><span class="sxs-lookup"><span data-stu-id="19ced-105">Permissions</span></span>
<span data-ttu-id="19ced-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="19ced-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19ced-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="19ced-108">Permission type</span></span>      | <span data-ttu-id="19ced-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="19ced-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="19ced-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="19ced-110">Delegated (work or school account)</span></span> | <span data-ttu-id="19ced-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19ced-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="19ced-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="19ced-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19ced-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19ced-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="19ced-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="19ced-114">Application</span></span> | <span data-ttu-id="19ced-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="19ced-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="19ced-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="19ced-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/sort/apply
POST /workbook/worksheets/{id|name}/range(address='<address>')/sort/apply
POST /workbook/tables/{id|name}/columns/{id|name}/range/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="19ced-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="19ced-117">Request headers</span></span>
| <span data-ttu-id="19ced-118">名称</span><span class="sxs-lookup"><span data-stu-id="19ced-118">Name</span></span>       | <span data-ttu-id="19ced-119">说明</span><span class="sxs-lookup"><span data-stu-id="19ced-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="19ced-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="19ced-120">Authorization</span></span>  | <span data-ttu-id="19ced-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="19ced-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="19ced-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="19ced-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="19ced-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="19ced-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="19ced-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="19ced-126">Request body</span></span>
<span data-ttu-id="19ced-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="19ced-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="19ced-128">参数</span><span class="sxs-lookup"><span data-stu-id="19ced-128">Parameter</span></span>    | <span data-ttu-id="19ced-129">类型</span><span class="sxs-lookup"><span data-stu-id="19ced-129">Type</span></span>   |<span data-ttu-id="19ced-130">说明</span><span class="sxs-lookup"><span data-stu-id="19ced-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="19ced-131">域</span><span class="sxs-lookup"><span data-stu-id="19ced-131">fields</span></span>|<span data-ttu-id="19ced-132">workbookSortField 集合</span><span class="sxs-lookup"><span data-stu-id="19ced-132">workbookSortField collection</span></span>|<span data-ttu-id="19ced-133">要用作排序依据的条件列表。</span><span class="sxs-lookup"><span data-stu-id="19ced-133">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="19ced-134">matchCase</span><span class="sxs-lookup"><span data-stu-id="19ced-134">matchCase</span></span>|<span data-ttu-id="19ced-135">boolean</span><span class="sxs-lookup"><span data-stu-id="19ced-135">boolean</span></span>|<span data-ttu-id="19ced-p104">可选。是否让大小写对字符串排序产生影响。</span><span class="sxs-lookup"><span data-stu-id="19ced-p104">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="19ced-138">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="19ced-138">hasHeaders</span></span>|<span data-ttu-id="19ced-139">布尔</span><span class="sxs-lookup"><span data-stu-id="19ced-139">boolean</span></span>|<span data-ttu-id="19ced-p105">可选。该区域是否有标头。</span><span class="sxs-lookup"><span data-stu-id="19ced-p105">Optional. Whether the range has a header.</span></span>|
|<span data-ttu-id="19ced-142">orientation</span><span class="sxs-lookup"><span data-stu-id="19ced-142">orientation</span></span>|<span data-ttu-id="19ced-143">string</span><span class="sxs-lookup"><span data-stu-id="19ced-143">string</span></span>|<span data-ttu-id="19ced-p106">可选。该操作是对行还是列排序。可能的值是：`Rows`、`Columns`。</span><span class="sxs-lookup"><span data-stu-id="19ced-p106">Optional. Whether the operation is sorting rows or columns.  Possible values are: `Rows`, `Columns`.</span></span>|
|<span data-ttu-id="19ced-147">方法</span><span class="sxs-lookup"><span data-stu-id="19ced-147">method</span></span>|<span data-ttu-id="19ced-148">string</span><span class="sxs-lookup"><span data-stu-id="19ced-148">string</span></span>|<span data-ttu-id="19ced-p107">可选。用于中文字符的排序方法。可能的值是：`PinYin`、`StrokeCount`。</span><span class="sxs-lookup"><span data-stu-id="19ced-p107">Optional. The ordering method used for Chinese characters.  Possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="19ced-152">响应</span><span class="sxs-lookup"><span data-stu-id="19ced-152">Response</span></span>

<span data-ttu-id="19ced-p108">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="19ced-p108">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19ced-155">示例</span><span class="sxs-lookup"><span data-stu-id="19ced-155">Example</span></span>
<span data-ttu-id="19ced-156">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="19ced-156">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="19ced-157">请求</span><span class="sxs-lookup"><span data-stu-id="19ced-157">Request</span></span>
<span data-ttu-id="19ced-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="19ced-158">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="19ced-159">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="19ced-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "rangesort_apply"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/sort/apply
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="19ced-160">C#</span><span class="sxs-lookup"><span data-stu-id="19ced-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/rangesort-apply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="19ced-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="19ced-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/rangesort-apply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="19ced-162">目标-C</span><span class="sxs-lookup"><span data-stu-id="19ced-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/rangesort-apply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="19ced-163">Java</span><span class="sxs-lookup"><span data-stu-id="19ced-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/rangesort-apply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="19ced-164">响应</span><span class="sxs-lookup"><span data-stu-id="19ced-164">Response</span></span>
<span data-ttu-id="19ced-165">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="19ced-165">Here is an example of the response.</span></span> 
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
  "description": "RangeSort: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
