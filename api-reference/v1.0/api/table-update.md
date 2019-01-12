---
title: 更新表
description: 更新 table 对象的属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: df975d13ddc97c0c6b592d02d61a978c5a0db732
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919811"
---
# <a name="update-table"></a><span data-ttu-id="8ebcf-103">更新表</span><span class="sxs-lookup"><span data-stu-id="8ebcf-103">Update table</span></span>

<span data-ttu-id="8ebcf-104">更新 table 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8ebcf-104">Update the properties of table object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8ebcf-105">权限</span><span class="sxs-lookup"><span data-stu-id="8ebcf-105">Permissions</span></span>
<span data-ttu-id="8ebcf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8ebcf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ebcf-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="8ebcf-108">Permission type</span></span>      | <span data-ttu-id="8ebcf-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8ebcf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8ebcf-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8ebcf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8ebcf-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8ebcf-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8ebcf-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8ebcf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ebcf-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="8ebcf-113">Not supported.</span></span>    |
|<span data-ttu-id="8ebcf-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="8ebcf-114">Application</span></span> | <span data-ttu-id="8ebcf-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8ebcf-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8ebcf-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8ebcf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}
PATCH /workbook/worksheets/{id|name}/tables/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="8ebcf-117">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="8ebcf-117">Optional request headers</span></span>
| <span data-ttu-id="8ebcf-118">名称</span><span class="sxs-lookup"><span data-stu-id="8ebcf-118">Name</span></span>       | <span data-ttu-id="8ebcf-119">说明</span><span class="sxs-lookup"><span data-stu-id="8ebcf-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="8ebcf-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ebcf-120">Authorization</span></span>  | <span data-ttu-id="8ebcf-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8ebcf-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8ebcf-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8ebcf-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="8ebcf-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="8ebcf-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ebcf-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8ebcf-126">Request body</span></span>
<span data-ttu-id="8ebcf-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="8ebcf-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8ebcf-130">属性</span><span class="sxs-lookup"><span data-stu-id="8ebcf-130">Property</span></span>     | <span data-ttu-id="8ebcf-131">类型</span><span class="sxs-lookup"><span data-stu-id="8ebcf-131">Type</span></span>   |<span data-ttu-id="8ebcf-132">说明</span><span class="sxs-lookup"><span data-stu-id="8ebcf-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8ebcf-133">name</span><span class="sxs-lookup"><span data-stu-id="8ebcf-133">name</span></span>|<span data-ttu-id="8ebcf-134">string</span><span class="sxs-lookup"><span data-stu-id="8ebcf-134">string</span></span>|<span data-ttu-id="8ebcf-135">表的名称。</span><span class="sxs-lookup"><span data-stu-id="8ebcf-135">Name of the table.</span></span>|
|<span data-ttu-id="8ebcf-136">showHeaders</span><span class="sxs-lookup"><span data-stu-id="8ebcf-136">showHeaders</span></span>|<span data-ttu-id="8ebcf-137">boolean</span><span class="sxs-lookup"><span data-stu-id="8ebcf-137">boolean</span></span>|<span data-ttu-id="8ebcf-p105">指示标头行是否可见。该值可以设置为显示或删除标头行。</span><span class="sxs-lookup"><span data-stu-id="8ebcf-p105">Indicates whether the header row is visible or not. This value can be set to show or remove the header row.</span></span>|
|<span data-ttu-id="8ebcf-140">showTotals</span><span class="sxs-lookup"><span data-stu-id="8ebcf-140">showTotals</span></span>|<span data-ttu-id="8ebcf-141">boolean</span><span class="sxs-lookup"><span data-stu-id="8ebcf-141">boolean</span></span>|<span data-ttu-id="8ebcf-p106">指示总计行是否可见。该值可以设置为显示或删除总计行。</span><span class="sxs-lookup"><span data-stu-id="8ebcf-p106">Indicates whether the total row is visible or not. This value can be set to show or remove the total row.</span></span>|
|<span data-ttu-id="8ebcf-144">style</span><span class="sxs-lookup"><span data-stu-id="8ebcf-144">style</span></span>|<span data-ttu-id="8ebcf-145">string</span><span class="sxs-lookup"><span data-stu-id="8ebcf-145">string</span></span>|<span data-ttu-id="8ebcf-146">代表表格样式的常量值。</span><span class="sxs-lookup"><span data-stu-id="8ebcf-146">Constant value that represents the Table style.</span></span> <span data-ttu-id="8ebcf-147">可能的值为： 至 TableStyleLight21，至 TableStyleMedium28，至 TableStyleStyleDark11 TableStyleStyleDark1 TableStyleMedium1 TableStyleLight1。</span><span class="sxs-lookup"><span data-stu-id="8ebcf-147">The possible values are: TableStyleLight1 thru TableStyleLight21, TableStyleMedium1 thru TableStyleMedium28, TableStyleStyleDark1 thru TableStyleStyleDark11.</span></span> <span data-ttu-id="8ebcf-148">此外可以指定自定义用户定义的样式工作簿中存在。</span><span class="sxs-lookup"><span data-stu-id="8ebcf-148">A custom user-defined style present in the workbook can also be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="8ebcf-149">响应</span><span class="sxs-lookup"><span data-stu-id="8ebcf-149">Response</span></span>

<span data-ttu-id="8ebcf-150">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[WorkbookTable](../resources/table.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8ebcf-150">If successful, this method returns a `200 OK` response code and updated [WorkbookTable](../resources/table.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8ebcf-151">示例</span><span class="sxs-lookup"><span data-stu-id="8ebcf-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8ebcf-152">请求</span><span class="sxs-lookup"><span data-stu-id="8ebcf-152">Request</span></span>
<span data-ttu-id="8ebcf-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8ebcf-153">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_table"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}
Content-type: application/json
Content-length: 109

{
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```
##### <a name="response"></a><span data-ttu-id="8ebcf-154">响应</span><span class="sxs-lookup"><span data-stu-id="8ebcf-154">Response</span></span>
<span data-ttu-id="8ebcf-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8ebcf-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update table",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
