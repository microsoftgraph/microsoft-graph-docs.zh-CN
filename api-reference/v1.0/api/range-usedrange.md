---
title: Range:UsedRange
description: 返回指定 range 对象的所用范围。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: dc8a8680154db8a165708eb75818285bc565758c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050365"
---
# <a name="range-usedrange"></a><span data-ttu-id="72105-103">Range:UsedRange</span><span class="sxs-lookup"><span data-stu-id="72105-103">Range: UsedRange</span></span>

<span data-ttu-id="72105-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72105-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="72105-105">返回指定 range 对象的所用范围。</span><span class="sxs-lookup"><span data-stu-id="72105-105">Returns the used range of the given range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="72105-106">权限</span><span class="sxs-lookup"><span data-stu-id="72105-106">Permissions</span></span>
<span data-ttu-id="72105-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="72105-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72105-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="72105-109">Permission type</span></span>      | <span data-ttu-id="72105-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="72105-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="72105-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="72105-111">Delegated (work or school account)</span></span> | <span data-ttu-id="72105-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="72105-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="72105-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="72105-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72105-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="72105-114">Not supported.</span></span>    |
|<span data-ttu-id="72105-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="72105-115">Application</span></span> | <span data-ttu-id="72105-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="72105-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="72105-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="72105-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/names/{name}/range/usedRange
GET /me/drive/root:/{item-path}:/workbook/names/{name}/range/usedRange
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/usedRange
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/usedRange
GET /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/usedRange
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/usedRange

```
## <a name="request-headers"></a><span data-ttu-id="72105-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="72105-118">Request headers</span></span>
| <span data-ttu-id="72105-119">名称</span><span class="sxs-lookup"><span data-stu-id="72105-119">Name</span></span>       | <span data-ttu-id="72105-120">说明</span><span class="sxs-lookup"><span data-stu-id="72105-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="72105-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="72105-121">Authorization</span></span>  | <span data-ttu-id="72105-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="72105-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="72105-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="72105-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="72105-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="72105-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="72105-127">路径参数</span><span class="sxs-lookup"><span data-stu-id="72105-127">Path parameters</span></span>
| <span data-ttu-id="72105-128">参数</span><span class="sxs-lookup"><span data-stu-id="72105-128">Parameter</span></span>    | <span data-ttu-id="72105-129">类型</span><span class="sxs-lookup"><span data-stu-id="72105-129">Type</span></span>   |<span data-ttu-id="72105-130">说明</span><span class="sxs-lookup"><span data-stu-id="72105-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="72105-131">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="72105-131">valuesOnly</span></span>|<span data-ttu-id="72105-132">布尔</span><span class="sxs-lookup"><span data-stu-id="72105-132">boolean</span></span>|<span data-ttu-id="72105-p104">可选。仅将有值的单元格视为已使用的单元格。</span><span class="sxs-lookup"><span data-stu-id="72105-p104">Optional. Considers only cells with values as used cells.</span></span>|

## <a name="response"></a><span data-ttu-id="72105-135">响应</span><span class="sxs-lookup"><span data-stu-id="72105-135">Response</span></span>

<span data-ttu-id="72105-136">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="72105-136">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72105-137">示例</span><span class="sxs-lookup"><span data-stu-id="72105-137">Example</span></span>
<span data-ttu-id="72105-138">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="72105-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="72105-139">请求</span><span class="sxs-lookup"><span data-stu-id="72105-139">Request</span></span>
<span data-ttu-id="72105-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="72105-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="72105-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="72105-141">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_usedrange"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/usedRange
```
# <a name="c"></a>[<span data-ttu-id="72105-142">C#</span><span class="sxs-lookup"><span data-stu-id="72105-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-usedrange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="72105-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="72105-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-usedrange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="72105-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="72105-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-usedrange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="72105-145">Java</span><span class="sxs-lookup"><span data-stu-id="72105-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-usedrange-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="72105-146">响应</span><span class="sxs-lookup"><span data-stu-id="72105-146">Response</span></span>
<span data-ttu-id="72105-147">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="72105-147">Here is an example of the response.</span></span> <span data-ttu-id="72105-148">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="72105-148">Note: The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<span data-ttu-id="72105-149">下面是指定可选参数 `valuesOnly` 的示例。</span><span class="sxs-lookup"><span data-stu-id="72105-149">Here is an example specifying the optional `valuesOnly` parameter.</span></span>

##### <a name="request"></a><span data-ttu-id="72105-150">请求</span><span class="sxs-lookup"><span data-stu-id="72105-150">Request</span></span>
<span data-ttu-id="72105-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="72105-151">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="72105-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="72105-152">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_usedrange_valuesonly"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/usedRange(valuesOnly=true)
```
# <a name="c"></a>[<span data-ttu-id="72105-153">C#</span><span class="sxs-lookup"><span data-stu-id="72105-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-usedrange-valuesonly-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="72105-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="72105-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-usedrange-valuesonly-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="72105-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="72105-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-usedrange-valuesonly-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="72105-156">Java</span><span class="sxs-lookup"><span data-stu-id="72105-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-usedrange-valuesonly-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="72105-157">响应</span><span class="sxs-lookup"><span data-stu-id="72105-157">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 90,
  "columnCount": 90,
  "columnIndex": 90,
  "valueTypes": "valueTypes-value"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: UsedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

