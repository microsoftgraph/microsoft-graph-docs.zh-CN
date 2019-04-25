---
title: 更新工作表
description: 更新 worksheet 对象的属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 651900f00e842640b292deef7569efde1701939b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569702"
---
# <a name="update-worksheet"></a><span data-ttu-id="e4602-103">更新工作表</span><span class="sxs-lookup"><span data-stu-id="e4602-103">Update worksheet</span></span>

<span data-ttu-id="e4602-104">更新 worksheet 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e4602-104">Update the properties of worksheet object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e4602-105">权限</span><span class="sxs-lookup"><span data-stu-id="e4602-105">Permissions</span></span>
<span data-ttu-id="e4602-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e4602-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4602-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e4602-108">Permission type</span></span>      | <span data-ttu-id="e4602-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e4602-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e4602-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e4602-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e4602-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e4602-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e4602-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e4602-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4602-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="e4602-113">Not supported.</span></span>    |
|<span data-ttu-id="e4602-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e4602-114">Application</span></span> | <span data-ttu-id="e4602-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e4602-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e4602-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e4602-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="e4602-117">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="e4602-117">Optional request headers</span></span>
| <span data-ttu-id="e4602-118">名称</span><span class="sxs-lookup"><span data-stu-id="e4602-118">Name</span></span>       | <span data-ttu-id="e4602-119">说明</span><span class="sxs-lookup"><span data-stu-id="e4602-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e4602-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4602-120">Authorization</span></span>  | <span data-ttu-id="e4602-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e4602-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e4602-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e4602-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="e4602-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="e4602-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4602-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e4602-126">Request body</span></span>
<span data-ttu-id="e4602-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="e4602-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e4602-130">属性</span><span class="sxs-lookup"><span data-stu-id="e4602-130">Property</span></span>     | <span data-ttu-id="e4602-131">类型</span><span class="sxs-lookup"><span data-stu-id="e4602-131">Type</span></span>   |<span data-ttu-id="e4602-132">说明</span><span class="sxs-lookup"><span data-stu-id="e4602-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e4602-133">name</span><span class="sxs-lookup"><span data-stu-id="e4602-133">name</span></span>|<span data-ttu-id="e4602-134">string</span><span class="sxs-lookup"><span data-stu-id="e4602-134">string</span></span>|<span data-ttu-id="e4602-135">工作表的显示名称。</span><span class="sxs-lookup"><span data-stu-id="e4602-135">The display name of the worksheet.</span></span>|
|<span data-ttu-id="e4602-136">position</span><span class="sxs-lookup"><span data-stu-id="e4602-136">position</span></span>|<span data-ttu-id="e4602-137">int</span><span class="sxs-lookup"><span data-stu-id="e4602-137">int</span></span>|<span data-ttu-id="e4602-138">工作表在工作簿中的位置，从零开始。</span><span class="sxs-lookup"><span data-stu-id="e4602-138">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="e4602-139">visibility</span><span class="sxs-lookup"><span data-stu-id="e4602-139">visibility</span></span>|<span data-ttu-id="e4602-140">string</span><span class="sxs-lookup"><span data-stu-id="e4602-140">string</span></span>|<span data-ttu-id="e4602-141">工作表的可见性。</span><span class="sxs-lookup"><span data-stu-id="e4602-141">The Visibility of the worksheet.</span></span> <span data-ttu-id="e4602-142">可能的值包括 `Visible`、`Hidden`、`VeryHidden`。</span><span class="sxs-lookup"><span data-stu-id="e4602-142">The possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="response"></a><span data-ttu-id="e4602-143">响应</span><span class="sxs-lookup"><span data-stu-id="e4602-143">Response</span></span>

<span data-ttu-id="e4602-144">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[WorkbookWorksheet](../resources/worksheet.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e4602-144">If successful, this method returns a `200 OK` response code and updated [WorkbookWorksheet](../resources/worksheet.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e4602-145">示例</span><span class="sxs-lookup"><span data-stu-id="e4602-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e4602-146">请求</span><span class="sxs-lookup"><span data-stu-id="e4602-146">Request</span></span>
<span data-ttu-id="e4602-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e4602-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_worksheet"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}
Content-type: application/json
Content-length: 100

{
  "position": 99,
  "name": "name-value",
  "visibility": "visibility-value"
}
```
##### <a name="response"></a><span data-ttu-id="e4602-148">响应</span><span class="sxs-lookup"><span data-stu-id="e4602-148">Response</span></span>
<span data-ttu-id="e4602-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e4602-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookWorksheet"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "id": "id-value",
  "position": 99,
  "name": "name-value",
  "visibility": "visibility-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update worksheet",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
