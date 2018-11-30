---
title: 'Chart: setData'
description: 重置图表的源数据。
ms.openlocfilehash: 9996951ba24e8a473a1e23359c76506595f04c58
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010765"
---
# <a name="chart-setdata"></a><span data-ttu-id="a4487-103">Chart: setData</span><span class="sxs-lookup"><span data-stu-id="a4487-103">Chart: setData</span></span>

<span data-ttu-id="a4487-104">重置图表的源数据。</span><span class="sxs-lookup"><span data-stu-id="a4487-104">Resets the source data for the chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="a4487-105">权限</span><span class="sxs-lookup"><span data-stu-id="a4487-105">Permissions</span></span>
<span data-ttu-id="a4487-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a4487-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4487-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="a4487-108">Permission type</span></span>      | <span data-ttu-id="a4487-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a4487-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a4487-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a4487-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a4487-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a4487-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a4487-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a4487-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4487-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="a4487-113">Not supported.</span></span>    |
|<span data-ttu-id="a4487-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="a4487-114">Application</span></span> | <span data-ttu-id="a4487-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a4487-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a4487-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a4487-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/setData

```
## <a name="request-headers"></a><span data-ttu-id="a4487-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="a4487-117">Request headers</span></span>
| <span data-ttu-id="a4487-118">名称</span><span class="sxs-lookup"><span data-stu-id="a4487-118">Name</span></span>       | <span data-ttu-id="a4487-119">说明</span><span class="sxs-lookup"><span data-stu-id="a4487-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a4487-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4487-120">Authorization</span></span>  | <span data-ttu-id="a4487-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a4487-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a4487-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a4487-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="a4487-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="a4487-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4487-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a4487-126">Request body</span></span>
<span data-ttu-id="a4487-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="a4487-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a4487-128">参数</span><span class="sxs-lookup"><span data-stu-id="a4487-128">Parameter</span></span>    | <span data-ttu-id="a4487-129">类型</span><span class="sxs-lookup"><span data-stu-id="a4487-129">Type</span></span>   |<span data-ttu-id="a4487-130">说明</span><span class="sxs-lookup"><span data-stu-id="a4487-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a4487-131">sourceData</span><span class="sxs-lookup"><span data-stu-id="a4487-131">sourceData</span></span>|<span data-ttu-id="a4487-132">Json</span><span class="sxs-lookup"><span data-stu-id="a4487-132">Json</span></span>|<span data-ttu-id="a4487-133">对应于源数据的 Range 对象。</span><span class="sxs-lookup"><span data-stu-id="a4487-133">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="a4487-134">seriesBy</span><span class="sxs-lookup"><span data-stu-id="a4487-134">seriesBy</span></span>|<span data-ttu-id="a4487-135">string</span><span class="sxs-lookup"><span data-stu-id="a4487-135">string</span></span>|<span data-ttu-id="a4487-136">可选。</span><span class="sxs-lookup"><span data-stu-id="a4487-136">Optional.</span></span> <span data-ttu-id="a4487-137">指定的方式列或行用作图表上的数据系列。</span><span class="sxs-lookup"><span data-stu-id="a4487-137">Specifies the way columns or rows are used as data series on the chart.</span></span> <span data-ttu-id="a4487-138">可以是下列选项之一： 自动 （默认）、 行、 列。</span><span class="sxs-lookup"><span data-stu-id="a4487-138">Can be one of the following: Auto (default), Rows, Columns.</span></span>  <span data-ttu-id="a4487-139">可能的值为： `Auto`， `Columns`， `Rows`。</span><span class="sxs-lookup"><span data-stu-id="a4487-139">The possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="a4487-140">响应</span><span class="sxs-lookup"><span data-stu-id="a4487-140">Response</span></span>

<span data-ttu-id="a4487-p105">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="a4487-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4487-143">示例</span><span class="sxs-lookup"><span data-stu-id="a4487-143">Example</span></span>
<span data-ttu-id="a4487-144">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="a4487-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a4487-145">请求</span><span class="sxs-lookup"><span data-stu-id="a4487-145">Request</span></span>
<span data-ttu-id="a4487-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a4487-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chart_setdata"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/setData
Content-type: application/json
Content-length: 70

{
  "sourceData": "sourceData-value",
  "seriesBy": "seriesBy-value"
}
```

##### <a name="response"></a><span data-ttu-id="a4487-147">响应</span><span class="sxs-lookup"><span data-stu-id="a4487-147">Response</span></span>
<span data-ttu-id="a4487-148">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a4487-148">Here is an example of the response.</span></span> 
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
  "description": "Chart: setData",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->