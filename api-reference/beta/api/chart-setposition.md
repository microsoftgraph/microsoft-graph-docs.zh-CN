---
title: 'Chart: setPosition'
description: 相对于工作表上的单元格放置图表。
author: lumine2008
ms.openlocfilehash: 8d5a5f2b599d9d3b3902c8bbb5feec2d8178a6e6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314922"
---
# <a name="chart-setposition"></a><span data-ttu-id="b8bba-103">Chart: setPosition</span><span class="sxs-lookup"><span data-stu-id="b8bba-103">Chart: setPosition</span></span>

> <span data-ttu-id="b8bba-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b8bba-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b8bba-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b8bba-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b8bba-106">相对于工作表上的单元格放置图表。</span><span class="sxs-lookup"><span data-stu-id="b8bba-106">Positions the chart relative to cells on the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="b8bba-107">权限</span><span class="sxs-lookup"><span data-stu-id="b8bba-107">Permissions</span></span>
<span data-ttu-id="b8bba-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b8bba-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8bba-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b8bba-110">Permission type</span></span>      | <span data-ttu-id="b8bba-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b8bba-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b8bba-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b8bba-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b8bba-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b8bba-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b8bba-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b8bba-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8bba-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b8bba-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b8bba-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b8bba-116">Application</span></span> | <span data-ttu-id="b8bba-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b8bba-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b8bba-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b8bba-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/setPosition

```
## <a name="request-headers"></a><span data-ttu-id="b8bba-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b8bba-119">Request headers</span></span>
| <span data-ttu-id="b8bba-120">Name</span><span class="sxs-lookup"><span data-stu-id="b8bba-120">Name</span></span>       | <span data-ttu-id="b8bba-121">说明</span><span class="sxs-lookup"><span data-stu-id="b8bba-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b8bba-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8bba-122">Authorization</span></span>  | <span data-ttu-id="b8bba-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b8bba-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b8bba-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b8bba-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="b8bba-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="b8bba-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8bba-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="b8bba-128">Request body</span></span>
<span data-ttu-id="b8bba-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="b8bba-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b8bba-130">参数</span><span class="sxs-lookup"><span data-stu-id="b8bba-130">Parameter</span></span>    | <span data-ttu-id="b8bba-131">Type</span><span class="sxs-lookup"><span data-stu-id="b8bba-131">Type</span></span>   |<span data-ttu-id="b8bba-132">说明</span><span class="sxs-lookup"><span data-stu-id="b8bba-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8bba-133">startCell</span><span class="sxs-lookup"><span data-stu-id="b8bba-133">startCell</span></span>|<span data-ttu-id="b8bba-134">string</span><span class="sxs-lookup"><span data-stu-id="b8bba-134">string</span></span>|<span data-ttu-id="b8bba-p105">起始单元格。这是图表将移动到的位置。起始单元格为左上角或右上角的单元格，具体取决于用户的从右到左显示设置。</span><span class="sxs-lookup"><span data-stu-id="b8bba-p105">The start cell. This is where the chart will be moved to. The start cell is the top-left or top-right cell, depending on the user's right-to-left display settings.</span></span>|
|<span data-ttu-id="b8bba-138">endCell</span><span class="sxs-lookup"><span data-stu-id="b8bba-138">endCell</span></span>|<span data-ttu-id="b8bba-139">string</span><span class="sxs-lookup"><span data-stu-id="b8bba-139">string</span></span>|<span data-ttu-id="b8bba-p106">可选。结束单元格。如果已指定，图表的宽度和高度将设置为完全覆盖此单元格/区域。</span><span class="sxs-lookup"><span data-stu-id="b8bba-p106">Optional. The end cell. If specified, the chart's width and height will be set to fully cover up this cell/range.</span></span>|

## <a name="response"></a><span data-ttu-id="b8bba-143">响应</span><span class="sxs-lookup"><span data-stu-id="b8bba-143">Response</span></span>

<span data-ttu-id="b8bba-p107">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b8bba-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8bba-146">示例</span><span class="sxs-lookup"><span data-stu-id="b8bba-146">Example</span></span>
<span data-ttu-id="b8bba-147">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="b8bba-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b8bba-148">请求</span><span class="sxs-lookup"><span data-stu-id="b8bba-148">Request</span></span>
<span data-ttu-id="b8bba-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b8bba-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chart_setposition"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/setPosition
Content-type: application/json
Content-length: 66

{
  "startCell": "startCell-value",
  "endCell": "endCell-value"
}
```

##### <a name="response"></a><span data-ttu-id="b8bba-150">响应</span><span class="sxs-lookup"><span data-stu-id="b8bba-150">Response</span></span>
<span data-ttu-id="b8bba-151">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b8bba-151">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chart: setPosition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->