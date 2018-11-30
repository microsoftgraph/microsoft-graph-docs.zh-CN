---
title: Range:BoundingRect
description: .
ms.openlocfilehash: 25a313fca1fe73c0717777b4dabc4c9b6eb9372f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041466"
---
# <a name="range-boundingrect"></a><span data-ttu-id="c63ff-103">Range:BoundingRect</span><span class="sxs-lookup"><span data-stu-id="c63ff-103">Range: BoundingRect</span></span>

> <span data-ttu-id="c63ff-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c63ff-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c63ff-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c63ff-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c63ff-p102">获取包含指定区域的最小 range 对象。例如，“B2:C5”和“D10:E15”的 GetBoundingRect 为“B2:E16”。</span><span class="sxs-lookup"><span data-stu-id="c63ff-p102">Gets the smallest range object that encompasses the given ranges. For example, the GetBoundingRect of "B2:C5" and "D10:E15" is "B2:E16".</span></span>
## <a name="permissions"></a><span data-ttu-id="c63ff-108">权限</span><span class="sxs-lookup"><span data-stu-id="c63ff-108">Permissions</span></span>
<span data-ttu-id="c63ff-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c63ff-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c63ff-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c63ff-111">Permission type</span></span>      | <span data-ttu-id="c63ff-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c63ff-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c63ff-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c63ff-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c63ff-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c63ff-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c63ff-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c63ff-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c63ff-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c63ff-116">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c63ff-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c63ff-117">Application</span></span> | <span data-ttu-id="c63ff-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c63ff-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c63ff-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c63ff-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/BoundingRect
GET /workbook/worksheets/{id|name}/range(address='<address>')/BoundingRect
GET /workbook/tables/{id|name}/columns/{id|name}/range/BoundingRect

```
## <a name="request-headers"></a><span data-ttu-id="c63ff-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c63ff-120">Request headers</span></span>
| <span data-ttu-id="c63ff-121">名称</span><span class="sxs-lookup"><span data-stu-id="c63ff-121">Name</span></span>       | <span data-ttu-id="c63ff-122">说明</span><span class="sxs-lookup"><span data-stu-id="c63ff-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c63ff-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c63ff-123">Authorization</span></span>  | <span data-ttu-id="c63ff-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c63ff-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c63ff-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c63ff-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="c63ff-p105">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="c63ff-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c63ff-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="c63ff-129">Request body</span></span>
<span data-ttu-id="c63ff-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="c63ff-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c63ff-131">参数</span><span class="sxs-lookup"><span data-stu-id="c63ff-131">Parameter</span></span>    | <span data-ttu-id="c63ff-132">类型</span><span class="sxs-lookup"><span data-stu-id="c63ff-132">Type</span></span>   |<span data-ttu-id="c63ff-133">说明</span><span class="sxs-lookup"><span data-stu-id="c63ff-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c63ff-134">anotherRange</span><span class="sxs-lookup"><span data-stu-id="c63ff-134">anotherRange</span></span>|<span data-ttu-id="c63ff-135">string</span><span class="sxs-lookup"><span data-stu-id="c63ff-135">string</span></span>|<span data-ttu-id="c63ff-136">Range 对象或地址或区域名称。</span><span class="sxs-lookup"><span data-stu-id="c63ff-136">The range object or address or range name.</span></span>|

## <a name="response"></a><span data-ttu-id="c63ff-137">响应</span><span class="sxs-lookup"><span data-stu-id="c63ff-137">Response</span></span>

<span data-ttu-id="c63ff-138">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c63ff-138">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c63ff-139">示例</span><span class="sxs-lookup"><span data-stu-id="c63ff-139">Example</span></span>
<span data-ttu-id="c63ff-140">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="c63ff-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c63ff-141">请求</span><span class="sxs-lookup"><span data-stu-id="c63ff-141">Request</span></span>
<span data-ttu-id="c63ff-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c63ff-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_boundingrect"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/BoundingRect
Content-type: application/json
Content-length: 42

{
  "anotherRange": "anotherRange-value"
}
```

##### <a name="response"></a><span data-ttu-id="c63ff-143">响应</span><span class="sxs-lookup"><span data-stu-id="c63ff-143">Response</span></span>
<span data-ttu-id="c63ff-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c63ff-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: BoundingRect",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->