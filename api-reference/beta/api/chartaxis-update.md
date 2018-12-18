---
title: 更新 chartaxis
description: 更新 chartaxis 对象的属性。
author: lumine2008
ms.openlocfilehash: bc6bea839751641530a3c3945307db2a206b7725
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325485"
---
# <a name="update-chartaxis"></a><span data-ttu-id="30be4-103">更新 chartaxis</span><span class="sxs-lookup"><span data-stu-id="30be4-103">Update chartaxis</span></span>

> <span data-ttu-id="30be4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="30be4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="30be4-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="30be4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="30be4-106">更新 chartaxis 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="30be4-106">Update the properties of chartaxis object.</span></span>
## <a name="permissions"></a><span data-ttu-id="30be4-107">权限</span><span class="sxs-lookup"><span data-stu-id="30be4-107">Permissions</span></span>
<span data-ttu-id="30be4-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="30be4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30be4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="30be4-110">Permission type</span></span>      | <span data-ttu-id="30be4-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="30be4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="30be4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="30be4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="30be4-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="30be4-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="30be4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="30be4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30be4-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="30be4-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="30be4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="30be4-116">Application</span></span> | <span data-ttu-id="30be4-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="30be4-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="30be4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="30be4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/categoryaxis
```
## <a name="optional-request-headers"></a><span data-ttu-id="30be4-119">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="30be4-119">Optional request headers</span></span>
| <span data-ttu-id="30be4-120">Name</span><span class="sxs-lookup"><span data-stu-id="30be4-120">Name</span></span>       | <span data-ttu-id="30be4-121">说明</span><span class="sxs-lookup"><span data-stu-id="30be4-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="30be4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="30be4-122">Authorization</span></span>  | <span data-ttu-id="30be4-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="30be4-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="30be4-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="30be4-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="30be4-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="30be4-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="30be4-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="30be4-128">Request body</span></span>
<span data-ttu-id="30be4-p105">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="30be4-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="30be4-132">属性</span><span class="sxs-lookup"><span data-stu-id="30be4-132">Property</span></span>     | <span data-ttu-id="30be4-133">类型</span><span class="sxs-lookup"><span data-stu-id="30be4-133">Type</span></span>   |<span data-ttu-id="30be4-134">说明</span><span class="sxs-lookup"><span data-stu-id="30be4-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="30be4-135">majorUnit</span><span class="sxs-lookup"><span data-stu-id="30be4-135">majorUnit</span></span>|<span data-ttu-id="30be4-136">对象</span><span class="sxs-lookup"><span data-stu-id="30be4-136">object</span></span>|<span data-ttu-id="30be4-p106">表示两个主要刻度标记之间的间隔。可以设置为数字值或空字符串。返回的值始终为数字。</span><span class="sxs-lookup"><span data-stu-id="30be4-p106">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="30be4-140">maximum</span><span class="sxs-lookup"><span data-stu-id="30be4-140">maximum</span></span>|<span data-ttu-id="30be4-141">对象</span><span class="sxs-lookup"><span data-stu-id="30be4-141">object</span></span>|<span data-ttu-id="30be4-p107">表示数值轴上的最大值。可以设置为数字值或空字符串（对于自动坐标轴值）。返回的值始终为数字。</span><span class="sxs-lookup"><span data-stu-id="30be4-p107">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="30be4-145">minimum</span><span class="sxs-lookup"><span data-stu-id="30be4-145">minimum</span></span>|<span data-ttu-id="30be4-146">对象</span><span class="sxs-lookup"><span data-stu-id="30be4-146">object</span></span>|<span data-ttu-id="30be4-p108">表示数值轴上的最小值。可以设置为数字值或空字符串（对于自动坐标轴值）。返回的值始终为数字。</span><span class="sxs-lookup"><span data-stu-id="30be4-p108">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="30be4-150">minorUnit</span><span class="sxs-lookup"><span data-stu-id="30be4-150">minorUnit</span></span>|<span data-ttu-id="30be4-151">对象</span><span class="sxs-lookup"><span data-stu-id="30be4-151">object</span></span>|<span data-ttu-id="30be4-p109">表示两个次要刻度标记之间的间隔。可以设置为数字值或空字符串（对于自动坐标轴值）。返回的值始终为数字。</span><span class="sxs-lookup"><span data-stu-id="30be4-p109">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="response"></a><span data-ttu-id="30be4-155">响应</span><span class="sxs-lookup"><span data-stu-id="30be4-155">Response</span></span>

<span data-ttu-id="30be4-156">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [ChartAxis](../resources/chartaxis.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="30be4-156">If successful, this method returns a `200 OK` response code and updated [ChartAxis](../resources/chartaxis.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="30be4-157">示例</span><span class="sxs-lookup"><span data-stu-id="30be4-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="30be4-158">请求</span><span class="sxs-lookup"><span data-stu-id="30be4-158">Request</span></span>
<span data-ttu-id="30be4-159">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="30be4-159">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartaxis"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis
Content-type: application/json
Content-length: 64

{
  "majorUnit": {
  },
  "maximum": {
  },
  "minimum": {
  }
}
```
##### <a name="response"></a><span data-ttu-id="30be4-160">响应</span><span class="sxs-lookup"><span data-stu-id="30be4-160">Response</span></span>
<span data-ttu-id="30be4-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="30be4-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartaxis"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 64

{
  "majorUnit": {
  },
  "maximum": {
  },
  "minimum": {
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartaxis",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->