---
title: 'Chart: setData'
description: 重置图表的源数据。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 37051d504cbce577b5c4e5ba46b37722dfc7eb65
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786196"
---
# <a name="chart-setdata"></a><span data-ttu-id="41808-103">Chart: setData</span><span class="sxs-lookup"><span data-stu-id="41808-103">Chart: setData</span></span>

<span data-ttu-id="41808-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41808-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41808-105">重置图表的源数据。</span><span class="sxs-lookup"><span data-stu-id="41808-105">Resets the source data for the chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="41808-106">权限</span><span class="sxs-lookup"><span data-stu-id="41808-106">Permissions</span></span>
<span data-ttu-id="41808-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="41808-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41808-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="41808-109">Permission type</span></span>      | <span data-ttu-id="41808-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="41808-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="41808-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="41808-111">Delegated (work or school account)</span></span> | <span data-ttu-id="41808-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="41808-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="41808-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="41808-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41808-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="41808-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="41808-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="41808-115">Application</span></span> | <span data-ttu-id="41808-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="41808-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="41808-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="41808-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/setData
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/setData

```
## <a name="request-headers"></a><span data-ttu-id="41808-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="41808-118">Request headers</span></span>
| <span data-ttu-id="41808-119">名称</span><span class="sxs-lookup"><span data-stu-id="41808-119">Name</span></span>       | <span data-ttu-id="41808-120">说明</span><span class="sxs-lookup"><span data-stu-id="41808-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="41808-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="41808-121">Authorization</span></span>  | <span data-ttu-id="41808-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="41808-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="41808-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="41808-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="41808-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="41808-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="41808-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="41808-127">Request body</span></span>
<span data-ttu-id="41808-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="41808-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="41808-129">参数</span><span class="sxs-lookup"><span data-stu-id="41808-129">Parameter</span></span>    | <span data-ttu-id="41808-130">类型</span><span class="sxs-lookup"><span data-stu-id="41808-130">Type</span></span>   |<span data-ttu-id="41808-131">说明</span><span class="sxs-lookup"><span data-stu-id="41808-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="41808-132">sourceData</span><span class="sxs-lookup"><span data-stu-id="41808-132">sourceData</span></span>|<span data-ttu-id="41808-133">string</span><span class="sxs-lookup"><span data-stu-id="41808-133">string</span></span>|<span data-ttu-id="41808-134">对应于源数据的 Range 对象。</span><span class="sxs-lookup"><span data-stu-id="41808-134">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="41808-135">seriesBy</span><span class="sxs-lookup"><span data-stu-id="41808-135">seriesBy</span></span>|<span data-ttu-id="41808-136">string</span><span class="sxs-lookup"><span data-stu-id="41808-136">string</span></span>|<span data-ttu-id="41808-p104">可选。指定列或行在图表上用作数据系列的方式。可以是下列值之一：自动（默认）、行、列。可能的值是：`Auto`、`Columns`、`Rows`。</span><span class="sxs-lookup"><span data-stu-id="41808-p104">Optional. Specifies the way columns or rows are used as data series on the chart. Can be one of the following: Auto (default), Rows, Columns.  Possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="41808-141">响应</span><span class="sxs-lookup"><span data-stu-id="41808-141">Response</span></span>

<span data-ttu-id="41808-p105">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="41808-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41808-144">示例</span><span class="sxs-lookup"><span data-stu-id="41808-144">Example</span></span>
<span data-ttu-id="41808-145">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="41808-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="41808-146">请求</span><span class="sxs-lookup"><span data-stu-id="41808-146">Request</span></span>
<span data-ttu-id="41808-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="41808-147">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="41808-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="41808-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chart_setdata"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/setData
Content-type: application/json
Content-length: 70

{
  "sourceData": "sourceData-value",
  "seriesBy": "seriesBy-value"
}
```
# <a name="c"></a>[<span data-ttu-id="41808-149">C#</span><span class="sxs-lookup"><span data-stu-id="41808-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chart-setdata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="41808-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="41808-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chart-setdata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="41808-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="41808-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chart-setdata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="41808-152">Java</span><span class="sxs-lookup"><span data-stu-id="41808-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chart-setdata-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="41808-153">响应</span><span class="sxs-lookup"><span data-stu-id="41808-153">Response</span></span>
<span data-ttu-id="41808-154">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="41808-154">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Chart: setData",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


