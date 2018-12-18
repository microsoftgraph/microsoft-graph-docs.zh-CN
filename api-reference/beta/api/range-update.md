---
title: 更新区域
description: 更新 range 对象的属性。
author: lumine2008
ms.openlocfilehash: de084bd15ad448d6723b62fde4ea7761e2b5607a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27347430"
---
# <a name="update-range"></a><span data-ttu-id="830de-103">更新区域</span><span class="sxs-lookup"><span data-stu-id="830de-103">Update range</span></span>

> <span data-ttu-id="830de-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="830de-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="830de-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="830de-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="830de-106">更新 range 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="830de-106">Update the properties of range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="830de-107">权限</span><span class="sxs-lookup"><span data-stu-id="830de-107">Permissions</span></span>
<span data-ttu-id="830de-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="830de-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="830de-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="830de-110">Permission type</span></span>      | <span data-ttu-id="830de-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="830de-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="830de-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="830de-112">Delegated (work or school account)</span></span> | <span data-ttu-id="830de-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="830de-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="830de-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="830de-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="830de-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="830de-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="830de-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="830de-116">Application</span></span> | <span data-ttu-id="830de-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="830de-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="830de-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="830de-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range
PATCH /workbook/worksheets/{id|name}/range(address='<address>')
PATCH /workbook/tables/{id|name}/columns/{id|name}/range
```
## <a name="optional-request-headers"></a><span data-ttu-id="830de-119">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="830de-119">Optional request headers</span></span>
| <span data-ttu-id="830de-120">Name</span><span class="sxs-lookup"><span data-stu-id="830de-120">Name</span></span>       | <span data-ttu-id="830de-121">说明</span><span class="sxs-lookup"><span data-stu-id="830de-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="830de-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="830de-122">Authorization</span></span>  | <span data-ttu-id="830de-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="830de-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="830de-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="830de-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="830de-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="830de-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="830de-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="830de-128">Request body</span></span>
<span data-ttu-id="830de-p105">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="830de-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="830de-132">属性</span><span class="sxs-lookup"><span data-stu-id="830de-132">Property</span></span>     | <span data-ttu-id="830de-133">类型</span><span class="sxs-lookup"><span data-stu-id="830de-133">Type</span></span>   |<span data-ttu-id="830de-134">说明</span><span class="sxs-lookup"><span data-stu-id="830de-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="830de-135">columnHidden</span><span class="sxs-lookup"><span data-stu-id="830de-135">columnHidden</span></span>|<span data-ttu-id="830de-136">boolean</span><span class="sxs-lookup"><span data-stu-id="830de-136">boolean</span></span>|<span data-ttu-id="830de-137">表示当前区域中的所有列是否隐藏。</span><span class="sxs-lookup"><span data-stu-id="830de-137">Represents if all columns of the current range are hidden.</span></span>|
|<span data-ttu-id="830de-138">formulas</span><span class="sxs-lookup"><span data-stu-id="830de-138">formulas</span></span>|<span data-ttu-id="830de-139">json</span><span class="sxs-lookup"><span data-stu-id="830de-139">json</span></span>|<span data-ttu-id="830de-140">表示采用 A1 样式表示法的公式。</span><span class="sxs-lookup"><span data-stu-id="830de-140">Represents the formula in A1-style notation.</span></span>|
|<span data-ttu-id="830de-141">formulasLocal</span><span class="sxs-lookup"><span data-stu-id="830de-141">formulasLocal</span></span>|<span data-ttu-id="830de-142">json</span><span class="sxs-lookup"><span data-stu-id="830de-142">json</span></span>|<span data-ttu-id="830de-p106">表示采用 A1 样式表示法的公式，使用用户的语言和数字格式区域设置。例如，英语中的公式 "=SUM(A1, 1.5)" 在德语中将变为 "=SUMME(A1; 1,5)"。</span><span class="sxs-lookup"><span data-stu-id="830de-p106">Represents the formula in A1-style notation, in the user's language and number-formatting locale.  For example, the English "=SUM(A1, 1.5)" formula would become "=SUMME(A1; 1,5)" in German.</span></span>|
|<span data-ttu-id="830de-145">formulasR1C1</span><span class="sxs-lookup"><span data-stu-id="830de-145">formulasR1C1</span></span>|<span data-ttu-id="830de-146">json</span><span class="sxs-lookup"><span data-stu-id="830de-146">json</span></span>|<span data-ttu-id="830de-147">表示采用 R1C1 样式表示法的公式。</span><span class="sxs-lookup"><span data-stu-id="830de-147">Represents the formula in R1C1-style notation.</span></span>|
|<span data-ttu-id="830de-148">numberFormat</span><span class="sxs-lookup"><span data-stu-id="830de-148">numberFormat</span></span>|<span data-ttu-id="830de-149">json</span><span class="sxs-lookup"><span data-stu-id="830de-149">json</span></span>|<span data-ttu-id="830de-150">表示 Excel 中指定单元格的数字格式代码。</span><span class="sxs-lookup"><span data-stu-id="830de-150">Represents Excel's number format code for the given cell.</span></span>|
|<span data-ttu-id="830de-151">rowHidden</span><span class="sxs-lookup"><span data-stu-id="830de-151">rowHidden</span></span>|<span data-ttu-id="830de-152">boolean</span><span class="sxs-lookup"><span data-stu-id="830de-152">boolean</span></span>|<span data-ttu-id="830de-153">表示当前区域中的所有行是否隐藏。</span><span class="sxs-lookup"><span data-stu-id="830de-153">Represents if all rows of the current range are hidden.</span></span>|
|<span data-ttu-id="830de-154">values</span><span class="sxs-lookup"><span data-stu-id="830de-154">values</span></span>|<span data-ttu-id="830de-155">json</span><span class="sxs-lookup"><span data-stu-id="830de-155">json</span></span>|<span data-ttu-id="830de-p107">表示指定区域的原始值。返回的数据类型可能是字符串、数字或布尔值。包含一个将返回错误字符串的错误的单元格。</span><span class="sxs-lookup"><span data-stu-id="830de-p107">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="830de-159">响应</span><span class="sxs-lookup"><span data-stu-id="830de-159">Response</span></span>

<span data-ttu-id="830de-160">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="830de-160">If successful, this method returns a `200 OK` response code and updated [Range](../resources/range.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="830de-161">示例</span><span class="sxs-lookup"><span data-stu-id="830de-161">Example</span></span>
##### <a name="request"></a><span data-ttu-id="830de-162">请求</span><span class="sxs-lookup"><span data-stu-id="830de-162">Request</span></span>
<span data-ttu-id="830de-p108">下面是一个请求示例。该示例更新区域 - 值、数字格式和公式。`null` 输入是为了指示 API 忽略单元格的特定输入。值、数字格式和公式可以独立更新，也可以在同一 API 调用中共同更新。</span><span class="sxs-lookup"><span data-stu-id="830de-p108">Here is an example of the request. It updates a range - values, number-format and formula. The `null` input is to instruct the API to ignore the cell for that particular input. The values, number-format and formulas can be independently updated or combined together in the same API call.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_range"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets('sheet1')/range(address='A1:B2')
Content-type: application/json
Content-length: 169

{
"values" : [["Hello", "100"],["1/1/2016", null]],
"formula" : [[null, null], [null, "=B1*2"]],
"numberFormat" : [[null,null], ["m-ddd", null]]
}
```
##### <a name="response"></a><span data-ttu-id="830de-167">响应</span><span class="sxs-lookup"><span data-stu-id="830de-167">Response</span></span>
<span data-ttu-id="830de-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="830de-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update range",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
