---
title: 更新 chartfont
description: 更新 chartfont 对象的属性。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 6030bd9a5ab39f56ecb84da4f60457b4c8d8ba53
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864951"
---
# <a name="update-chartfont"></a><span data-ttu-id="026e1-103">更新 chartfont</span><span class="sxs-lookup"><span data-stu-id="026e1-103">Update chartfont</span></span>

> <span data-ttu-id="026e1-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="026e1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="026e1-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="026e1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="026e1-106">更新 chartfont 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="026e1-106">Update the properties of chartfont object.</span></span>
## <a name="permissions"></a><span data-ttu-id="026e1-107">权限</span><span class="sxs-lookup"><span data-stu-id="026e1-107">Permissions</span></span>
<span data-ttu-id="026e1-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="026e1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="026e1-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="026e1-110">Permission type</span></span>      | <span data-ttu-id="026e1-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="026e1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="026e1-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="026e1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="026e1-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="026e1-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="026e1-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="026e1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="026e1-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="026e1-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="026e1-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="026e1-116">Application</span></span> | <span data-ttu-id="026e1-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="026e1-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="026e1-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="026e1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/format/font
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/format/font
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/categoryaxis/format/font
```
## <a name="optional-request-headers"></a><span data-ttu-id="026e1-119">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="026e1-119">Optional request headers</span></span>
| <span data-ttu-id="026e1-120">名称</span><span class="sxs-lookup"><span data-stu-id="026e1-120">Name</span></span>       | <span data-ttu-id="026e1-121">说明</span><span class="sxs-lookup"><span data-stu-id="026e1-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="026e1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="026e1-122">Authorization</span></span>  | <span data-ttu-id="026e1-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="026e1-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="026e1-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="026e1-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="026e1-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="026e1-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="026e1-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="026e1-128">Request body</span></span>
<span data-ttu-id="026e1-p105">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="026e1-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="026e1-132">属性</span><span class="sxs-lookup"><span data-stu-id="026e1-132">Property</span></span>     | <span data-ttu-id="026e1-133">类型</span><span class="sxs-lookup"><span data-stu-id="026e1-133">Type</span></span>   |<span data-ttu-id="026e1-134">说明</span><span class="sxs-lookup"><span data-stu-id="026e1-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="026e1-135">bold</span><span class="sxs-lookup"><span data-stu-id="026e1-135">bold</span></span>|<span data-ttu-id="026e1-136">boolean</span><span class="sxs-lookup"><span data-stu-id="026e1-136">boolean</span></span>|<span data-ttu-id="026e1-137">表示字体的加粗状态。</span><span class="sxs-lookup"><span data-stu-id="026e1-137">Represents the bold status of font.</span></span>|
|<span data-ttu-id="026e1-138">color</span><span class="sxs-lookup"><span data-stu-id="026e1-138">color</span></span>|<span data-ttu-id="026e1-139">string</span><span class="sxs-lookup"><span data-stu-id="026e1-139">string</span></span>|<span data-ttu-id="026e1-p106">文本颜色的 HTML 颜色代码表示。例如，#FF0000 表示红色。</span><span class="sxs-lookup"><span data-stu-id="026e1-p106">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="026e1-143">italic</span><span class="sxs-lookup"><span data-stu-id="026e1-143">italic</span></span>|<span data-ttu-id="026e1-144">boolean</span><span class="sxs-lookup"><span data-stu-id="026e1-144">boolean</span></span>|<span data-ttu-id="026e1-145">表示字体的斜体状态。</span><span class="sxs-lookup"><span data-stu-id="026e1-145">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="026e1-146">name</span><span class="sxs-lookup"><span data-stu-id="026e1-146">name</span></span>|<span data-ttu-id="026e1-147">string</span><span class="sxs-lookup"><span data-stu-id="026e1-147">string</span></span>|<span data-ttu-id="026e1-148">字体名称（例如"Calibri"）</span><span class="sxs-lookup"><span data-stu-id="026e1-148">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="026e1-149">大小</span><span class="sxs-lookup"><span data-stu-id="026e1-149">size</span></span>|<span data-ttu-id="026e1-150">double</span><span class="sxs-lookup"><span data-stu-id="026e1-150">double</span></span>|<span data-ttu-id="026e1-151">字体大小（例如 11）</span><span class="sxs-lookup"><span data-stu-id="026e1-151">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="026e1-152">underline</span><span class="sxs-lookup"><span data-stu-id="026e1-152">underline</span></span>|<span data-ttu-id="026e1-153">string</span><span class="sxs-lookup"><span data-stu-id="026e1-153">string</span></span>|<span data-ttu-id="026e1-p107">应用于字体的下划线类型。可能的值是：`None`、`Single`。</span><span class="sxs-lookup"><span data-stu-id="026e1-p107">Type of underline applied to the font. Possible values are: `None`, `Single`.</span></span>|

## <a name="response"></a><span data-ttu-id="026e1-156">响应</span><span class="sxs-lookup"><span data-stu-id="026e1-156">Response</span></span>

<span data-ttu-id="026e1-157">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [ChartFont](../resources/chartfont.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="026e1-157">If successful, this method returns a `200 OK` response code and updated [ChartFont](../resources/chartfont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="026e1-158">示例</span><span class="sxs-lookup"><span data-stu-id="026e1-158">Example</span></span>
##### <a name="request"></a><span data-ttu-id="026e1-159">请求</span><span class="sxs-lookup"><span data-stu-id="026e1-159">Request</span></span>
<span data-ttu-id="026e1-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="026e1-160">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartfont"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis/format/font
Content-type: application/json
Content-length: 134

{
  "bold": true,
  "color": "color-value",
  "italic": true,
  "name": "name-value",
  "size": 99,
  "underline": "underline-value"
}
```
##### <a name="response"></a><span data-ttu-id="026e1-161">响应</span><span class="sxs-lookup"><span data-stu-id="026e1-161">Response</span></span>
<span data-ttu-id="026e1-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="026e1-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartFont"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 134

{
  "bold": true,
  "color": "color-value",
  "italic": true,
  "name": "name-value",
  "size": 99,
  "underline": "underline-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartfont",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
