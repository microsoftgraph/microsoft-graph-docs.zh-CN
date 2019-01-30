---
title: 更新表
description: 更新 table 对象的属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 2b78603a261145e2047b5e16175143a3b3c591e1
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641741"
---
# <a name="update-table"></a><span data-ttu-id="e4e38-103">更新表</span><span class="sxs-lookup"><span data-stu-id="e4e38-103">Update table</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4e38-104">更新 table 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e4e38-104">Update the properties of table object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e4e38-105">权限</span><span class="sxs-lookup"><span data-stu-id="e4e38-105">Permissions</span></span>
<span data-ttu-id="e4e38-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e4e38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4e38-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e4e38-108">Permission type</span></span>      | <span data-ttu-id="e4e38-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e4e38-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e4e38-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e4e38-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e4e38-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e4e38-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e4e38-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e4e38-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4e38-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e4e38-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e4e38-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e4e38-114">Application</span></span> | <span data-ttu-id="e4e38-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e4e38-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e4e38-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e4e38-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}
PATCH /workbook/worksheets/{id|name}/tables/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="e4e38-117">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="e4e38-117">Optional request headers</span></span>
| <span data-ttu-id="e4e38-118">名称</span><span class="sxs-lookup"><span data-stu-id="e4e38-118">Name</span></span>       | <span data-ttu-id="e4e38-119">说明</span><span class="sxs-lookup"><span data-stu-id="e4e38-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e4e38-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4e38-120">Authorization</span></span>  | <span data-ttu-id="e4e38-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e4e38-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e4e38-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e4e38-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="e4e38-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="e4e38-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4e38-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e4e38-126">Request body</span></span>
<span data-ttu-id="e4e38-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="e4e38-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e4e38-130">属性</span><span class="sxs-lookup"><span data-stu-id="e4e38-130">Property</span></span>     | <span data-ttu-id="e4e38-131">类型</span><span class="sxs-lookup"><span data-stu-id="e4e38-131">Type</span></span>   |<span data-ttu-id="e4e38-132">说明</span><span class="sxs-lookup"><span data-stu-id="e4e38-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e4e38-133">name</span><span class="sxs-lookup"><span data-stu-id="e4e38-133">name</span></span>|<span data-ttu-id="e4e38-134">string</span><span class="sxs-lookup"><span data-stu-id="e4e38-134">string</span></span>|<span data-ttu-id="e4e38-135">表的名称。</span><span class="sxs-lookup"><span data-stu-id="e4e38-135">Name of the table.</span></span>|
|<span data-ttu-id="e4e38-136">showHeaders</span><span class="sxs-lookup"><span data-stu-id="e4e38-136">showHeaders</span></span>|<span data-ttu-id="e4e38-137">boolean</span><span class="sxs-lookup"><span data-stu-id="e4e38-137">boolean</span></span>|<span data-ttu-id="e4e38-p105">指示标头行是否可见。该值可以设置为显示或删除标头行。</span><span class="sxs-lookup"><span data-stu-id="e4e38-p105">Indicates whether the header row is visible or not. This value can be set to show or remove the header row.</span></span>|
|<span data-ttu-id="e4e38-140">showTotals</span><span class="sxs-lookup"><span data-stu-id="e4e38-140">showTotals</span></span>|<span data-ttu-id="e4e38-141">boolean</span><span class="sxs-lookup"><span data-stu-id="e4e38-141">boolean</span></span>|<span data-ttu-id="e4e38-p106">指示总计行是否可见。该值可以设置为显示或删除总计行。</span><span class="sxs-lookup"><span data-stu-id="e4e38-p106">Indicates whether the total row is visible or not. This value can be set to show or remove the total row.</span></span>|
|<span data-ttu-id="e4e38-144">style</span><span class="sxs-lookup"><span data-stu-id="e4e38-144">style</span></span>|<span data-ttu-id="e4e38-145">string</span><span class="sxs-lookup"><span data-stu-id="e4e38-145">string</span></span>|<span data-ttu-id="e4e38-p107">表示表格样式的常量值。可能的值是：TableStyleLight1 thru TableStyleLight21、TableStyleMedium1 thru TableStyleMedium28、TableStyleStyleDark1 thru TableStyleStyleDark11。还可以指定工作簿中显示的用户定义的自定义样式。</span><span class="sxs-lookup"><span data-stu-id="e4e38-p107">Constant value that represents the Table style. Possible values are: TableStyleLight1 thru TableStyleLight21, TableStyleMedium1 thru TableStyleMedium28, TableStyleStyleDark1 thru TableStyleStyleDark11. A custom user-defined style present in the workbook can also be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="e4e38-149">响应</span><span class="sxs-lookup"><span data-stu-id="e4e38-149">Response</span></span>

<span data-ttu-id="e4e38-150">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [Table](../resources/table.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e4e38-150">If successful, this method returns a `200 OK` response code and updated [Table](../resources/table.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e4e38-151">示例</span><span class="sxs-lookup"><span data-stu-id="e4e38-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e4e38-152">请求</span><span class="sxs-lookup"><span data-stu-id="e4e38-152">Request</span></span>
<span data-ttu-id="e4e38-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e4e38-153">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_table"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}
Content-type: application/json
Content-length: 109

{
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```
##### <a name="response"></a><span data-ttu-id="e4e38-154">响应</span><span class="sxs-lookup"><span data-stu-id="e4e38-154">Response</span></span>
<span data-ttu-id="e4e38-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e4e38-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.table"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 109

{
  "id": "99",
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update table",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/table-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
