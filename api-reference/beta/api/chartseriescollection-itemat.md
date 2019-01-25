---
title: 'ChartSeriesCollection: ItemAt'
description: 根据其在集合中的位置检索系列
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 063a5a605908693e5b189c92865eaec2c0dba1ba
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518266"
---
# <a name="chartseriescollection-itemat"></a><span data-ttu-id="73c35-103">ChartSeriesCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="73c35-103">ChartSeriesCollection: ItemAt</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73c35-104">根据其在集合中的位置检索系列</span><span class="sxs-lookup"><span data-stu-id="73c35-104">Retrieves a series based on its position in the collection</span></span>
## <a name="permissions"></a><span data-ttu-id="73c35-105">权限</span><span class="sxs-lookup"><span data-stu-id="73c35-105">Permissions</span></span>
<span data-ttu-id="73c35-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="73c35-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73c35-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="73c35-108">Permission type</span></span>      | <span data-ttu-id="73c35-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="73c35-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73c35-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="73c35-110">Delegated (work or school account)</span></span> | <span data-ttu-id="73c35-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73c35-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="73c35-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="73c35-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73c35-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73c35-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="73c35-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="73c35-114">Application</span></span> | <span data-ttu-id="73c35-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="73c35-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="73c35-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="73c35-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/series/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="73c35-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="73c35-117">Request headers</span></span>
| <span data-ttu-id="73c35-118">名称</span><span class="sxs-lookup"><span data-stu-id="73c35-118">Name</span></span>       | <span data-ttu-id="73c35-119">说明</span><span class="sxs-lookup"><span data-stu-id="73c35-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="73c35-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="73c35-120">Authorization</span></span>  | <span data-ttu-id="73c35-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="73c35-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="73c35-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="73c35-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="73c35-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="73c35-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="73c35-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="73c35-126">Request body</span></span>
<span data-ttu-id="73c35-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="73c35-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="73c35-128">参数</span><span class="sxs-lookup"><span data-stu-id="73c35-128">Parameter</span></span>    | <span data-ttu-id="73c35-129">类型</span><span class="sxs-lookup"><span data-stu-id="73c35-129">Type</span></span>   |<span data-ttu-id="73c35-130">说明</span><span class="sxs-lookup"><span data-stu-id="73c35-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="73c35-131">index</span><span class="sxs-lookup"><span data-stu-id="73c35-131">index</span></span>|<span data-ttu-id="73c35-132">number</span><span class="sxs-lookup"><span data-stu-id="73c35-132">number</span></span>|<span data-ttu-id="73c35-p104">要检索的对象的索引值。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="73c35-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="73c35-135">响应</span><span class="sxs-lookup"><span data-stu-id="73c35-135">Response</span></span>

<span data-ttu-id="73c35-136">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [ChartSeries](../resources/chartseries.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="73c35-136">If successful, this method returns `200 OK` response code and [ChartSeries](../resources/chartseries.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73c35-137">示例</span><span class="sxs-lookup"><span data-stu-id="73c35-137">Example</span></span>
<span data-ttu-id="73c35-138">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="73c35-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="73c35-139">请求</span><span class="sxs-lookup"><span data-stu-id="73c35-139">Request</span></span>
<span data-ttu-id="73c35-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="73c35-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartseriescollection_itemat"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/series/ItemAt
Content-type: application/json
Content-length: 20

{
  "index": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="73c35-141">响应</span><span class="sxs-lookup"><span data-stu-id="73c35-141">Response</span></span>
<span data-ttu-id="73c35-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="73c35-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartSeries"
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
<!--
{
  "type": "#page.annotation",
  "description": "ChartSeriesCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chartseriescollection-itemat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
