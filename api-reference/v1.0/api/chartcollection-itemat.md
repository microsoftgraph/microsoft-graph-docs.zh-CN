---
title: 'ChartCollection: ItemAt'
description: 根据其在集合中的位置获取图表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: a0c91ad7fd24ab75e44936c442dce6d3beff9a34
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048818"
---
# <a name="chartcollection-itemat"></a><span data-ttu-id="5d1a1-103">ChartCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="5d1a1-103">ChartCollection: ItemAt</span></span>

<span data-ttu-id="5d1a1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d1a1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5d1a1-105">根据其在集合中的位置获取图表。</span><span class="sxs-lookup"><span data-stu-id="5d1a1-105">Gets a chart based on its position in the collection.</span></span>
## <a name="permissions"></a><span data-ttu-id="5d1a1-106">权限</span><span class="sxs-lookup"><span data-stu-id="5d1a1-106">Permissions</span></span>
<span data-ttu-id="5d1a1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5d1a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d1a1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5d1a1-109">Permission type</span></span>      | <span data-ttu-id="5d1a1-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5d1a1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d1a1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5d1a1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5d1a1-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5d1a1-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5d1a1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5d1a1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d1a1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5d1a1-114">Not supported.</span></span>    |
|<span data-ttu-id="5d1a1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5d1a1-115">Application</span></span> | <span data-ttu-id="5d1a1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5d1a1-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d1a1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5d1a1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/itemAt
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/itemAt

```
## <a name="request-headers"></a><span data-ttu-id="5d1a1-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="5d1a1-118">Request headers</span></span>
| <span data-ttu-id="5d1a1-119">名称</span><span class="sxs-lookup"><span data-stu-id="5d1a1-119">Name</span></span>       | <span data-ttu-id="5d1a1-120">说明</span><span class="sxs-lookup"><span data-stu-id="5d1a1-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5d1a1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d1a1-121">Authorization</span></span>  | <span data-ttu-id="5d1a1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5d1a1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5d1a1-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="5d1a1-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="5d1a1-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="5d1a1-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d1a1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5d1a1-127">Request body</span></span>
<span data-ttu-id="5d1a1-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="5d1a1-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5d1a1-129">参数</span><span class="sxs-lookup"><span data-stu-id="5d1a1-129">Parameter</span></span>    | <span data-ttu-id="5d1a1-130">类型</span><span class="sxs-lookup"><span data-stu-id="5d1a1-130">Type</span></span>   |<span data-ttu-id="5d1a1-131">说明</span><span class="sxs-lookup"><span data-stu-id="5d1a1-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5d1a1-132">index</span><span class="sxs-lookup"><span data-stu-id="5d1a1-132">index</span></span>|<span data-ttu-id="5d1a1-133">Int32</span><span class="sxs-lookup"><span data-stu-id="5d1a1-133">Int32</span></span>|<span data-ttu-id="5d1a1-p104">要检索的对象的索引值。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="5d1a1-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="5d1a1-136">响应</span><span class="sxs-lookup"><span data-stu-id="5d1a1-136">Response</span></span>

<span data-ttu-id="5d1a1-137">如果成功，此方法在 `200 OK` 响应正文中返回 响应代码和 [WorkbookChart](../resources/chart.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5d1a1-137">If successful, this method returns `200 OK` response code and [WorkbookChart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d1a1-138">示例</span><span class="sxs-lookup"><span data-stu-id="5d1a1-138">Example</span></span>
<span data-ttu-id="5d1a1-139">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="5d1a1-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5d1a1-140">请求</span><span class="sxs-lookup"><span data-stu-id="5d1a1-140">Request</span></span>
<span data-ttu-id="5d1a1-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5d1a1-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5d1a1-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="5d1a1-142">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "chartcollection_itemat",
  "idempotent": true,
  "@type": "requestBodyResourceFor.chartcollection_itemat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/itemAt
Content-type: application/json
Content-length: 20

{
  "index": 8
}
```
# <a name="javascript"></a>[<span data-ttu-id="5d1a1-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5d1a1-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chartcollection-itemat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5d1a1-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5d1a1-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chartcollection-itemat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5d1a1-145">响应</span><span class="sxs-lookup"><span data-stu-id="5d1a1-145">Response</span></span>
<span data-ttu-id="5d1a1-146">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5d1a1-146">Here is an example of the response.</span></span> <span data-ttu-id="5d1a1-147">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5d1a1-147">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChart"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

