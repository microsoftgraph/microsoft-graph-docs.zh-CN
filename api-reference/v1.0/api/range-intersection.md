---
title: Range:Intersection
description: 获取表示给定范围的矩形交集的 range 对象。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 95e7af555c1ac857272994dc634ed0dc9f1b0fad
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951633"
---
# <a name="range-intersection"></a><span data-ttu-id="cd0cc-103">Range:Intersection</span><span class="sxs-lookup"><span data-stu-id="cd0cc-103">Range: Intersection</span></span>

<span data-ttu-id="cd0cc-104">获取表示给定范围的矩形交集的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="cd0cc-104">Gets the range object that represents the rectangular intersection of the given ranges.</span></span>
## <a name="permissions"></a><span data-ttu-id="cd0cc-105">权限</span><span class="sxs-lookup"><span data-stu-id="cd0cc-105">Permissions</span></span>
<span data-ttu-id="cd0cc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cd0cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd0cc-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="cd0cc-108">Permission type</span></span>      | <span data-ttu-id="cd0cc-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cd0cc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cd0cc-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cd0cc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cd0cc-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cd0cc-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cd0cc-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cd0cc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd0cc-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="cd0cc-113">Not supported.</span></span>    |
|<span data-ttu-id="cd0cc-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="cd0cc-114">Application</span></span> | <span data-ttu-id="cd0cc-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cd0cc-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cd0cc-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cd0cc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/intersection
GET /workbook/worksheets/{id|name}/range(address='<address>')/intersection
GET /workbook/tables/{id|name}/columns/{id|name}/range/intersection

```
## <a name="request-headers"></a><span data-ttu-id="cd0cc-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="cd0cc-117">Request headers</span></span>
| <span data-ttu-id="cd0cc-118">名称</span><span class="sxs-lookup"><span data-stu-id="cd0cc-118">Name</span></span>       | <span data-ttu-id="cd0cc-119">说明</span><span class="sxs-lookup"><span data-stu-id="cd0cc-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cd0cc-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd0cc-120">Authorization</span></span>  | <span data-ttu-id="cd0cc-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cd0cc-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cd0cc-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="cd0cc-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="cd0cc-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="cd0cc-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd0cc-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="cd0cc-126">Request body</span></span>
<span data-ttu-id="cd0cc-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="cd0cc-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cd0cc-128">参数</span><span class="sxs-lookup"><span data-stu-id="cd0cc-128">Parameter</span></span>    | <span data-ttu-id="cd0cc-129">类型</span><span class="sxs-lookup"><span data-stu-id="cd0cc-129">Type</span></span>   |<span data-ttu-id="cd0cc-130">说明</span><span class="sxs-lookup"><span data-stu-id="cd0cc-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cd0cc-131">anotherRange</span><span class="sxs-lookup"><span data-stu-id="cd0cc-131">anotherRange</span></span>|<span data-ttu-id="cd0cc-132">string</span><span class="sxs-lookup"><span data-stu-id="cd0cc-132">string</span></span>|<span data-ttu-id="cd0cc-133">将用于确定区域交集的 range 对象或区域地址。</span><span class="sxs-lookup"><span data-stu-id="cd0cc-133">The range object or range address that will be used to determine the intersection of ranges.</span></span>|

## <a name="response"></a><span data-ttu-id="cd0cc-134">响应</span><span class="sxs-lookup"><span data-stu-id="cd0cc-134">Response</span></span>

<span data-ttu-id="cd0cc-135">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cd0cc-135">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd0cc-136">示例</span><span class="sxs-lookup"><span data-stu-id="cd0cc-136">Example</span></span>
<span data-ttu-id="cd0cc-137">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="cd0cc-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="cd0cc-138">请求</span><span class="sxs-lookup"><span data-stu-id="cd0cc-138">Request</span></span>
<span data-ttu-id="cd0cc-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cd0cc-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "isComposable": true,
  "name": "range_intersection"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/intersection
Content-type: application/json
Content-length: 42

{
  "anotherRange": "anotherRange-value"
}
```

##### <a name="response"></a><span data-ttu-id="cd0cc-140">响应</span><span class="sxs-lookup"><span data-stu-id="cd0cc-140">Response</span></span>
<span data-ttu-id="cd0cc-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cd0cc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: Intersection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
