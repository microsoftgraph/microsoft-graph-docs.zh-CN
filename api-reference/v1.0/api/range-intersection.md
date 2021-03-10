---
title: Range:Intersection
description: 获取表示给定范围的矩形交集的 range 对象。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: bceba8e704b1a4c3e0ee485b8c10643f9bf84e4c
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50577707"
---
# <a name="range-intersection"></a><span data-ttu-id="8d096-103">Range:Intersection</span><span class="sxs-lookup"><span data-stu-id="8d096-103">Range: Intersection</span></span>

<span data-ttu-id="8d096-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d096-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8d096-105">获取表示给定范围的矩形交集的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="8d096-105">Gets the range object that represents the rectangular intersection of the given ranges.</span></span>
## <a name="permissions"></a><span data-ttu-id="8d096-106">权限</span><span class="sxs-lookup"><span data-stu-id="8d096-106">Permissions</span></span>
<span data-ttu-id="8d096-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8d096-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d096-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8d096-109">Permission type</span></span>      | <span data-ttu-id="8d096-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8d096-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d096-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8d096-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8d096-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8d096-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8d096-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8d096-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d096-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8d096-114">Not supported.</span></span>    |
|<span data-ttu-id="8d096-115">Application</span><span class="sxs-lookup"><span data-stu-id="8d096-115">Application</span></span> | <span data-ttu-id="8d096-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8d096-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8d096-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8d096-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/names/{name}/range/intersection
GET /me/drive/root:/{item-path}:/workbook/names/{name}/range/intersection
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/intersection
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/intersection
GET /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/intersection
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/intersection

```
## <a name="request-headers"></a><span data-ttu-id="8d096-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="8d096-118">Request headers</span></span>
| <span data-ttu-id="8d096-119">名称</span><span class="sxs-lookup"><span data-stu-id="8d096-119">Name</span></span>       | <span data-ttu-id="8d096-120">说明</span><span class="sxs-lookup"><span data-stu-id="8d096-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8d096-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d096-121">Authorization</span></span>  | <span data-ttu-id="8d096-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8d096-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8d096-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8d096-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="8d096-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="8d096-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d096-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8d096-127">Request body</span></span>
<span data-ttu-id="8d096-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="8d096-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8d096-129">参数</span><span class="sxs-lookup"><span data-stu-id="8d096-129">Parameter</span></span>    | <span data-ttu-id="8d096-130">类型</span><span class="sxs-lookup"><span data-stu-id="8d096-130">Type</span></span>   |<span data-ttu-id="8d096-131">说明</span><span class="sxs-lookup"><span data-stu-id="8d096-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8d096-132">anotherRange</span><span class="sxs-lookup"><span data-stu-id="8d096-132">anotherRange</span></span>|<span data-ttu-id="8d096-133">string</span><span class="sxs-lookup"><span data-stu-id="8d096-133">string</span></span>|<span data-ttu-id="8d096-134">将用于确定区域交集的 range 对象或区域地址。</span><span class="sxs-lookup"><span data-stu-id="8d096-134">The range object or range address that will be used to determine the intersection of ranges.</span></span>|

## <a name="response"></a><span data-ttu-id="8d096-135">响应</span><span class="sxs-lookup"><span data-stu-id="8d096-135">Response</span></span>

<span data-ttu-id="8d096-136">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8d096-136">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d096-137">示例</span><span class="sxs-lookup"><span data-stu-id="8d096-137">Example</span></span>
<span data-ttu-id="8d096-138">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="8d096-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8d096-139">请求</span><span class="sxs-lookup"><span data-stu-id="8d096-139">Request</span></span>
<span data-ttu-id="8d096-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8d096-140">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="8d096-141">响应</span><span class="sxs-lookup"><span data-stu-id="8d096-141">Response</span></span>
<span data-ttu-id="8d096-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8d096-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

