---
title: 'TableSort: apply'
description: 执行排序操作。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 433dd7f62727f87ef5439708aa2b5958cf4b1e5d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509483"
---
# <a name="tablesort-apply"></a><span data-ttu-id="639b8-103">TableSort: apply</span><span class="sxs-lookup"><span data-stu-id="639b8-103">TableSort: apply</span></span>

<span data-ttu-id="639b8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="639b8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="639b8-105">执行排序操作。</span><span class="sxs-lookup"><span data-stu-id="639b8-105">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="639b8-106">权限</span><span class="sxs-lookup"><span data-stu-id="639b8-106">Permissions</span></span>
<span data-ttu-id="639b8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="639b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="639b8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="639b8-109">Permission type</span></span>      | <span data-ttu-id="639b8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="639b8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="639b8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="639b8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="639b8-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="639b8-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="639b8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="639b8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="639b8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="639b8-114">Not supported.</span></span>    |
|<span data-ttu-id="639b8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="639b8-115">Application</span></span> | <span data-ttu-id="639b8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="639b8-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="639b8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="639b8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="639b8-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="639b8-118">Request headers</span></span>
| <span data-ttu-id="639b8-119">名称</span><span class="sxs-lookup"><span data-stu-id="639b8-119">Name</span></span>       | <span data-ttu-id="639b8-120">说明</span><span class="sxs-lookup"><span data-stu-id="639b8-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="639b8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="639b8-121">Authorization</span></span>  | <span data-ttu-id="639b8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="639b8-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="639b8-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="639b8-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="639b8-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="639b8-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="639b8-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="639b8-127">Request body</span></span>
<span data-ttu-id="639b8-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="639b8-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="639b8-129">参数</span><span class="sxs-lookup"><span data-stu-id="639b8-129">Parameter</span></span>    | <span data-ttu-id="639b8-130">类型</span><span class="sxs-lookup"><span data-stu-id="639b8-130">Type</span></span>   |<span data-ttu-id="639b8-131">说明</span><span class="sxs-lookup"><span data-stu-id="639b8-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="639b8-132">域</span><span class="sxs-lookup"><span data-stu-id="639b8-132">fields</span></span>|<span data-ttu-id="639b8-133">WorkbookSortField 集合</span><span class="sxs-lookup"><span data-stu-id="639b8-133">WorkbookSortField collection</span></span>|<span data-ttu-id="639b8-134">要用作排序依据的条件列表。</span><span class="sxs-lookup"><span data-stu-id="639b8-134">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="639b8-135">matchCase</span><span class="sxs-lookup"><span data-stu-id="639b8-135">matchCase</span></span>|<span data-ttu-id="639b8-136">布尔</span><span class="sxs-lookup"><span data-stu-id="639b8-136">boolean</span></span>|<span data-ttu-id="639b8-p104">可选。是否让大小写对字符串排序产生影响。</span><span class="sxs-lookup"><span data-stu-id="639b8-p104">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="639b8-139">方法</span><span class="sxs-lookup"><span data-stu-id="639b8-139">method</span></span>|<span data-ttu-id="639b8-140">字符串</span><span class="sxs-lookup"><span data-stu-id="639b8-140">string</span></span>|<span data-ttu-id="639b8-141">可选。</span><span class="sxs-lookup"><span data-stu-id="639b8-141">Optional.</span></span> <span data-ttu-id="639b8-142">用于中文字符的排序方法。</span><span class="sxs-lookup"><span data-stu-id="639b8-142">The ordering method used for Chinese characters.</span></span>  <span data-ttu-id="639b8-143">可能的值为： `PinYin`、 `StrokeCount`。</span><span class="sxs-lookup"><span data-stu-id="639b8-143">The possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="639b8-144">响应</span><span class="sxs-lookup"><span data-stu-id="639b8-144">Response</span></span>

<span data-ttu-id="639b8-p106">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="639b8-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="639b8-147">示例</span><span class="sxs-lookup"><span data-stu-id="639b8-147">Example</span></span>
<span data-ttu-id="639b8-148">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="639b8-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="639b8-149">请求</span><span class="sxs-lookup"><span data-stu-id="639b8-149">Request</span></span>
<span data-ttu-id="639b8-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="639b8-150">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="639b8-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="639b8-151">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="639b8-152">C#</span><span class="sxs-lookup"><span data-stu-id="639b8-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablesort-apply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="639b8-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="639b8-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablesort-apply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="639b8-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="639b8-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablesort-apply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="639b8-155">Java</span><span class="sxs-lookup"><span data-stu-id="639b8-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tablesort-apply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="639b8-156">响应</span><span class="sxs-lookup"><span data-stu-id="639b8-156">Response</span></span>
<span data-ttu-id="639b8-157">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="639b8-157">Here is an example of the response.</span></span> 
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
