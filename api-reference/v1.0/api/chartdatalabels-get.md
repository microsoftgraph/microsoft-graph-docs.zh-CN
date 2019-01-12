---
title: 获取 ChartDataLabels
description: 检索 chartdatalabels 对象的属性和关系。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 336fef8e1f237e1aa54677dc96a055126335d7e2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27974369"
---
# <a name="get-chartdatalabels"></a><span data-ttu-id="058ce-103">获取 ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="058ce-103">Get ChartDataLabels</span></span>

<span data-ttu-id="058ce-104">检索 chartdatalabels 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="058ce-104">Retrieve the properties and relationships of chartdatalabels object.</span></span>
## <a name="permissions"></a><span data-ttu-id="058ce-105">权限</span><span class="sxs-lookup"><span data-stu-id="058ce-105">Permissions</span></span>
<span data-ttu-id="058ce-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="058ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="058ce-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="058ce-108">Permission type</span></span>      | <span data-ttu-id="058ce-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="058ce-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="058ce-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="058ce-110">Delegated (work or school account)</span></span> | <span data-ttu-id="058ce-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="058ce-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="058ce-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="058ce-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="058ce-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="058ce-113">Not supported.</span></span>    |
|<span data-ttu-id="058ce-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="058ce-114">Application</span></span> | <span data-ttu-id="058ce-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="058ce-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="058ce-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="058ce-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/dataLabels
```
## <a name="optional-query-parameters"></a><span data-ttu-id="058ce-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="058ce-117">Optional query parameters</span></span>
<span data-ttu-id="058ce-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="058ce-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="058ce-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="058ce-119">Request headers</span></span>
| <span data-ttu-id="058ce-120">名称</span><span class="sxs-lookup"><span data-stu-id="058ce-120">Name</span></span>      |<span data-ttu-id="058ce-121">说明</span><span class="sxs-lookup"><span data-stu-id="058ce-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="058ce-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="058ce-122">Authorization</span></span>  | <span data-ttu-id="058ce-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="058ce-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="058ce-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="058ce-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="058ce-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="058ce-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="058ce-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="058ce-128">Request body</span></span>
<span data-ttu-id="058ce-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="058ce-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="058ce-130">响应</span><span class="sxs-lookup"><span data-stu-id="058ce-130">Response</span></span>

<span data-ttu-id="058ce-131">如果成功，此方法返回`200 OK`响应代码和[WorkbookChartDataLabels](../resources/chartdatalabels.md)响应正文中的对象。</span><span class="sxs-lookup"><span data-stu-id="058ce-131">If successful, this method returns a `200 OK` response code and [WorkbookChartDataLabels](../resources/chartdatalabels.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="058ce-132">示例</span><span class="sxs-lookup"><span data-stu-id="058ce-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="058ce-133">请求</span><span class="sxs-lookup"><span data-stu-id="058ce-133">Request</span></span>
<span data-ttu-id="058ce-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="058ce-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_chartdatalabels"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/dataLabels
```
##### <a name="response"></a><span data-ttu-id="058ce-135">响应</span><span class="sxs-lookup"><span data-stu-id="058ce-135">Response</span></span>
<span data-ttu-id="058ce-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="058ce-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartDataLabels"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 134

{
  "position": "position-value",
  "showValue": true,
  "showSeriesName": true,
  "showCategoryName": true,
  "showLegendKey": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get ChartDataLabels",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
