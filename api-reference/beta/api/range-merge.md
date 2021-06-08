---
title: 'Range: merge'
description: 将范围单元格合并到工作表的一个区域中。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 76624d83ace7f72a7b6daf24857fb976511139c7
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52785905"
---
# <a name="range-merge"></a><span data-ttu-id="28b41-103">Range: merge</span><span class="sxs-lookup"><span data-stu-id="28b41-103">Range: merge</span></span>

<span data-ttu-id="28b41-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28b41-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28b41-105">将范围单元格合并到工作表的一个区域中。</span><span class="sxs-lookup"><span data-stu-id="28b41-105">Merge the range cells into one region in the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="28b41-106">权限</span><span class="sxs-lookup"><span data-stu-id="28b41-106">Permissions</span></span>
<span data-ttu-id="28b41-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="28b41-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28b41-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="28b41-109">Permission type</span></span>      | <span data-ttu-id="28b41-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="28b41-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="28b41-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="28b41-111">Delegated (work or school account)</span></span> | <span data-ttu-id="28b41-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="28b41-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="28b41-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="28b41-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28b41-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="28b41-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="28b41-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="28b41-115">Application</span></span> | <span data-ttu-id="28b41-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="28b41-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="28b41-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="28b41-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/names/{name}/range/merge
POST /me/drive/root:/{item-path}:/workbook/names/{name}/range/merge
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/merge
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/merge
POST /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/merge
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/merge

```
## <a name="request-headers"></a><span data-ttu-id="28b41-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="28b41-118">Request headers</span></span>
| <span data-ttu-id="28b41-119">名称</span><span class="sxs-lookup"><span data-stu-id="28b41-119">Name</span></span>       | <span data-ttu-id="28b41-120">说明</span><span class="sxs-lookup"><span data-stu-id="28b41-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="28b41-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="28b41-121">Authorization</span></span>  | <span data-ttu-id="28b41-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="28b41-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="28b41-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="28b41-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="28b41-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="28b41-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="28b41-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="28b41-127">Request body</span></span>
<span data-ttu-id="28b41-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="28b41-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="28b41-129">参数</span><span class="sxs-lookup"><span data-stu-id="28b41-129">Parameter</span></span>    | <span data-ttu-id="28b41-130">类型</span><span class="sxs-lookup"><span data-stu-id="28b41-130">Type</span></span>   |<span data-ttu-id="28b41-131">说明</span><span class="sxs-lookup"><span data-stu-id="28b41-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="28b41-132">横向</span><span class="sxs-lookup"><span data-stu-id="28b41-132">across</span></span>|<span data-ttu-id="28b41-133">布尔</span><span class="sxs-lookup"><span data-stu-id="28b41-133">boolean</span></span>|<span data-ttu-id="28b41-p104">可选。如果为 True，则将指定区域中每一行的单元格合并为一个单独的合并单元格。默认值是 false。</span><span class="sxs-lookup"><span data-stu-id="28b41-p104">Optional. Set true to merge cells in each row of the specified range as separate merged cells. The default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="28b41-137">响应</span><span class="sxs-lookup"><span data-stu-id="28b41-137">Response</span></span>

<span data-ttu-id="28b41-p105">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="28b41-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28b41-140">示例</span><span class="sxs-lookup"><span data-stu-id="28b41-140">Example</span></span>
<span data-ttu-id="28b41-141">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="28b41-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="28b41-142">请求</span><span class="sxs-lookup"><span data-stu-id="28b41-142">Request</span></span>
<span data-ttu-id="28b41-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="28b41-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="28b41-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="28b41-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "range_merge"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/merge
Content-type: application/json
Content-length: 20

{
  "across": true
}
```
# <a name="c"></a>[<span data-ttu-id="28b41-145">C#</span><span class="sxs-lookup"><span data-stu-id="28b41-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-merge-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="28b41-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="28b41-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-merge-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="28b41-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="28b41-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-merge-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="28b41-148">Java</span><span class="sxs-lookup"><span data-stu-id="28b41-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-merge-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="28b41-149">响应</span><span class="sxs-lookup"><span data-stu-id="28b41-149">Response</span></span>
<span data-ttu-id="28b41-150">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="28b41-150">Here is an example of the response.</span></span> 
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
  "description": "Range: merge",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


