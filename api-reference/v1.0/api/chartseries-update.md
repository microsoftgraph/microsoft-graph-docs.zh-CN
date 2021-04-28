---
title: 更新 chartseries
description: 更新 chartseries 对象的属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 5a9b56fd4cdb8e88bf3e614a0ba81f6a16cf2a15
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054110"
---
# <a name="update-chartseries"></a><span data-ttu-id="aa483-103">更新 chartseries</span><span class="sxs-lookup"><span data-stu-id="aa483-103">Update chartseries</span></span>

<span data-ttu-id="aa483-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa483-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="aa483-105">更新 chartseries 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="aa483-105">Update the properties of chartseries object.</span></span>
## <a name="permissions"></a><span data-ttu-id="aa483-106">权限</span><span class="sxs-lookup"><span data-stu-id="aa483-106">Permissions</span></span>
<span data-ttu-id="aa483-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aa483-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa483-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="aa483-109">Permission type</span></span>      | <span data-ttu-id="aa483-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aa483-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aa483-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aa483-111">Delegated (work or school account)</span></span> | <span data-ttu-id="aa483-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aa483-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="aa483-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aa483-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa483-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="aa483-114">Not supported.</span></span>    |
|<span data-ttu-id="aa483-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="aa483-115">Application</span></span> | <span data-ttu-id="aa483-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="aa483-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="aa483-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aa483-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{series-id}
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/series/{series-id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="aa483-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="aa483-118">Optional request headers</span></span>
| <span data-ttu-id="aa483-119">名称</span><span class="sxs-lookup"><span data-stu-id="aa483-119">Name</span></span>       | <span data-ttu-id="aa483-120">说明</span><span class="sxs-lookup"><span data-stu-id="aa483-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="aa483-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa483-121">Authorization</span></span>  | <span data-ttu-id="aa483-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="aa483-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="aa483-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="aa483-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="aa483-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="aa483-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa483-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="aa483-127">Request body</span></span>
<span data-ttu-id="aa483-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="aa483-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="aa483-131">属性</span><span class="sxs-lookup"><span data-stu-id="aa483-131">Property</span></span>     | <span data-ttu-id="aa483-132">类型</span><span class="sxs-lookup"><span data-stu-id="aa483-132">Type</span></span>   |<span data-ttu-id="aa483-133">说明</span><span class="sxs-lookup"><span data-stu-id="aa483-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aa483-134">name</span><span class="sxs-lookup"><span data-stu-id="aa483-134">name</span></span>|<span data-ttu-id="aa483-135">string</span><span class="sxs-lookup"><span data-stu-id="aa483-135">string</span></span>|<span data-ttu-id="aa483-136">表示图表中某个系列的名称。</span><span class="sxs-lookup"><span data-stu-id="aa483-136">Represents the name of a series in a chart.</span></span>|

## <a name="response"></a><span data-ttu-id="aa483-137">响应</span><span class="sxs-lookup"><span data-stu-id="aa483-137">Response</span></span>

<span data-ttu-id="aa483-138">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [WorkbookChartSeries](../resources/chartseries.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="aa483-138">If successful, this method returns a `200 OK` response code and updated [WorkbookChartSeries](../resources/chartseries.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="aa483-139">示例</span><span class="sxs-lookup"><span data-stu-id="aa483-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aa483-140">请求</span><span class="sxs-lookup"><span data-stu-id="aa483-140">Request</span></span>
<span data-ttu-id="aa483-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="aa483-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="aa483-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="aa483-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_chartseries"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{series-id}
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```
# <a name="c"></a>[<span data-ttu-id="aa483-143">C#</span><span class="sxs-lookup"><span data-stu-id="aa483-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chartseries-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aa483-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aa483-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chartseries-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aa483-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aa483-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chartseries-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="aa483-146">Java</span><span class="sxs-lookup"><span data-stu-id="aa483-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-chartseries-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="aa483-147">响应</span><span class="sxs-lookup"><span data-stu-id="aa483-147">Response</span></span>
<span data-ttu-id="aa483-148">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="aa483-148">Here is an example of the response.</span></span> <span data-ttu-id="aa483-149">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="aa483-149">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartSeries"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartseries",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

