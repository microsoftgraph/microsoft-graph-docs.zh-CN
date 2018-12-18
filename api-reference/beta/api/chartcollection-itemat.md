---
title: 'ChartCollection: ItemAt'
description: 根据其在集合中的位置获取图表。
author: lumine2008
ms.openlocfilehash: 6490958908e7f6093e2d307764dd422026205f46
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303736"
---
# <a name="chartcollection-itemat"></a><span data-ttu-id="75923-103">ChartCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="75923-103">ChartCollection: ItemAt</span></span>

> <span data-ttu-id="75923-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="75923-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="75923-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="75923-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="75923-106">根据其在集合中的位置获取图表。</span><span class="sxs-lookup"><span data-stu-id="75923-106">Gets a chart based on its position in the collection.</span></span>
## <a name="permissions"></a><span data-ttu-id="75923-107">权限</span><span class="sxs-lookup"><span data-stu-id="75923-107">Permissions</span></span>
<span data-ttu-id="75923-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="75923-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75923-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="75923-110">Permission type</span></span>      | <span data-ttu-id="75923-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="75923-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="75923-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="75923-112">Delegated (work or school account)</span></span> | <span data-ttu-id="75923-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="75923-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="75923-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="75923-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75923-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="75923-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="75923-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="75923-116">Application</span></span> | <span data-ttu-id="75923-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="75923-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="75923-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="75923-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="75923-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="75923-119">Request headers</span></span>
| <span data-ttu-id="75923-120">Name</span><span class="sxs-lookup"><span data-stu-id="75923-120">Name</span></span>       | <span data-ttu-id="75923-121">说明</span><span class="sxs-lookup"><span data-stu-id="75923-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="75923-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="75923-122">Authorization</span></span>  | <span data-ttu-id="75923-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="75923-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="75923-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="75923-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="75923-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="75923-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="75923-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="75923-128">Request body</span></span>
<span data-ttu-id="75923-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="75923-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="75923-130">参数</span><span class="sxs-lookup"><span data-stu-id="75923-130">Parameter</span></span>    | <span data-ttu-id="75923-131">Type</span><span class="sxs-lookup"><span data-stu-id="75923-131">Type</span></span>   |<span data-ttu-id="75923-132">说明</span><span class="sxs-lookup"><span data-stu-id="75923-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="75923-133">index</span><span class="sxs-lookup"><span data-stu-id="75923-133">index</span></span>|<span data-ttu-id="75923-134">number</span><span class="sxs-lookup"><span data-stu-id="75923-134">number</span></span>|<span data-ttu-id="75923-p105">要检索的对象的索引值。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="75923-p105">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="75923-137">响应</span><span class="sxs-lookup"><span data-stu-id="75923-137">Response</span></span>

<span data-ttu-id="75923-138">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Chart](../resources/chart.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="75923-138">If successful, this method returns `200 OK` response code and [Chart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75923-139">示例</span><span class="sxs-lookup"><span data-stu-id="75923-139">Example</span></span>
<span data-ttu-id="75923-140">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="75923-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="75923-141">请求</span><span class="sxs-lookup"><span data-stu-id="75923-141">Request</span></span>
<span data-ttu-id="75923-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="75923-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartcollection_itemat"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/ItemAt
Content-type: application/json
Content-length: 20

{
  "index": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="75923-143">响应</span><span class="sxs-lookup"><span data-stu-id="75923-143">Response</span></span>
<span data-ttu-id="75923-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="75923-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chart"
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
  "tocPath": ""
}-->