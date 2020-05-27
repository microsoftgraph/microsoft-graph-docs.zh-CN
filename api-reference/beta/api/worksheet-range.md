---
title: Worksheet:Range
description: 获取地址或名称指定的 range 对象。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: a7ae6fe3f01eb5105791770451fba1bf1525290e
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2020
ms.locfileid: "44383810"
---
# <a name="worksheet-range"></a><span data-ttu-id="0e9a2-103">Worksheet:Range</span><span class="sxs-lookup"><span data-stu-id="0e9a2-103">Worksheet: Range</span></span>

<span data-ttu-id="0e9a2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e9a2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e9a2-105">获取地址或名称指定的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="0e9a2-105">Gets the range object specified by the address or name.</span></span>
## <a name="permissions"></a><span data-ttu-id="0e9a2-106">权限</span><span class="sxs-lookup"><span data-stu-id="0e9a2-106">Permissions</span></span>
<span data-ttu-id="0e9a2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0e9a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e9a2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0e9a2-109">Permission type</span></span>      | <span data-ttu-id="0e9a2-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0e9a2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0e9a2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0e9a2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0e9a2-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0e9a2-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0e9a2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0e9a2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e9a2-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0e9a2-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0e9a2-115">Application</span><span class="sxs-lookup"><span data-stu-id="0e9a2-115">Application</span></span> | <span data-ttu-id="0e9a2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0e9a2-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0e9a2-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0e9a2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/Range

```
## <a name="request-headers"></a><span data-ttu-id="0e9a2-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="0e9a2-118">Request headers</span></span>
| <span data-ttu-id="0e9a2-119">名称</span><span class="sxs-lookup"><span data-stu-id="0e9a2-119">Name</span></span>       | <span data-ttu-id="0e9a2-120">说明</span><span class="sxs-lookup"><span data-stu-id="0e9a2-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0e9a2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e9a2-121">Authorization</span></span>  | <span data-ttu-id="0e9a2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0e9a2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0e9a2-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0e9a2-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="0e9a2-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="0e9a2-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e9a2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0e9a2-127">Request body</span></span>
<span data-ttu-id="0e9a2-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="0e9a2-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0e9a2-129">参数</span><span class="sxs-lookup"><span data-stu-id="0e9a2-129">Parameter</span></span>    | <span data-ttu-id="0e9a2-130">类型</span><span class="sxs-lookup"><span data-stu-id="0e9a2-130">Type</span></span>   |<span data-ttu-id="0e9a2-131">Description</span><span class="sxs-lookup"><span data-stu-id="0e9a2-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0e9a2-132">address</span><span class="sxs-lookup"><span data-stu-id="0e9a2-132">address</span></span>|<span data-ttu-id="0e9a2-133">string</span><span class="sxs-lookup"><span data-stu-id="0e9a2-133">string</span></span>|<span data-ttu-id="0e9a2-p104">可选。区域的地址或名称。如果未指定，则返回整个工作表区域。</span><span class="sxs-lookup"><span data-stu-id="0e9a2-p104">Optional. The address or the name of the range. If not specified, the entire worksheet range is returned.</span></span>|

## <a name="response"></a><span data-ttu-id="0e9a2-137">响应</span><span class="sxs-lookup"><span data-stu-id="0e9a2-137">Response</span></span>

<span data-ttu-id="0e9a2-138">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [workbookRange](../resources/workbookrange.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0e9a2-138">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e9a2-139">示例</span><span class="sxs-lookup"><span data-stu-id="0e9a2-139">Example</span></span>
<span data-ttu-id="0e9a2-140">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="0e9a2-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0e9a2-141">请求</span><span class="sxs-lookup"><span data-stu-id="0e9a2-141">Request</span></span>
<span data-ttu-id="0e9a2-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0e9a2-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0e9a2-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="0e9a2-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "worksheet_range"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/Range
Content-type: application/json
Content-length: 32

{
  "address": "address-value"
}
```
# <a name="c"></a>[<span data-ttu-id="0e9a2-144">C#</span><span class="sxs-lookup"><span data-stu-id="0e9a2-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheet-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0e9a2-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0e9a2-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheet-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0e9a2-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0e9a2-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheet-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0e9a2-147">响应</span><span class="sxs-lookup"><span data-stu-id="0e9a2-147">Response</span></span>
<span data-ttu-id="0e9a2-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0e9a2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
