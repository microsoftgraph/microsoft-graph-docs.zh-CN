---
title: 更新 rangefont
description: 更新 rangefont 对象的属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 13272be477c76b75e74b3159ae3baa122ef3633d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934021"
---
# <a name="update-rangefont"></a><span data-ttu-id="d475e-103">更新 rangefont</span><span class="sxs-lookup"><span data-stu-id="d475e-103">Update rangefont</span></span>

> <span data-ttu-id="d475e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d475e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d475e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d475e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d475e-106">更新 rangefont 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d475e-106">Update the properties of rangefont object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d475e-107">权限</span><span class="sxs-lookup"><span data-stu-id="d475e-107">Permissions</span></span>
<span data-ttu-id="d475e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d475e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d475e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d475e-110">Permission type</span></span>      | <span data-ttu-id="d475e-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d475e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d475e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d475e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d475e-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d475e-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d475e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d475e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d475e-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d475e-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d475e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d475e-116">Application</span></span> | <span data-ttu-id="d475e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d475e-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d475e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d475e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range/format/font
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format/font
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/font
```
## <a name="optional-request-headers"></a><span data-ttu-id="d475e-119">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="d475e-119">Optional request headers</span></span>
| <span data-ttu-id="d475e-120">名称</span><span class="sxs-lookup"><span data-stu-id="d475e-120">Name</span></span>       | <span data-ttu-id="d475e-121">说明</span><span class="sxs-lookup"><span data-stu-id="d475e-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d475e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d475e-122">Authorization</span></span>  | <span data-ttu-id="d475e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d475e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d475e-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d475e-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="d475e-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="d475e-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d475e-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="d475e-128">Request body</span></span>
<span data-ttu-id="d475e-p105">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="d475e-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d475e-132">属性</span><span class="sxs-lookup"><span data-stu-id="d475e-132">Property</span></span>     | <span data-ttu-id="d475e-133">类型</span><span class="sxs-lookup"><span data-stu-id="d475e-133">Type</span></span>   |<span data-ttu-id="d475e-134">说明</span><span class="sxs-lookup"><span data-stu-id="d475e-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d475e-135">bold</span><span class="sxs-lookup"><span data-stu-id="d475e-135">bold</span></span>|<span data-ttu-id="d475e-136">boolean</span><span class="sxs-lookup"><span data-stu-id="d475e-136">boolean</span></span>|<span data-ttu-id="d475e-137">表示字体的加粗状态。</span><span class="sxs-lookup"><span data-stu-id="d475e-137">Represents the bold status of font.</span></span>|
|<span data-ttu-id="d475e-138">color</span><span class="sxs-lookup"><span data-stu-id="d475e-138">color</span></span>|<span data-ttu-id="d475e-139">string</span><span class="sxs-lookup"><span data-stu-id="d475e-139">string</span></span>|<span data-ttu-id="d475e-p106">文本颜色的 HTML 颜色代码表示。例如，#FF0000 表示红色。</span><span class="sxs-lookup"><span data-stu-id="d475e-p106">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="d475e-143">italic</span><span class="sxs-lookup"><span data-stu-id="d475e-143">italic</span></span>|<span data-ttu-id="d475e-144">boolean</span><span class="sxs-lookup"><span data-stu-id="d475e-144">boolean</span></span>|<span data-ttu-id="d475e-145">表示字体的斜体状态。</span><span class="sxs-lookup"><span data-stu-id="d475e-145">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="d475e-146">name</span><span class="sxs-lookup"><span data-stu-id="d475e-146">name</span></span>|<span data-ttu-id="d475e-147">string</span><span class="sxs-lookup"><span data-stu-id="d475e-147">string</span></span>|<span data-ttu-id="d475e-148">字体名称（例如"Calibri"）</span><span class="sxs-lookup"><span data-stu-id="d475e-148">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="d475e-149">大小</span><span class="sxs-lookup"><span data-stu-id="d475e-149">size</span></span>|<span data-ttu-id="d475e-150">double</span><span class="sxs-lookup"><span data-stu-id="d475e-150">double</span></span>|<span data-ttu-id="d475e-151">字号</span><span class="sxs-lookup"><span data-stu-id="d475e-151">Font size.</span></span>|
|<span data-ttu-id="d475e-152">underline</span><span class="sxs-lookup"><span data-stu-id="d475e-152">underline</span></span>|<span data-ttu-id="d475e-153">string</span><span class="sxs-lookup"><span data-stu-id="d475e-153">string</span></span>|<span data-ttu-id="d475e-p107">应用于字体的下划线类型。可能的值是：`None`、`Single`、`Double`、`SingleAccountant`、`DoubleAccountant`。</span><span class="sxs-lookup"><span data-stu-id="d475e-p107">Type of underline applied to the font. Possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="response"></a><span data-ttu-id="d475e-156">响应</span><span class="sxs-lookup"><span data-stu-id="d475e-156">Response</span></span>

<span data-ttu-id="d475e-157">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [RangeFont](../resources/rangefont.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d475e-157">If successful, this method returns a `200 OK` response code and updated [RangeFont](../resources/rangefont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d475e-158">示例</span><span class="sxs-lookup"><span data-stu-id="d475e-158">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d475e-159">请求</span><span class="sxs-lookup"><span data-stu-id="d475e-159">Request</span></span>
<span data-ttu-id="d475e-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d475e-160">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_rangefont"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/format/font
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
##### <a name="response"></a><span data-ttu-id="d475e-161">响应</span><span class="sxs-lookup"><span data-stu-id="d475e-161">Response</span></span>
<span data-ttu-id="d475e-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d475e-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFont"
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
  "description": "Update rangefont",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
