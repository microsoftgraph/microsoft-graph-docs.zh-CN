---
title: 'RangeSort: apply'
description: 执行排序操作。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 47e2076bb3c556cd277cb5a022ffcbba88ec2f6f
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52788029"
---
# <a name="rangesort-apply"></a><span data-ttu-id="cfa5f-103">RangeSort: apply</span><span class="sxs-lookup"><span data-stu-id="cfa5f-103">RangeSort: apply</span></span>

<span data-ttu-id="cfa5f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cfa5f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cfa5f-105">执行排序操作。</span><span class="sxs-lookup"><span data-stu-id="cfa5f-105">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="cfa5f-106">权限</span><span class="sxs-lookup"><span data-stu-id="cfa5f-106">Permissions</span></span>
<span data-ttu-id="cfa5f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cfa5f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cfa5f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cfa5f-109">Permission type</span></span>      | <span data-ttu-id="cfa5f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cfa5f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cfa5f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cfa5f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cfa5f-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cfa5f-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cfa5f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cfa5f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cfa5f-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cfa5f-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cfa5f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="cfa5f-115">Application</span></span> | <span data-ttu-id="cfa5f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cfa5f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cfa5f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cfa5f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/names/{name}/range/sort/apply
POST /me/drive/root:/{item-path}:/workbook/names/{name}/range/sort/apply
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/sort/apply
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/sort/apply
POST /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/sort/apply
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="cfa5f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="cfa5f-118">Request headers</span></span>
| <span data-ttu-id="cfa5f-119">名称</span><span class="sxs-lookup"><span data-stu-id="cfa5f-119">Name</span></span>       | <span data-ttu-id="cfa5f-120">说明</span><span class="sxs-lookup"><span data-stu-id="cfa5f-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cfa5f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cfa5f-121">Authorization</span></span>  | <span data-ttu-id="cfa5f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cfa5f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cfa5f-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="cfa5f-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="cfa5f-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="cfa5f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cfa5f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="cfa5f-127">Request body</span></span>
<span data-ttu-id="cfa5f-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="cfa5f-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cfa5f-129">参数</span><span class="sxs-lookup"><span data-stu-id="cfa5f-129">Parameter</span></span>    | <span data-ttu-id="cfa5f-130">类型</span><span class="sxs-lookup"><span data-stu-id="cfa5f-130">Type</span></span>   |<span data-ttu-id="cfa5f-131">说明</span><span class="sxs-lookup"><span data-stu-id="cfa5f-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cfa5f-132">域</span><span class="sxs-lookup"><span data-stu-id="cfa5f-132">fields</span></span>|<span data-ttu-id="cfa5f-133">workbookSortField 集合</span><span class="sxs-lookup"><span data-stu-id="cfa5f-133">workbookSortField collection</span></span>|<span data-ttu-id="cfa5f-134">要用作排序依据的条件列表。</span><span class="sxs-lookup"><span data-stu-id="cfa5f-134">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="cfa5f-135">matchCase</span><span class="sxs-lookup"><span data-stu-id="cfa5f-135">matchCase</span></span>|<span data-ttu-id="cfa5f-136">布尔</span><span class="sxs-lookup"><span data-stu-id="cfa5f-136">boolean</span></span>|<span data-ttu-id="cfa5f-p104">可选。是否让大小写对字符串排序产生影响。</span><span class="sxs-lookup"><span data-stu-id="cfa5f-p104">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="cfa5f-139">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="cfa5f-139">hasHeaders</span></span>|<span data-ttu-id="cfa5f-140">布尔</span><span class="sxs-lookup"><span data-stu-id="cfa5f-140">boolean</span></span>|<span data-ttu-id="cfa5f-p105">可选。该区域是否有标头。</span><span class="sxs-lookup"><span data-stu-id="cfa5f-p105">Optional. Whether the range has a header.</span></span>|
|<span data-ttu-id="cfa5f-143">orientation</span><span class="sxs-lookup"><span data-stu-id="cfa5f-143">orientation</span></span>|<span data-ttu-id="cfa5f-144">string</span><span class="sxs-lookup"><span data-stu-id="cfa5f-144">string</span></span>|<span data-ttu-id="cfa5f-p106">可选。该操作是对行还是列排序。可能的值是：`Rows`、`Columns`。</span><span class="sxs-lookup"><span data-stu-id="cfa5f-p106">Optional. Whether the operation is sorting rows or columns.  Possible values are: `Rows`, `Columns`.</span></span>|
|<span data-ttu-id="cfa5f-148">方法</span><span class="sxs-lookup"><span data-stu-id="cfa5f-148">method</span></span>|<span data-ttu-id="cfa5f-149">string</span><span class="sxs-lookup"><span data-stu-id="cfa5f-149">string</span></span>|<span data-ttu-id="cfa5f-p107">可选。用于中文字符的排序方法。可能的值是：`PinYin`、`StrokeCount`。</span><span class="sxs-lookup"><span data-stu-id="cfa5f-p107">Optional. The ordering method used for Chinese characters.  Possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="cfa5f-153">响应</span><span class="sxs-lookup"><span data-stu-id="cfa5f-153">Response</span></span>

<span data-ttu-id="cfa5f-p108">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="cfa5f-p108">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cfa5f-156">示例</span><span class="sxs-lookup"><span data-stu-id="cfa5f-156">Example</span></span>
<span data-ttu-id="cfa5f-157">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="cfa5f-157">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="cfa5f-158">请求</span><span class="sxs-lookup"><span data-stu-id="cfa5f-158">Request</span></span>
<span data-ttu-id="cfa5f-159">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cfa5f-159">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cfa5f-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="cfa5f-160">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="cfa5f-161">C#</span><span class="sxs-lookup"><span data-stu-id="cfa5f-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/rangesort-apply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cfa5f-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cfa5f-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/rangesort-apply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cfa5f-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cfa5f-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/rangesort-apply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cfa5f-164">Java</span><span class="sxs-lookup"><span data-stu-id="cfa5f-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/rangesort-apply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="cfa5f-165">响应</span><span class="sxs-lookup"><span data-stu-id="cfa5f-165">Response</span></span>
<span data-ttu-id="cfa5f-166">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="cfa5f-166">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
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


