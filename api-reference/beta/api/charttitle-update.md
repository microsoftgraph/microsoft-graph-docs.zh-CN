---
title: 更新 charttitle
description: 更新 charttitle 对象的属性。
author: lumine2008
ms.openlocfilehash: 2a3dd005b7932325685e9efa23acf1accd9320f8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353366"
---
# <a name="update-charttitle"></a><span data-ttu-id="de3b6-103">更新 charttitle</span><span class="sxs-lookup"><span data-stu-id="de3b6-103">Update charttitle</span></span>

> <span data-ttu-id="de3b6-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="de3b6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="de3b6-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="de3b6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="de3b6-106">更新 charttitle 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="de3b6-106">Update the properties of charttitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="de3b6-107">权限</span><span class="sxs-lookup"><span data-stu-id="de3b6-107">Permissions</span></span>
<span data-ttu-id="de3b6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="de3b6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de3b6-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="de3b6-110">Permission type</span></span>      | <span data-ttu-id="de3b6-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="de3b6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="de3b6-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="de3b6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="de3b6-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="de3b6-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="de3b6-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="de3b6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de3b6-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="de3b6-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="de3b6-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="de3b6-116">Application</span></span> | <span data-ttu-id="de3b6-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="de3b6-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="de3b6-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="de3b6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/title
```
## <a name="optional-request-headers"></a><span data-ttu-id="de3b6-119">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="de3b6-119">Optional request headers</span></span>
| <span data-ttu-id="de3b6-120">Name</span><span class="sxs-lookup"><span data-stu-id="de3b6-120">Name</span></span>       | <span data-ttu-id="de3b6-121">说明</span><span class="sxs-lookup"><span data-stu-id="de3b6-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="de3b6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="de3b6-122">Authorization</span></span>  | <span data-ttu-id="de3b6-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="de3b6-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="de3b6-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="de3b6-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="de3b6-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="de3b6-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="de3b6-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="de3b6-128">Request body</span></span>
<span data-ttu-id="de3b6-p105">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="de3b6-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="de3b6-132">属性</span><span class="sxs-lookup"><span data-stu-id="de3b6-132">Property</span></span>     | <span data-ttu-id="de3b6-133">类型</span><span class="sxs-lookup"><span data-stu-id="de3b6-133">Type</span></span>   |<span data-ttu-id="de3b6-134">说明</span><span class="sxs-lookup"><span data-stu-id="de3b6-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="de3b6-135">overlay</span><span class="sxs-lookup"><span data-stu-id="de3b6-135">overlay</span></span>|<span data-ttu-id="de3b6-136">boolean</span><span class="sxs-lookup"><span data-stu-id="de3b6-136">boolean</span></span>|<span data-ttu-id="de3b6-137">表示图表标题是否将叠加在图表上的布尔值。</span><span class="sxs-lookup"><span data-stu-id="de3b6-137">Boolean value representing if the chart title will overlay the chart or not.</span></span>|
|<span data-ttu-id="de3b6-138">text</span><span class="sxs-lookup"><span data-stu-id="de3b6-138">text</span></span>|<span data-ttu-id="de3b6-139">string</span><span class="sxs-lookup"><span data-stu-id="de3b6-139">string</span></span>|<span data-ttu-id="de3b6-140">表示图表的标题文本。</span><span class="sxs-lookup"><span data-stu-id="de3b6-140">Represents the title text of a chart.</span></span>|
|<span data-ttu-id="de3b6-141">visible</span><span class="sxs-lookup"><span data-stu-id="de3b6-141">visible</span></span>|<span data-ttu-id="de3b6-142">boolean</span><span class="sxs-lookup"><span data-stu-id="de3b6-142">boolean</span></span>|<span data-ttu-id="de3b6-143">表示 chart title 对象的可见性的布尔值。</span><span class="sxs-lookup"><span data-stu-id="de3b6-143">A boolean value the represents the visibility of a chart title object.</span></span>|

## <a name="response"></a><span data-ttu-id="de3b6-144">响应</span><span class="sxs-lookup"><span data-stu-id="de3b6-144">Response</span></span>

<span data-ttu-id="de3b6-145">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [ChartTitle](../resources/charttitle.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="de3b6-145">If successful, this method returns a `200 OK` response code and updated [ChartTitle](../resources/charttitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="de3b6-146">示例</span><span class="sxs-lookup"><span data-stu-id="de3b6-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="de3b6-147">请求</span><span class="sxs-lookup"><span data-stu-id="de3b6-147">Request</span></span>
<span data-ttu-id="de3b6-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="de3b6-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_charttitle"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/title
Content-type: application/json
Content-length: 64

{
  "overlay": true,
  "text": "text-value",
  "visible": true
}
```
##### <a name="response"></a><span data-ttu-id="de3b6-149">响应</span><span class="sxs-lookup"><span data-stu-id="de3b6-149">Response</span></span>
<span data-ttu-id="de3b6-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="de3b6-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartTitle"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 64

{
  "overlay": true,
  "text": "text-value",
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update charttitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->