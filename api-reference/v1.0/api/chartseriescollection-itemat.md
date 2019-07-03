---
title: 'ChartSeriesCollection: ItemAt'
description: 根据其在集合中的位置检索系列
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: c82d95a1e373fb068636ded4433019b8de9dd57d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35443152"
---
# <a name="chartseriescollection-itemat"></a><span data-ttu-id="b12fd-103">ChartSeriesCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="b12fd-103">ChartSeriesCollection: ItemAt</span></span>

<span data-ttu-id="b12fd-104">根据其在集合中的位置检索系列</span><span class="sxs-lookup"><span data-stu-id="b12fd-104">Retrieves a series based on its position in the collection</span></span>
## <a name="permissions"></a><span data-ttu-id="b12fd-105">权限</span><span class="sxs-lookup"><span data-stu-id="b12fd-105">Permissions</span></span>
<span data-ttu-id="b12fd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b12fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b12fd-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b12fd-108">Permission type</span></span>      | <span data-ttu-id="b12fd-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b12fd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b12fd-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b12fd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b12fd-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b12fd-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b12fd-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b12fd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b12fd-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="b12fd-113">Not supported.</span></span>    |
|<span data-ttu-id="b12fd-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="b12fd-114">Application</span></span> | <span data-ttu-id="b12fd-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b12fd-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b12fd-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b12fd-116">HTTP request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b12fd-117">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="b12fd-117">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/series/itemAt

```
## <a name="request-headers"></a><span data-ttu-id="b12fd-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b12fd-118">Request headers</span></span>
| <span data-ttu-id="b12fd-119">名称</span><span class="sxs-lookup"><span data-stu-id="b12fd-119">Name</span></span>       | <span data-ttu-id="b12fd-120">说明</span><span class="sxs-lookup"><span data-stu-id="b12fd-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b12fd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b12fd-121">Authorization</span></span>  | <span data-ttu-id="b12fd-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b12fd-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b12fd-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b12fd-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="b12fd-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="b12fd-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b12fd-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b12fd-127">Request body</span></span>
<span data-ttu-id="b12fd-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="b12fd-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b12fd-129">参数</span><span class="sxs-lookup"><span data-stu-id="b12fd-129">Parameter</span></span>    | <span data-ttu-id="b12fd-130">类型</span><span class="sxs-lookup"><span data-stu-id="b12fd-130">Type</span></span>   |<span data-ttu-id="b12fd-131">说明</span><span class="sxs-lookup"><span data-stu-id="b12fd-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b12fd-132">index</span><span class="sxs-lookup"><span data-stu-id="b12fd-132">index</span></span>|<span data-ttu-id="b12fd-133">Int32</span><span class="sxs-lookup"><span data-stu-id="b12fd-133">Int32</span></span>|<span data-ttu-id="b12fd-p104">要检索的对象的索引值。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="b12fd-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="b12fd-136">响应</span><span class="sxs-lookup"><span data-stu-id="b12fd-136">Response</span></span>

<span data-ttu-id="b12fd-137">如果成功, 此方法在`200 OK`响应正文中返回响应代码和[WorkbookChartSeries](../resources/chartseries.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b12fd-137">If successful, this method returns `200 OK` response code and [WorkbookChartSeries](../resources/chartseries.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b12fd-138">示例</span><span class="sxs-lookup"><span data-stu-id="b12fd-138">Example</span></span>
<span data-ttu-id="b12fd-139">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="b12fd-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b12fd-140">请求</span><span class="sxs-lookup"><span data-stu-id="b12fd-140">Request</span></span>
<span data-ttu-id="b12fd-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b12fd-141">Here is an example of the request.</span></span>
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b12fd-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="b12fd-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chartseriescollection-itemat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b12fd-143">目标-C</span><span class="sxs-lookup"><span data-stu-id="b12fd-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chartseriescollection-itemat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b12fd-144">响应</span><span class="sxs-lookup"><span data-stu-id="b12fd-144">Response</span></span>
<span data-ttu-id="b12fd-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b12fd-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
