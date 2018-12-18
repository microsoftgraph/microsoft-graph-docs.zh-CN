---
title: 'RangeSort: apply'
description: 执行排序操作。
author: lumine2008
ms.openlocfilehash: df083fb9f81e529d3f70363eaedec6e4286fc835
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330217"
---
# <a name="rangesort-apply"></a><span data-ttu-id="d0573-103">RangeSort: apply</span><span class="sxs-lookup"><span data-stu-id="d0573-103">RangeSort: apply</span></span>

> <span data-ttu-id="d0573-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d0573-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d0573-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d0573-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d0573-106">执行排序操作。</span><span class="sxs-lookup"><span data-stu-id="d0573-106">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="d0573-107">权限</span><span class="sxs-lookup"><span data-stu-id="d0573-107">Permissions</span></span>
<span data-ttu-id="d0573-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d0573-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0573-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d0573-110">Permission type</span></span>      | <span data-ttu-id="d0573-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d0573-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0573-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d0573-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d0573-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d0573-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d0573-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d0573-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0573-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d0573-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d0573-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d0573-116">Application</span></span> | <span data-ttu-id="d0573-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d0573-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d0573-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d0573-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/sort/apply
POST /workbook/worksheets/{id|name}/range(address='<address>')/sort/apply
POST /workbook/tables/{id|name}/columns/{id|name}/range/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="d0573-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d0573-119">Request headers</span></span>
| <span data-ttu-id="d0573-120">Name</span><span class="sxs-lookup"><span data-stu-id="d0573-120">Name</span></span>       | <span data-ttu-id="d0573-121">说明</span><span class="sxs-lookup"><span data-stu-id="d0573-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d0573-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0573-122">Authorization</span></span>  | <span data-ttu-id="d0573-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d0573-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d0573-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d0573-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="d0573-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="d0573-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0573-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="d0573-128">Request body</span></span>
<span data-ttu-id="d0573-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="d0573-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d0573-130">参数</span><span class="sxs-lookup"><span data-stu-id="d0573-130">Parameter</span></span>    | <span data-ttu-id="d0573-131">Type</span><span class="sxs-lookup"><span data-stu-id="d0573-131">Type</span></span>   |<span data-ttu-id="d0573-132">说明</span><span class="sxs-lookup"><span data-stu-id="d0573-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d0573-133">fields</span><span class="sxs-lookup"><span data-stu-id="d0573-133">fields</span></span>|<span data-ttu-id="d0573-134">SortField</span><span class="sxs-lookup"><span data-stu-id="d0573-134">SortField</span></span>|<span data-ttu-id="d0573-135">作为排序依据的条件列表。</span><span class="sxs-lookup"><span data-stu-id="d0573-135">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="d0573-136">matchCase</span><span class="sxs-lookup"><span data-stu-id="d0573-136">matchCase</span></span>|<span data-ttu-id="d0573-137">boolean</span><span class="sxs-lookup"><span data-stu-id="d0573-137">boolean</span></span>|<span data-ttu-id="d0573-p105">可选。是否让大小写对字符串排序产生影响。</span><span class="sxs-lookup"><span data-stu-id="d0573-p105">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="d0573-140">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="d0573-140">hasHeaders</span></span>|<span data-ttu-id="d0573-141">boolean</span><span class="sxs-lookup"><span data-stu-id="d0573-141">boolean</span></span>|<span data-ttu-id="d0573-p106">可选。该区域是否有标头。</span><span class="sxs-lookup"><span data-stu-id="d0573-p106">Optional. Whether the range has a header.</span></span>|
|<span data-ttu-id="d0573-144">orientation</span><span class="sxs-lookup"><span data-stu-id="d0573-144">orientation</span></span>|<span data-ttu-id="d0573-145">string</span><span class="sxs-lookup"><span data-stu-id="d0573-145">string</span></span>|<span data-ttu-id="d0573-p107">可选。该操作是对行还是列排序。可能的值是：`Rows`、`Columns`。</span><span class="sxs-lookup"><span data-stu-id="d0573-p107">Optional. Whether the operation is sorting rows or columns.  Possible values are: `Rows`, `Columns`.</span></span>|
|<span data-ttu-id="d0573-149">method</span><span class="sxs-lookup"><span data-stu-id="d0573-149">method</span></span>|<span data-ttu-id="d0573-150">string</span><span class="sxs-lookup"><span data-stu-id="d0573-150">string</span></span>|<span data-ttu-id="d0573-p108">可选。用于中文字符的排序方法。可能的值是：`PinYin`、`StrokeCount`。</span><span class="sxs-lookup"><span data-stu-id="d0573-p108">Optional. The ordering method used for Chinese characters.  Possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="d0573-154">响应</span><span class="sxs-lookup"><span data-stu-id="d0573-154">Response</span></span>

<span data-ttu-id="d0573-p109">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="d0573-p109">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0573-157">示例</span><span class="sxs-lookup"><span data-stu-id="d0573-157">Example</span></span>
<span data-ttu-id="d0573-158">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="d0573-158">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d0573-159">请求</span><span class="sxs-lookup"><span data-stu-id="d0573-159">Request</span></span>
<span data-ttu-id="d0573-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d0573-160">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangesort_apply"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/sort/apply
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

##### <a name="response"></a><span data-ttu-id="d0573-161">响应</span><span class="sxs-lookup"><span data-stu-id="d0573-161">Response</span></span>
<span data-ttu-id="d0573-162">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d0573-162">Here is an example of the response.</span></span> 
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
<!-- {
  "type": "#page.annotation",
  "description": "RangeSort: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->