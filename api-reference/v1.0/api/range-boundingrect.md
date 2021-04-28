---
title: Range:BoundingRect
description: .
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 38f0c1fe4346232878b6a76470a086b3fdd669c0
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055825"
---
# <a name="range-boundingrect"></a><span data-ttu-id="79386-103">Range:BoundingRect</span><span class="sxs-lookup"><span data-stu-id="79386-103">Range: BoundingRect</span></span>

<span data-ttu-id="79386-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79386-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="79386-p101">获取包含指定区域的最小 range 对象。例如，“B2:C5”和“D10:E15”的 GetBoundingRect 为“B2:E16”。</span><span class="sxs-lookup"><span data-stu-id="79386-p101">Gets the smallest range object that encompasses the given ranges. For example, the GetBoundingRect of "B2:C5" and "D10:E15" is "B2:E16".</span></span>
## <a name="permissions"></a><span data-ttu-id="79386-107">权限</span><span class="sxs-lookup"><span data-stu-id="79386-107">Permissions</span></span>
<span data-ttu-id="79386-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="79386-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79386-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="79386-110">Permission type</span></span>      | <span data-ttu-id="79386-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="79386-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="79386-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="79386-112">Delegated (work or school account)</span></span> | <span data-ttu-id="79386-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79386-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="79386-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="79386-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79386-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="79386-115">Not supported.</span></span>    |
|<span data-ttu-id="79386-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="79386-116">Application</span></span> | <span data-ttu-id="79386-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="79386-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="79386-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="79386-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/names/{name}/range/boundingRect
GET /me/drive/root:/{item-path}:/workbook/names/{name}/range/boundingRect
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/boundingRect
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/boundingRect
GET /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/boundingRect
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/boundingRect

```
## <a name="request-headers"></a><span data-ttu-id="79386-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="79386-119">Request headers</span></span>
| <span data-ttu-id="79386-120">名称</span><span class="sxs-lookup"><span data-stu-id="79386-120">Name</span></span>       | <span data-ttu-id="79386-121">说明</span><span class="sxs-lookup"><span data-stu-id="79386-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="79386-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="79386-122">Authorization</span></span>  | <span data-ttu-id="79386-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="79386-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="79386-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="79386-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="79386-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="79386-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="79386-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="79386-128">Request body</span></span>
<span data-ttu-id="79386-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="79386-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="79386-130">参数</span><span class="sxs-lookup"><span data-stu-id="79386-130">Parameter</span></span>    | <span data-ttu-id="79386-131">类型</span><span class="sxs-lookup"><span data-stu-id="79386-131">Type</span></span>   |<span data-ttu-id="79386-132">说明</span><span class="sxs-lookup"><span data-stu-id="79386-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="79386-133">anotherRange</span><span class="sxs-lookup"><span data-stu-id="79386-133">anotherRange</span></span>|<span data-ttu-id="79386-134">string</span><span class="sxs-lookup"><span data-stu-id="79386-134">string</span></span>|<span data-ttu-id="79386-135">Range 对象或地址或区域名称。</span><span class="sxs-lookup"><span data-stu-id="79386-135">The range object or address or range name.</span></span>|

## <a name="response"></a><span data-ttu-id="79386-136">响应</span><span class="sxs-lookup"><span data-stu-id="79386-136">Response</span></span>

<span data-ttu-id="79386-137">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="79386-137">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79386-138">示例</span><span class="sxs-lookup"><span data-stu-id="79386-138">Example</span></span>
<span data-ttu-id="79386-139">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="79386-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="79386-140">请求</span><span class="sxs-lookup"><span data-stu-id="79386-140">Request</span></span>
<span data-ttu-id="79386-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="79386-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "isComposable": true,
  "name": "range_boundingrect"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/boundingRect
Content-type: application/json
Content-length: 42

{
  "anotherRange": "anotherRange-value"
}
```

##### <a name="response"></a><span data-ttu-id="79386-142">响应</span><span class="sxs-lookup"><span data-stu-id="79386-142">Response</span></span>
<span data-ttu-id="79386-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="79386-143">Here is an example of the response.</span></span> <span data-ttu-id="79386-144">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="79386-144">Note: The response object shown here might be shortened for readability.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Range: BoundingRect",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

