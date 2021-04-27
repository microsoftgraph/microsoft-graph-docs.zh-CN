---
title: Range:UsedRange
description: 返回指定 range 对象的所用范围。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: d705c89ca70616a57209bf788e43c433c6f8ee61
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055048"
---
# <a name="range-usedrange"></a><span data-ttu-id="2da18-103">Range:UsedRange</span><span class="sxs-lookup"><span data-stu-id="2da18-103">Range: UsedRange</span></span>

<span data-ttu-id="2da18-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2da18-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2da18-105">返回指定 range 对象的所用范围。</span><span class="sxs-lookup"><span data-stu-id="2da18-105">Returns the used range of the given range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2da18-106">权限</span><span class="sxs-lookup"><span data-stu-id="2da18-106">Permissions</span></span>
<span data-ttu-id="2da18-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2da18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2da18-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2da18-109">Permission type</span></span>      | <span data-ttu-id="2da18-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2da18-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2da18-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2da18-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2da18-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2da18-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2da18-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2da18-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2da18-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2da18-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2da18-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2da18-115">Application</span></span> | <span data-ttu-id="2da18-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2da18-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2da18-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2da18-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/names/{name}/range/UsedRange
GET /me/drive/root:/{item-path}:/workbook/names/{name}/range/UsedRange
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/UsedRange
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/UsedRange
GET /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/UsedRange
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/UsedRange

```
## <a name="request-headers"></a><span data-ttu-id="2da18-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="2da18-118">Request headers</span></span>
| <span data-ttu-id="2da18-119">名称</span><span class="sxs-lookup"><span data-stu-id="2da18-119">Name</span></span>       | <span data-ttu-id="2da18-120">说明</span><span class="sxs-lookup"><span data-stu-id="2da18-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2da18-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2da18-121">Authorization</span></span>  | <span data-ttu-id="2da18-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2da18-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2da18-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2da18-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="2da18-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="2da18-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2da18-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2da18-127">Request body</span></span>
<span data-ttu-id="2da18-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="2da18-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2da18-129">参数</span><span class="sxs-lookup"><span data-stu-id="2da18-129">Parameter</span></span>    | <span data-ttu-id="2da18-130">类型</span><span class="sxs-lookup"><span data-stu-id="2da18-130">Type</span></span>   |<span data-ttu-id="2da18-131">说明</span><span class="sxs-lookup"><span data-stu-id="2da18-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2da18-132">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="2da18-132">valuesOnly</span></span>|<span data-ttu-id="2da18-133">布尔</span><span class="sxs-lookup"><span data-stu-id="2da18-133">boolean</span></span>|<span data-ttu-id="2da18-p104">可选。仅将有值的单元格视为已使用的单元格。</span><span class="sxs-lookup"><span data-stu-id="2da18-p104">Optional. Considers only cells with values as used cells.</span></span>|

## <a name="response"></a><span data-ttu-id="2da18-136">响应</span><span class="sxs-lookup"><span data-stu-id="2da18-136">Response</span></span>

<span data-ttu-id="2da18-137">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [workbookRange](../resources/workbookrange.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2da18-137">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2da18-138">示例</span><span class="sxs-lookup"><span data-stu-id="2da18-138">Example</span></span>
<span data-ttu-id="2da18-139">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="2da18-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2da18-140">请求</span><span class="sxs-lookup"><span data-stu-id="2da18-140">Request</span></span>
<span data-ttu-id="2da18-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2da18-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2da18-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="2da18-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "range_usedrange"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/UsedRange
Content-type: application/json
Content-length: 24

{
  "valuesOnly": true
}
```
# <a name="c"></a>[<span data-ttu-id="2da18-143">C#</span><span class="sxs-lookup"><span data-stu-id="2da18-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-usedrange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2da18-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2da18-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-usedrange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2da18-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2da18-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-usedrange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2da18-146">Java</span><span class="sxs-lookup"><span data-stu-id="2da18-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-usedrange-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2da18-147">响应</span><span class="sxs-lookup"><span data-stu-id="2da18-147">Response</span></span>
<span data-ttu-id="2da18-148">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="2da18-148">Here is an example of the response.</span></span> <span data-ttu-id="2da18-149">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2da18-149">Note: The response object shown here might be shortened for readability.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Range: UsedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


