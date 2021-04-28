---
title: 'ChartSeriesCollection: ItemAt'
description: 根据其在集合中的位置检索系列
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 8a48e21e592b7d353b968f09ced42def3f72fcc5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054103"
---
# <a name="chartseriescollection-itemat"></a><span data-ttu-id="794de-103">ChartSeriesCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="794de-103">ChartSeriesCollection: ItemAt</span></span>

<span data-ttu-id="794de-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="794de-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="794de-105">根据其在集合中的位置检索系列</span><span class="sxs-lookup"><span data-stu-id="794de-105">Retrieves a series based on its position in the collection</span></span>
## <a name="permissions"></a><span data-ttu-id="794de-106">权限</span><span class="sxs-lookup"><span data-stu-id="794de-106">Permissions</span></span>
<span data-ttu-id="794de-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="794de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="794de-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="794de-109">Permission type</span></span>      | <span data-ttu-id="794de-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="794de-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="794de-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="794de-111">Delegated (work or school account)</span></span> | <span data-ttu-id="794de-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="794de-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="794de-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="794de-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="794de-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="794de-114">Not supported.</span></span>    |
|<span data-ttu-id="794de-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="794de-115">Application</span></span> | <span data-ttu-id="794de-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="794de-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="794de-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="794de-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/itemAt
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/series/itemAt

```
## <a name="request-headers"></a><span data-ttu-id="794de-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="794de-118">Request headers</span></span>
| <span data-ttu-id="794de-119">名称</span><span class="sxs-lookup"><span data-stu-id="794de-119">Name</span></span>       | <span data-ttu-id="794de-120">说明</span><span class="sxs-lookup"><span data-stu-id="794de-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="794de-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="794de-121">Authorization</span></span>  | <span data-ttu-id="794de-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="794de-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="794de-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="794de-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="794de-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="794de-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="794de-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="794de-127">Request body</span></span>
<span data-ttu-id="794de-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="794de-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="794de-129">参数</span><span class="sxs-lookup"><span data-stu-id="794de-129">Parameter</span></span>    | <span data-ttu-id="794de-130">类型</span><span class="sxs-lookup"><span data-stu-id="794de-130">Type</span></span>   |<span data-ttu-id="794de-131">说明</span><span class="sxs-lookup"><span data-stu-id="794de-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="794de-132">index</span><span class="sxs-lookup"><span data-stu-id="794de-132">index</span></span>|<span data-ttu-id="794de-133">Int32</span><span class="sxs-lookup"><span data-stu-id="794de-133">Int32</span></span>|<span data-ttu-id="794de-p104">要检索的对象的索引值。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="794de-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="794de-136">响应</span><span class="sxs-lookup"><span data-stu-id="794de-136">Response</span></span>

<span data-ttu-id="794de-137">如果成功，此方法在 `200 OK` 响应正文中返回 响应代码和 [WorkbookChartSeries](../resources/chartseries.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="794de-137">If successful, this method returns `200 OK` response code and [WorkbookChartSeries](../resources/chartseries.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="794de-138">示例</span><span class="sxs-lookup"><span data-stu-id="794de-138">Example</span></span>
<span data-ttu-id="794de-139">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="794de-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="794de-140">请求</span><span class="sxs-lookup"><span data-stu-id="794de-140">Request</span></span>
<span data-ttu-id="794de-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="794de-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="794de-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="794de-142">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "chartseriescollection_itemat",
  "idempotent": true,
  "@type": "requestBodyResourceFor.chartseriescollection_itemat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/itemAt
Content-type: application/json
Content-length: 20

{
  "index": 2
}
```
# <a name="javascript"></a>[<span data-ttu-id="794de-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="794de-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chartseriescollection-itemat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="794de-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="794de-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chartseriescollection-itemat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="794de-145">响应</span><span class="sxs-lookup"><span data-stu-id="794de-145">Response</span></span>
<span data-ttu-id="794de-146">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="794de-146">Here is an example of the response.</span></span> <span data-ttu-id="794de-147">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="794de-147">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartSeries"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartSeriesCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

