---
title: Worksheet:Range
description: 获取地址或名称指定的 range 对象。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: dc5c893071c72f242d64814f10ec028762e49a58
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048867"
---
# <a name="worksheet-range"></a><span data-ttu-id="19d5c-103">Worksheet:Range</span><span class="sxs-lookup"><span data-stu-id="19d5c-103">Worksheet: Range</span></span>

<span data-ttu-id="19d5c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19d5c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19d5c-105">获取地址或名称指定的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="19d5c-105">Gets the range object specified by the address or name.</span></span>
## <a name="permissions"></a><span data-ttu-id="19d5c-106">权限</span><span class="sxs-lookup"><span data-stu-id="19d5c-106">Permissions</span></span>
<span data-ttu-id="19d5c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="19d5c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19d5c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="19d5c-109">Permission type</span></span>      | <span data-ttu-id="19d5c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="19d5c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="19d5c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="19d5c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="19d5c-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19d5c-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="19d5c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="19d5c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19d5c-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19d5c-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="19d5c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="19d5c-115">Application</span></span> | <span data-ttu-id="19d5c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="19d5c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="19d5c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="19d5c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/Range
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/Range

```
## <a name="request-headers"></a><span data-ttu-id="19d5c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="19d5c-118">Request headers</span></span>
| <span data-ttu-id="19d5c-119">名称</span><span class="sxs-lookup"><span data-stu-id="19d5c-119">Name</span></span>       | <span data-ttu-id="19d5c-120">说明</span><span class="sxs-lookup"><span data-stu-id="19d5c-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="19d5c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="19d5c-121">Authorization</span></span>  | <span data-ttu-id="19d5c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="19d5c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="19d5c-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="19d5c-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="19d5c-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="19d5c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="19d5c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="19d5c-127">Request body</span></span>
<span data-ttu-id="19d5c-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="19d5c-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="19d5c-129">参数</span><span class="sxs-lookup"><span data-stu-id="19d5c-129">Parameter</span></span>    | <span data-ttu-id="19d5c-130">类型</span><span class="sxs-lookup"><span data-stu-id="19d5c-130">Type</span></span>   |<span data-ttu-id="19d5c-131">说明</span><span class="sxs-lookup"><span data-stu-id="19d5c-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="19d5c-132">address</span><span class="sxs-lookup"><span data-stu-id="19d5c-132">address</span></span>|<span data-ttu-id="19d5c-133">string</span><span class="sxs-lookup"><span data-stu-id="19d5c-133">string</span></span>|<span data-ttu-id="19d5c-p104">可选。区域的地址或名称。如果未指定，则返回整个工作表区域。</span><span class="sxs-lookup"><span data-stu-id="19d5c-p104">Optional. The address or the name of the range. If not specified, the entire worksheet range is returned.</span></span>|

## <a name="response"></a><span data-ttu-id="19d5c-137">响应</span><span class="sxs-lookup"><span data-stu-id="19d5c-137">Response</span></span>

<span data-ttu-id="19d5c-138">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [workbookRange](../resources/workbookrange.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="19d5c-138">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19d5c-139">示例</span><span class="sxs-lookup"><span data-stu-id="19d5c-139">Example</span></span>
<span data-ttu-id="19d5c-140">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="19d5c-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="19d5c-141">请求</span><span class="sxs-lookup"><span data-stu-id="19d5c-141">Request</span></span>
<span data-ttu-id="19d5c-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="19d5c-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="19d5c-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="19d5c-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "worksheet_range"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/Range
Content-type: application/json
Content-length: 32

{
  "address": "address-value"
}
```
# <a name="c"></a>[<span data-ttu-id="19d5c-144">C#</span><span class="sxs-lookup"><span data-stu-id="19d5c-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheet-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="19d5c-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="19d5c-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheet-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="19d5c-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="19d5c-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheet-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="19d5c-147">Java</span><span class="sxs-lookup"><span data-stu-id="19d5c-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheet-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="19d5c-148">响应</span><span class="sxs-lookup"><span data-stu-id="19d5c-148">Response</span></span>
<span data-ttu-id="19d5c-149">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="19d5c-149">Here is an example of the response.</span></span> <span data-ttu-id="19d5c-150">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="19d5c-150">Note: The response object shown here might be shortened for readability.</span></span>
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
  "description": "Worksheet: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


