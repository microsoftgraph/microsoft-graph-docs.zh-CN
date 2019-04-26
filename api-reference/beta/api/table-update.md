---
title: 更新表
description: 更新 table 对象的属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 5a75f1de081443af7dbb83c675430f79c97c5c0a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33330665"
---
# <a name="update-table"></a><span data-ttu-id="fb403-103">更新表</span><span class="sxs-lookup"><span data-stu-id="fb403-103">Update table</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb403-104">更新 table 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="fb403-104">Update the properties of table object.</span></span>
## <a name="permissions"></a><span data-ttu-id="fb403-105">权限</span><span class="sxs-lookup"><span data-stu-id="fb403-105">Permissions</span></span>
<span data-ttu-id="fb403-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fb403-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb403-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="fb403-108">Permission type</span></span>      | <span data-ttu-id="fb403-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fb403-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fb403-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fb403-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fb403-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fb403-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fb403-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fb403-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb403-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fb403-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fb403-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="fb403-114">Application</span></span> | <span data-ttu-id="fb403-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="fb403-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fb403-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fb403-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}
PATCH /workbook/worksheets/{id|name}/tables/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="fb403-117">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="fb403-117">Optional request headers</span></span>
| <span data-ttu-id="fb403-118">名称</span><span class="sxs-lookup"><span data-stu-id="fb403-118">Name</span></span>       | <span data-ttu-id="fb403-119">说明</span><span class="sxs-lookup"><span data-stu-id="fb403-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="fb403-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb403-120">Authorization</span></span>  | <span data-ttu-id="fb403-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fb403-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fb403-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="fb403-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="fb403-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="fb403-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb403-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="fb403-126">Request body</span></span>
<span data-ttu-id="fb403-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="fb403-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="fb403-130">属性</span><span class="sxs-lookup"><span data-stu-id="fb403-130">Property</span></span>     | <span data-ttu-id="fb403-131">类型</span><span class="sxs-lookup"><span data-stu-id="fb403-131">Type</span></span>   |<span data-ttu-id="fb403-132">说明</span><span class="sxs-lookup"><span data-stu-id="fb403-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fb403-133">name</span><span class="sxs-lookup"><span data-stu-id="fb403-133">name</span></span>|<span data-ttu-id="fb403-134">string</span><span class="sxs-lookup"><span data-stu-id="fb403-134">string</span></span>|<span data-ttu-id="fb403-135">表的名称。</span><span class="sxs-lookup"><span data-stu-id="fb403-135">Name of the table.</span></span>|
|<span data-ttu-id="fb403-136">showHeaders</span><span class="sxs-lookup"><span data-stu-id="fb403-136">showHeaders</span></span>|<span data-ttu-id="fb403-137">布尔</span><span class="sxs-lookup"><span data-stu-id="fb403-137">boolean</span></span>|<span data-ttu-id="fb403-p105">指示标头行是否可见。该值可以设置为显示或删除标头行。</span><span class="sxs-lookup"><span data-stu-id="fb403-p105">Indicates whether the header row is visible or not. This value can be set to show or remove the header row.</span></span>|
|<span data-ttu-id="fb403-140">showTotals</span><span class="sxs-lookup"><span data-stu-id="fb403-140">showTotals</span></span>|<span data-ttu-id="fb403-141">boolean</span><span class="sxs-lookup"><span data-stu-id="fb403-141">boolean</span></span>|<span data-ttu-id="fb403-p106">指示总计行是否可见。该值可以设置为显示或删除总计行。</span><span class="sxs-lookup"><span data-stu-id="fb403-p106">Indicates whether the total row is visible or not. This value can be set to show or remove the total row.</span></span>|
|<span data-ttu-id="fb403-144">style</span><span class="sxs-lookup"><span data-stu-id="fb403-144">style</span></span>|<span data-ttu-id="fb403-145">string</span><span class="sxs-lookup"><span data-stu-id="fb403-145">string</span></span>|<span data-ttu-id="fb403-p107">表示表格样式的常量值。可能的值是：TableStyleLight1 thru TableStyleLight21、TableStyleMedium1 thru TableStyleMedium28、TableStyleStyleDark1 thru TableStyleStyleDark11。还可以指定工作簿中显示的用户定义的自定义样式。</span><span class="sxs-lookup"><span data-stu-id="fb403-p107">Constant value that represents the Table style. Possible values are: TableStyleLight1 thru TableStyleLight21, TableStyleMedium1 thru TableStyleMedium28, TableStyleStyleDark1 thru TableStyleStyleDark11. A custom user-defined style present in the workbook can also be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="fb403-149">响应</span><span class="sxs-lookup"><span data-stu-id="fb403-149">Response</span></span>

<span data-ttu-id="fb403-150">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [Table](../resources/workbooktable.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fb403-150">If successful, this method returns a `200 OK` response code and updated [Table](../resources/workbooktable.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fb403-151">示例</span><span class="sxs-lookup"><span data-stu-id="fb403-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fb403-152">请求</span><span class="sxs-lookup"><span data-stu-id="fb403-152">Request</span></span>
<span data-ttu-id="fb403-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fb403-153">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="fb403-154">响应</span><span class="sxs-lookup"><span data-stu-id="fb403-154">Response</span></span>
<span data-ttu-id="fb403-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fb403-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTable"
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
  "suppressions": []
}
-->
