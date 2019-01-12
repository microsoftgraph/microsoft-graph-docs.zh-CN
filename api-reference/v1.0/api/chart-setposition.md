---
title: 'Chart: setPosition'
description: 相对于工作表上的单元格放置图表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: d8e4c65954790fcebc885a84183b7941e2701e28
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981810"
---
# <a name="chart-setposition"></a><span data-ttu-id="57407-103">Chart: setPosition</span><span class="sxs-lookup"><span data-stu-id="57407-103">Chart: setPosition</span></span>

<span data-ttu-id="57407-104">相对于工作表上的单元格放置图表。</span><span class="sxs-lookup"><span data-stu-id="57407-104">Positions the chart relative to cells on the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="57407-105">权限</span><span class="sxs-lookup"><span data-stu-id="57407-105">Permissions</span></span>
<span data-ttu-id="57407-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="57407-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57407-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="57407-108">Permission type</span></span>      | <span data-ttu-id="57407-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="57407-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="57407-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="57407-110">Delegated (work or school account)</span></span> | <span data-ttu-id="57407-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="57407-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="57407-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="57407-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57407-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="57407-113">Not supported.</span></span>    |
|<span data-ttu-id="57407-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="57407-114">Application</span></span> | <span data-ttu-id="57407-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="57407-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="57407-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="57407-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/setPosition

```
## <a name="request-headers"></a><span data-ttu-id="57407-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="57407-117">Request headers</span></span>
| <span data-ttu-id="57407-118">名称</span><span class="sxs-lookup"><span data-stu-id="57407-118">Name</span></span>       | <span data-ttu-id="57407-119">说明</span><span class="sxs-lookup"><span data-stu-id="57407-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="57407-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="57407-120">Authorization</span></span>  | <span data-ttu-id="57407-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="57407-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="57407-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="57407-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="57407-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="57407-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="57407-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="57407-126">Request body</span></span>
<span data-ttu-id="57407-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="57407-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="57407-128">参数</span><span class="sxs-lookup"><span data-stu-id="57407-128">Parameter</span></span>    | <span data-ttu-id="57407-129">类型</span><span class="sxs-lookup"><span data-stu-id="57407-129">Type</span></span>   |<span data-ttu-id="57407-130">说明</span><span class="sxs-lookup"><span data-stu-id="57407-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="57407-131">startCell</span><span class="sxs-lookup"><span data-stu-id="57407-131">startCell</span></span>|<span data-ttu-id="57407-132">Json</span><span class="sxs-lookup"><span data-stu-id="57407-132">Json</span></span>|<span data-ttu-id="57407-p104">起始单元格。这是图表将移动到的位置。起始单元格为左上角或右上角的单元格，具体取决于用户的从右到左显示设置。</span><span class="sxs-lookup"><span data-stu-id="57407-p104">The start cell. This is where the chart will be moved to. The start cell is the top-left or top-right cell, depending on the user's right-to-left display settings.</span></span>|
|<span data-ttu-id="57407-136">endCell</span><span class="sxs-lookup"><span data-stu-id="57407-136">endCell</span></span>|<span data-ttu-id="57407-137">Json</span><span class="sxs-lookup"><span data-stu-id="57407-137">Json</span></span>|<span data-ttu-id="57407-p105">可选。结束单元格。如果已指定，图表的宽度和高度将设置为完全覆盖此单元格/区域。</span><span class="sxs-lookup"><span data-stu-id="57407-p105">Optional. The end cell. If specified, the chart's width and height will be set to fully cover up this cell/range.</span></span>|

## <a name="response"></a><span data-ttu-id="57407-141">响应</span><span class="sxs-lookup"><span data-stu-id="57407-141">Response</span></span>

<span data-ttu-id="57407-p106">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="57407-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57407-144">示例</span><span class="sxs-lookup"><span data-stu-id="57407-144">Example</span></span>
<span data-ttu-id="57407-145">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="57407-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="57407-146">请求</span><span class="sxs-lookup"><span data-stu-id="57407-146">Request</span></span>
<span data-ttu-id="57407-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="57407-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chart_setposition"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/setPosition
Content-type: application/json
Content-length: 66

{
  "startCell": "startCell-value",
  "endCell": "endCell-value"
}
```

##### <a name="response"></a><span data-ttu-id="57407-148">响应</span><span class="sxs-lookup"><span data-stu-id="57407-148">Response</span></span>
<span data-ttu-id="57407-149">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="57407-149">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
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
