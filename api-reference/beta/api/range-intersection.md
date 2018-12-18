---
title: Range:Intersection
description: 获取表示给定范围的矩形交集的 range 对象。
author: lumine2008
ms.openlocfilehash: 0ba9767c3c7d30ee5746b5a6723fd8103c1b8533
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344553"
---
# <a name="range-intersection"></a><span data-ttu-id="8f8e2-103">Range:Intersection</span><span class="sxs-lookup"><span data-stu-id="8f8e2-103">Range: Intersection</span></span>

> <span data-ttu-id="8f8e2-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8f8e2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8f8e2-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8f8e2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8f8e2-106">获取表示给定范围的矩形交集的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="8f8e2-106">Gets the range object that represents the rectangular intersection of the given ranges.</span></span>
## <a name="permissions"></a><span data-ttu-id="8f8e2-107">权限</span><span class="sxs-lookup"><span data-stu-id="8f8e2-107">Permissions</span></span>
<span data-ttu-id="8f8e2-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8f8e2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f8e2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8f8e2-110">Permission type</span></span>      | <span data-ttu-id="8f8e2-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8f8e2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8f8e2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8f8e2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8f8e2-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8f8e2-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8f8e2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8f8e2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f8e2-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8f8e2-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8f8e2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8f8e2-116">Application</span></span> | <span data-ttu-id="8f8e2-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="8f8e2-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f8e2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8f8e2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/Intersection
GET /workbook/worksheets/{id|name}/range(address='<address>')/Intersection
GET /workbook/tables/{id|name}/columns/{id|name}/range/Intersection

```
## <a name="request-headers"></a><span data-ttu-id="8f8e2-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8f8e2-119">Request headers</span></span>
| <span data-ttu-id="8f8e2-120">Name</span><span class="sxs-lookup"><span data-stu-id="8f8e2-120">Name</span></span>       | <span data-ttu-id="8f8e2-121">说明</span><span class="sxs-lookup"><span data-stu-id="8f8e2-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8f8e2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f8e2-122">Authorization</span></span>  | <span data-ttu-id="8f8e2-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8f8e2-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8f8e2-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8f8e2-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="8f8e2-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="8f8e2-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f8e2-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="8f8e2-128">Request body</span></span>
<span data-ttu-id="8f8e2-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="8f8e2-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8f8e2-130">参数</span><span class="sxs-lookup"><span data-stu-id="8f8e2-130">Parameter</span></span>    | <span data-ttu-id="8f8e2-131">Type</span><span class="sxs-lookup"><span data-stu-id="8f8e2-131">Type</span></span>   |<span data-ttu-id="8f8e2-132">说明</span><span class="sxs-lookup"><span data-stu-id="8f8e2-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8f8e2-133">anotherRange</span><span class="sxs-lookup"><span data-stu-id="8f8e2-133">anotherRange</span></span>|<span data-ttu-id="8f8e2-134">string</span><span class="sxs-lookup"><span data-stu-id="8f8e2-134">string</span></span>|<span data-ttu-id="8f8e2-135">将用于确定区域交集的 range 对象或区域地址。</span><span class="sxs-lookup"><span data-stu-id="8f8e2-135">The range object or range address that will be used to determine the intersection of ranges.</span></span>|

## <a name="response"></a><span data-ttu-id="8f8e2-136">响应</span><span class="sxs-lookup"><span data-stu-id="8f8e2-136">Response</span></span>

<span data-ttu-id="8f8e2-137">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8f8e2-137">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f8e2-138">示例</span><span class="sxs-lookup"><span data-stu-id="8f8e2-138">Example</span></span>
<span data-ttu-id="8f8e2-139">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="8f8e2-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8f8e2-140">请求</span><span class="sxs-lookup"><span data-stu-id="8f8e2-140">Request</span></span>
<span data-ttu-id="8f8e2-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8f8e2-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_intersection"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/Intersection
Content-type: application/json
Content-length: 42

{
  "anotherRange": "anotherRange-value"
}
```

##### <a name="response"></a><span data-ttu-id="8f8e2-142">响应</span><span class="sxs-lookup"><span data-stu-id="8f8e2-142">Response</span></span>
<span data-ttu-id="8f8e2-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8f8e2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
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