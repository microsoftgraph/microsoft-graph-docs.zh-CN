---
title: Worksheet:Range
description: 获取地址或名称指定的 range 对象。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: ec627bcdf1415fd022a25a4234371d2c5b9c6a6a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35456433"
---
# <a name="worksheet-range"></a><span data-ttu-id="29327-103">Worksheet:Range</span><span class="sxs-lookup"><span data-stu-id="29327-103">Worksheet: Range</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29327-104">获取地址或名称指定的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="29327-104">Gets the range object specified by the address or name.</span></span>
## <a name="permissions"></a><span data-ttu-id="29327-105">权限</span><span class="sxs-lookup"><span data-stu-id="29327-105">Permissions</span></span>
<span data-ttu-id="29327-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="29327-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29327-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="29327-108">Permission type</span></span>      | <span data-ttu-id="29327-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="29327-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="29327-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="29327-110">Delegated (work or school account)</span></span> | <span data-ttu-id="29327-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="29327-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="29327-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="29327-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29327-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="29327-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="29327-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="29327-114">Application</span></span> | <span data-ttu-id="29327-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="29327-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="29327-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="29327-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/Range

```
## <a name="request-headers"></a><span data-ttu-id="29327-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="29327-117">Request headers</span></span>
| <span data-ttu-id="29327-118">名称</span><span class="sxs-lookup"><span data-stu-id="29327-118">Name</span></span>       | <span data-ttu-id="29327-119">说明</span><span class="sxs-lookup"><span data-stu-id="29327-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="29327-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="29327-120">Authorization</span></span>  | <span data-ttu-id="29327-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="29327-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="29327-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="29327-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="29327-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="29327-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="29327-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="29327-126">Request body</span></span>
<span data-ttu-id="29327-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="29327-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="29327-128">参数</span><span class="sxs-lookup"><span data-stu-id="29327-128">Parameter</span></span>    | <span data-ttu-id="29327-129">类型</span><span class="sxs-lookup"><span data-stu-id="29327-129">Type</span></span>   |<span data-ttu-id="29327-130">说明</span><span class="sxs-lookup"><span data-stu-id="29327-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="29327-131">address</span><span class="sxs-lookup"><span data-stu-id="29327-131">address</span></span>|<span data-ttu-id="29327-132">string</span><span class="sxs-lookup"><span data-stu-id="29327-132">string</span></span>|<span data-ttu-id="29327-p104">可选。区域的地址或名称。如果未指定，则返回整个工作表区域。</span><span class="sxs-lookup"><span data-stu-id="29327-p104">Optional. The address or the name of the range. If not specified, the entire worksheet range is returned.</span></span>|

## <a name="response"></a><span data-ttu-id="29327-136">响应</span><span class="sxs-lookup"><span data-stu-id="29327-136">Response</span></span>

<span data-ttu-id="29327-137">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [workbookRange](../resources/workbookrange.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="29327-137">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29327-138">示例</span><span class="sxs-lookup"><span data-stu-id="29327-138">Example</span></span>
<span data-ttu-id="29327-139">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="29327-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="29327-140">请求</span><span class="sxs-lookup"><span data-stu-id="29327-140">Request</span></span>
<span data-ttu-id="29327-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="29327-141">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="29327-142">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="29327-142">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="29327-143">C#</span><span class="sxs-lookup"><span data-stu-id="29327-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheet-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="29327-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="29327-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheet-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="29327-145">目标-C</span><span class="sxs-lookup"><span data-stu-id="29327-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheet-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="29327-146">响应</span><span class="sxs-lookup"><span data-stu-id="29327-146">Response</span></span>
<span data-ttu-id="29327-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="29327-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
