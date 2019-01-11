---
title: 更新 chartseries
description: 更新 chartseries 对象的属性。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 1772265a833d60cc20fdd55e2b6d1755687bd1ca
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823728"
---
# <a name="update-chartseries"></a><span data-ttu-id="86fee-103">更新 chartseries</span><span class="sxs-lookup"><span data-stu-id="86fee-103">Update chartseries</span></span>

<span data-ttu-id="86fee-104">更新 chartseries 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="86fee-104">Update the properties of chartseries object.</span></span>
## <a name="permissions"></a><span data-ttu-id="86fee-105">权限</span><span class="sxs-lookup"><span data-stu-id="86fee-105">Permissions</span></span>
<span data-ttu-id="86fee-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="86fee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86fee-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="86fee-108">Permission type</span></span>      | <span data-ttu-id="86fee-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="86fee-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="86fee-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="86fee-110">Delegated (work or school account)</span></span> | <span data-ttu-id="86fee-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="86fee-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="86fee-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="86fee-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86fee-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="86fee-113">Not supported.</span></span>    |
|<span data-ttu-id="86fee-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="86fee-114">Application</span></span> | <span data-ttu-id="86fee-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="86fee-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="86fee-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="86fee-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/series/{series-id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="86fee-117">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="86fee-117">Optional request headers</span></span>
| <span data-ttu-id="86fee-118">名称</span><span class="sxs-lookup"><span data-stu-id="86fee-118">Name</span></span>       | <span data-ttu-id="86fee-119">说明</span><span class="sxs-lookup"><span data-stu-id="86fee-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="86fee-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="86fee-120">Authorization</span></span>  | <span data-ttu-id="86fee-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="86fee-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="86fee-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="86fee-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="86fee-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="86fee-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="86fee-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="86fee-126">Request body</span></span>
<span data-ttu-id="86fee-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="86fee-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="86fee-130">属性</span><span class="sxs-lookup"><span data-stu-id="86fee-130">Property</span></span>     | <span data-ttu-id="86fee-131">类型</span><span class="sxs-lookup"><span data-stu-id="86fee-131">Type</span></span>   |<span data-ttu-id="86fee-132">说明</span><span class="sxs-lookup"><span data-stu-id="86fee-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="86fee-133">name</span><span class="sxs-lookup"><span data-stu-id="86fee-133">name</span></span>|<span data-ttu-id="86fee-134">string</span><span class="sxs-lookup"><span data-stu-id="86fee-134">string</span></span>|<span data-ttu-id="86fee-135">表示图表中某个系列的名称。</span><span class="sxs-lookup"><span data-stu-id="86fee-135">Represents the name of a series in a chart.</span></span>|

## <a name="response"></a><span data-ttu-id="86fee-136">响应</span><span class="sxs-lookup"><span data-stu-id="86fee-136">Response</span></span>

<span data-ttu-id="86fee-137">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[WorkbookChartSeries](../resources/chartseries.md)对象。</span><span class="sxs-lookup"><span data-stu-id="86fee-137">If successful, this method returns a `200 OK` response code and updated [WorkbookChartSeries](../resources/chartseries.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="86fee-138">示例</span><span class="sxs-lookup"><span data-stu-id="86fee-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="86fee-139">请求</span><span class="sxs-lookup"><span data-stu-id="86fee-139">Request</span></span>
<span data-ttu-id="86fee-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="86fee-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartseries"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{series-id}
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```
##### <a name="response"></a><span data-ttu-id="86fee-141">响应</span><span class="sxs-lookup"><span data-stu-id="86fee-141">Response</span></span>
<span data-ttu-id="86fee-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="86fee-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Update chartseries",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
