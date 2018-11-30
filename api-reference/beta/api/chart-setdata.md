---
title: 'Chart: setData'
description: 重置图表的源数据。
ms.openlocfilehash: 0646bf77175fbd81feffc8c2fb26ce2179afcaa5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041378"
---
# <a name="chart-setdata"></a><span data-ttu-id="f50d5-103">Chart: setData</span><span class="sxs-lookup"><span data-stu-id="f50d5-103">Chart: setData</span></span>

> <span data-ttu-id="f50d5-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f50d5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f50d5-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f50d5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f50d5-106">重置图表的源数据。</span><span class="sxs-lookup"><span data-stu-id="f50d5-106">Resets the source data for the chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="f50d5-107">权限</span><span class="sxs-lookup"><span data-stu-id="f50d5-107">Permissions</span></span>
<span data-ttu-id="f50d5-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f50d5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f50d5-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f50d5-110">Permission type</span></span>      | <span data-ttu-id="f50d5-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f50d5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f50d5-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f50d5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f50d5-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f50d5-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f50d5-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f50d5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f50d5-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f50d5-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f50d5-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f50d5-116">Application</span></span> | <span data-ttu-id="f50d5-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f50d5-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f50d5-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f50d5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/setData

```
## <a name="request-headers"></a><span data-ttu-id="f50d5-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f50d5-119">Request headers</span></span>
| <span data-ttu-id="f50d5-120">名称</span><span class="sxs-lookup"><span data-stu-id="f50d5-120">Name</span></span>       | <span data-ttu-id="f50d5-121">说明</span><span class="sxs-lookup"><span data-stu-id="f50d5-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f50d5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f50d5-122">Authorization</span></span>  | <span data-ttu-id="f50d5-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f50d5-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f50d5-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f50d5-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="f50d5-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="f50d5-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f50d5-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="f50d5-128">Request body</span></span>
<span data-ttu-id="f50d5-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="f50d5-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f50d5-130">参数</span><span class="sxs-lookup"><span data-stu-id="f50d5-130">Parameter</span></span>    | <span data-ttu-id="f50d5-131">类型</span><span class="sxs-lookup"><span data-stu-id="f50d5-131">Type</span></span>   |<span data-ttu-id="f50d5-132">说明</span><span class="sxs-lookup"><span data-stu-id="f50d5-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f50d5-133">sourceData</span><span class="sxs-lookup"><span data-stu-id="f50d5-133">sourceData</span></span>|<span data-ttu-id="f50d5-134">string</span><span class="sxs-lookup"><span data-stu-id="f50d5-134">string</span></span>|<span data-ttu-id="f50d5-135">对应于源数据的 Range 对象。</span><span class="sxs-lookup"><span data-stu-id="f50d5-135">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="f50d5-136">seriesBy</span><span class="sxs-lookup"><span data-stu-id="f50d5-136">seriesBy</span></span>|<span data-ttu-id="f50d5-137">string</span><span class="sxs-lookup"><span data-stu-id="f50d5-137">string</span></span>|<span data-ttu-id="f50d5-p105">可选。指定列或行在图表上用作数据系列的方式。可以是下列值之一：自动（默认）、行、列。可能的值是：`Auto`、`Columns`、`Rows`。</span><span class="sxs-lookup"><span data-stu-id="f50d5-p105">Optional. Specifies the way columns or rows are used as data series on the chart. Can be one of the following: Auto (default), Rows, Columns.  Possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="f50d5-142">响应</span><span class="sxs-lookup"><span data-stu-id="f50d5-142">Response</span></span>

<span data-ttu-id="f50d5-p106">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f50d5-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f50d5-145">示例</span><span class="sxs-lookup"><span data-stu-id="f50d5-145">Example</span></span>
<span data-ttu-id="f50d5-146">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="f50d5-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f50d5-147">请求</span><span class="sxs-lookup"><span data-stu-id="f50d5-147">Request</span></span>
<span data-ttu-id="f50d5-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f50d5-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chart_setdata"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/setData
Content-type: application/json
Content-length: 70

{
  "sourceData": "sourceData-value",
  "seriesBy": "seriesBy-value"
}
```

##### <a name="response"></a><span data-ttu-id="f50d5-149">响应</span><span class="sxs-lookup"><span data-stu-id="f50d5-149">Response</span></span>
<span data-ttu-id="f50d5-150">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f50d5-150">Here is an example of the response.</span></span> 
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
  "description": "Chart: setData",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->