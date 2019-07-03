---
title: 'TableSort: apply'
description: 执行排序操作。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 5f825ac6aa54c90064fbbb058383b83c132e4ded
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35456048"
---
# <a name="tablesort-apply"></a><span data-ttu-id="252c9-103">TableSort: apply</span><span class="sxs-lookup"><span data-stu-id="252c9-103">TableSort: apply</span></span>

<span data-ttu-id="252c9-104">执行排序操作。</span><span class="sxs-lookup"><span data-stu-id="252c9-104">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="252c9-105">权限</span><span class="sxs-lookup"><span data-stu-id="252c9-105">Permissions</span></span>
<span data-ttu-id="252c9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="252c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="252c9-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="252c9-108">Permission type</span></span>      | <span data-ttu-id="252c9-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="252c9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="252c9-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="252c9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="252c9-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="252c9-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="252c9-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="252c9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="252c9-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="252c9-113">Not supported.</span></span>    |
|<span data-ttu-id="252c9-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="252c9-114">Application</span></span> | <span data-ttu-id="252c9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="252c9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="252c9-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="252c9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="252c9-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="252c9-117">Request headers</span></span>
| <span data-ttu-id="252c9-118">名称</span><span class="sxs-lookup"><span data-stu-id="252c9-118">Name</span></span>       | <span data-ttu-id="252c9-119">说明</span><span class="sxs-lookup"><span data-stu-id="252c9-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="252c9-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="252c9-120">Authorization</span></span>  | <span data-ttu-id="252c9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="252c9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="252c9-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="252c9-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="252c9-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="252c9-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="252c9-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="252c9-126">Request body</span></span>
<span data-ttu-id="252c9-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="252c9-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="252c9-128">参数</span><span class="sxs-lookup"><span data-stu-id="252c9-128">Parameter</span></span>    | <span data-ttu-id="252c9-129">类型</span><span class="sxs-lookup"><span data-stu-id="252c9-129">Type</span></span>   |<span data-ttu-id="252c9-130">说明</span><span class="sxs-lookup"><span data-stu-id="252c9-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="252c9-131">域</span><span class="sxs-lookup"><span data-stu-id="252c9-131">fields</span></span>|<span data-ttu-id="252c9-132">WorkbookSortField 集合</span><span class="sxs-lookup"><span data-stu-id="252c9-132">WorkbookSortField collection</span></span>|<span data-ttu-id="252c9-133">要用作排序依据的条件列表。</span><span class="sxs-lookup"><span data-stu-id="252c9-133">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="252c9-134">matchCase</span><span class="sxs-lookup"><span data-stu-id="252c9-134">matchCase</span></span>|<span data-ttu-id="252c9-135">布尔</span><span class="sxs-lookup"><span data-stu-id="252c9-135">boolean</span></span>|<span data-ttu-id="252c9-p104">可选。是否让大小写对字符串排序产生影响。</span><span class="sxs-lookup"><span data-stu-id="252c9-p104">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="252c9-138">方法</span><span class="sxs-lookup"><span data-stu-id="252c9-138">method</span></span>|<span data-ttu-id="252c9-139">字符串</span><span class="sxs-lookup"><span data-stu-id="252c9-139">string</span></span>|<span data-ttu-id="252c9-140">可选。</span><span class="sxs-lookup"><span data-stu-id="252c9-140">Optional.</span></span> <span data-ttu-id="252c9-141">用于中文字符的排序方法。</span><span class="sxs-lookup"><span data-stu-id="252c9-141">The ordering method used for Chinese characters.</span></span>  <span data-ttu-id="252c9-142">可能的值为: `PinYin`、 `StrokeCount`。</span><span class="sxs-lookup"><span data-stu-id="252c9-142">The possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="252c9-143">响应</span><span class="sxs-lookup"><span data-stu-id="252c9-143">Response</span></span>

<span data-ttu-id="252c9-p106">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="252c9-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="252c9-146">示例</span><span class="sxs-lookup"><span data-stu-id="252c9-146">Example</span></span>
<span data-ttu-id="252c9-147">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="252c9-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="252c9-148">请求</span><span class="sxs-lookup"><span data-stu-id="252c9-148">Request</span></span>
<span data-ttu-id="252c9-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="252c9-149">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="252c9-150">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="252c9-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tablesort_apply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/apply
Content-type: application/json
Content-length: 298

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
  "method": "method-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="252c9-151">C#</span><span class="sxs-lookup"><span data-stu-id="252c9-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablesort-apply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="252c9-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="252c9-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablesort-apply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="252c9-153">目标-C</span><span class="sxs-lookup"><span data-stu-id="252c9-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablesort-apply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="252c9-154">响应</span><span class="sxs-lookup"><span data-stu-id="252c9-154">Response</span></span>
<span data-ttu-id="252c9-155">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="252c9-155">Here is an example of the response.</span></span> 
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
  "description": "TableSort: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
