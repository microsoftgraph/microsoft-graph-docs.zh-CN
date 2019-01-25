---
title: 更新 chartaxistitle
description: 更新 chartaxistitle 对象的属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 6f8e1ba265246678bb930c1135fbf465147c1c7b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522614"
---
# <a name="update-chartaxistitle"></a><span data-ttu-id="7e554-103">更新 chartaxistitle</span><span class="sxs-lookup"><span data-stu-id="7e554-103">Update chartaxistitle</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e554-104">更新 chartaxistitle 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7e554-104">Update the properties of chartaxistitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7e554-105">权限</span><span class="sxs-lookup"><span data-stu-id="7e554-105">Permissions</span></span>
<span data-ttu-id="7e554-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7e554-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e554-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="7e554-108">Permission type</span></span>      | <span data-ttu-id="7e554-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7e554-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7e554-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7e554-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7e554-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7e554-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7e554-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7e554-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e554-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7e554-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7e554-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="7e554-114">Application</span></span> | <span data-ttu-id="7e554-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7e554-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7e554-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7e554-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/title
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/title
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/categoryaxis/title
```
## <a name="optional-request-headers"></a><span data-ttu-id="7e554-117">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="7e554-117">Optional request headers</span></span>
| <span data-ttu-id="7e554-118">名称</span><span class="sxs-lookup"><span data-stu-id="7e554-118">Name</span></span>       | <span data-ttu-id="7e554-119">说明</span><span class="sxs-lookup"><span data-stu-id="7e554-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="7e554-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e554-120">Authorization</span></span>  | <span data-ttu-id="7e554-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7e554-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7e554-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7e554-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="7e554-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="7e554-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e554-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="7e554-126">Request body</span></span>
<span data-ttu-id="7e554-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="7e554-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="7e554-130">属性</span><span class="sxs-lookup"><span data-stu-id="7e554-130">Property</span></span>     | <span data-ttu-id="7e554-131">类型</span><span class="sxs-lookup"><span data-stu-id="7e554-131">Type</span></span>   |<span data-ttu-id="7e554-132">说明</span><span class="sxs-lookup"><span data-stu-id="7e554-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7e554-133">text</span><span class="sxs-lookup"><span data-stu-id="7e554-133">text</span></span>|<span data-ttu-id="7e554-134">string</span><span class="sxs-lookup"><span data-stu-id="7e554-134">string</span></span>|<span data-ttu-id="7e554-135">表示坐标轴标题。</span><span class="sxs-lookup"><span data-stu-id="7e554-135">Represents the axis title.</span></span>|
|<span data-ttu-id="7e554-136">visible</span><span class="sxs-lookup"><span data-stu-id="7e554-136">visible</span></span>|<span data-ttu-id="7e554-137">布尔</span><span class="sxs-lookup"><span data-stu-id="7e554-137">boolean</span></span>|<span data-ttu-id="7e554-138">指定坐标轴标题可见性的布尔值。</span><span class="sxs-lookup"><span data-stu-id="7e554-138">A boolean that specifies the visibility of an axis title.</span></span>|

## <a name="response"></a><span data-ttu-id="7e554-139">响应</span><span class="sxs-lookup"><span data-stu-id="7e554-139">Response</span></span>

<span data-ttu-id="7e554-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [ChartAxisTitle](../resources/chartaxistitle.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7e554-140">If successful, this method returns a `200 OK` response code and updated [ChartAxisTitle](../resources/chartaxistitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7e554-141">示例</span><span class="sxs-lookup"><span data-stu-id="7e554-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7e554-142">请求</span><span class="sxs-lookup"><span data-stu-id="7e554-142">Request</span></span>
<span data-ttu-id="7e554-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7e554-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartaxistitle"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/title
Content-type: application/json
Content-length: 45

{
  "text": "text-value",
  "visible": true
}
```
##### <a name="response"></a><span data-ttu-id="7e554-144">响应</span><span class="sxs-lookup"><span data-stu-id="7e554-144">Response</span></span>
<span data-ttu-id="7e554-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7e554-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartAxisTitle"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "text": "text-value",
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update chartaxistitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chartaxistitle-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
