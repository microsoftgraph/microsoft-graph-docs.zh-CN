---
title: Worksheet:Range
description: 获取地址或名称指定的 range 对象。
ms.openlocfilehash: defe05f953d5fe7cd5fafda6ae16f04bb9f91e86
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046074"
---
# <a name="worksheet-range"></a><span data-ttu-id="87102-103">Worksheet:Range</span><span class="sxs-lookup"><span data-stu-id="87102-103">Worksheet: Range</span></span>

> <span data-ttu-id="87102-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="87102-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="87102-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="87102-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="87102-106">获取地址或名称指定的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="87102-106">Gets the range object specified by the address or name.</span></span>
## <a name="permissions"></a><span data-ttu-id="87102-107">权限</span><span class="sxs-lookup"><span data-stu-id="87102-107">Permissions</span></span>
<span data-ttu-id="87102-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="87102-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87102-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="87102-110">Permission type</span></span>      | <span data-ttu-id="87102-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="87102-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87102-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="87102-112">Delegated (work or school account)</span></span> | <span data-ttu-id="87102-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="87102-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="87102-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="87102-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87102-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="87102-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="87102-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="87102-116">Application</span></span> | <span data-ttu-id="87102-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="87102-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="87102-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="87102-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/Range

```
## <a name="request-headers"></a><span data-ttu-id="87102-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="87102-119">Request headers</span></span>
| <span data-ttu-id="87102-120">名称</span><span class="sxs-lookup"><span data-stu-id="87102-120">Name</span></span>       | <span data-ttu-id="87102-121">说明</span><span class="sxs-lookup"><span data-stu-id="87102-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="87102-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="87102-122">Authorization</span></span>  | <span data-ttu-id="87102-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="87102-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="87102-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="87102-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="87102-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="87102-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="87102-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="87102-128">Request body</span></span>
<span data-ttu-id="87102-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="87102-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="87102-130">参数</span><span class="sxs-lookup"><span data-stu-id="87102-130">Parameter</span></span>    | <span data-ttu-id="87102-131">类型</span><span class="sxs-lookup"><span data-stu-id="87102-131">Type</span></span>   |<span data-ttu-id="87102-132">说明</span><span class="sxs-lookup"><span data-stu-id="87102-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="87102-133">address</span><span class="sxs-lookup"><span data-stu-id="87102-133">address</span></span>|<span data-ttu-id="87102-134">string</span><span class="sxs-lookup"><span data-stu-id="87102-134">string</span></span>|<span data-ttu-id="87102-p105">可选。区域的地址或名称。如果未指定，则返回整个工作表区域。</span><span class="sxs-lookup"><span data-stu-id="87102-p105">Optional. The address or the name of the range. If not specified, the entire worksheet range is returned.</span></span>|

## <a name="response"></a><span data-ttu-id="87102-138">响应</span><span class="sxs-lookup"><span data-stu-id="87102-138">Response</span></span>

<span data-ttu-id="87102-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="87102-139">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87102-140">示例</span><span class="sxs-lookup"><span data-stu-id="87102-140">Example</span></span>
<span data-ttu-id="87102-141">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="87102-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="87102-142">请求</span><span class="sxs-lookup"><span data-stu-id="87102-142">Request</span></span>
<span data-ttu-id="87102-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="87102-143">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="87102-144">响应</span><span class="sxs-lookup"><span data-stu-id="87102-144">Response</span></span>
<span data-ttu-id="87102-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="87102-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Worksheet: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->