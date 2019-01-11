---
title: 更新 chartlineformat
description: 更新 chartlineformat 对象的属性。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: c47ec9159ba6592de2a57c50ff1a22bad0b52e3b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892377"
---
# <a name="update-chartlineformat"></a><span data-ttu-id="8e92d-103">更新 chartlineformat</span><span class="sxs-lookup"><span data-stu-id="8e92d-103">Update chartlineformat</span></span>

> <span data-ttu-id="8e92d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8e92d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8e92d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8e92d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8e92d-106">更新 chartlineformat 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8e92d-106">Update the properties of chartlineformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8e92d-107">权限</span><span class="sxs-lookup"><span data-stu-id="8e92d-107">Permissions</span></span>
<span data-ttu-id="8e92d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8e92d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e92d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8e92d-110">Permission type</span></span>      | <span data-ttu-id="8e92d-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8e92d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e92d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8e92d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8e92d-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8e92d-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8e92d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8e92d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e92d-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8e92d-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8e92d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8e92d-116">Application</span></span> | <span data-ttu-id="8e92d-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="8e92d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8e92d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8e92d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/format/line
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/categoryaxis/format/line
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/majorgridlines/format/line
```
## <a name="optional-request-headers"></a><span data-ttu-id="8e92d-119">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="8e92d-119">Optional request headers</span></span>
| <span data-ttu-id="8e92d-120">名称</span><span class="sxs-lookup"><span data-stu-id="8e92d-120">Name</span></span>       | <span data-ttu-id="8e92d-121">说明</span><span class="sxs-lookup"><span data-stu-id="8e92d-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="8e92d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e92d-122">Authorization</span></span>  | <span data-ttu-id="8e92d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8e92d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8e92d-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8e92d-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="8e92d-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="8e92d-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e92d-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="8e92d-128">Request body</span></span>
<span data-ttu-id="8e92d-p105">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="8e92d-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8e92d-132">属性</span><span class="sxs-lookup"><span data-stu-id="8e92d-132">Property</span></span>     | <span data-ttu-id="8e92d-133">类型</span><span class="sxs-lookup"><span data-stu-id="8e92d-133">Type</span></span>   |<span data-ttu-id="8e92d-134">说明</span><span class="sxs-lookup"><span data-stu-id="8e92d-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8e92d-135">color</span><span class="sxs-lookup"><span data-stu-id="8e92d-135">color</span></span>|<span data-ttu-id="8e92d-136">string</span><span class="sxs-lookup"><span data-stu-id="8e92d-136">string</span></span>|<span data-ttu-id="8e92d-137">表示图表中的线条颜色的 HTML 颜色代码。</span><span class="sxs-lookup"><span data-stu-id="8e92d-137">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="response"></a><span data-ttu-id="8e92d-138">响应</span><span class="sxs-lookup"><span data-stu-id="8e92d-138">Response</span></span>

<span data-ttu-id="8e92d-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [ChartLineFormat](../resources/chartlineformat.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8e92d-139">If successful, this method returns a `200 OK` response code and updated [ChartLineFormat](../resources/chartlineformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8e92d-140">示例</span><span class="sxs-lookup"><span data-stu-id="8e92d-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8e92d-141">请求</span><span class="sxs-lookup"><span data-stu-id="8e92d-141">Request</span></span>
<span data-ttu-id="8e92d-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8e92d-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartlineformat"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/format/line
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```
##### <a name="response"></a><span data-ttu-id="8e92d-143">响应</span><span class="sxs-lookup"><span data-stu-id="8e92d-143">Response</span></span>
<span data-ttu-id="8e92d-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8e92d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartLineFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartlineformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
