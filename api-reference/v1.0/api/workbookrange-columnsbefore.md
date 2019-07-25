---
title: 'workbookRange: columnsBefore'
description: 获取给定范围左侧的一定数量的列。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 93674f4dcc37708bc682d8831ad4d135a50681ef
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35886878"
---
# <a name="workbookrange-columnsbefore"></a><span data-ttu-id="6e590-103">workbookRange: columnsBefore</span><span class="sxs-lookup"><span data-stu-id="6e590-103">workbookRange: columnsBefore</span></span>

<span data-ttu-id="6e590-104">获取给定范围左侧的一定数量的列。</span><span class="sxs-lookup"><span data-stu-id="6e590-104">Gets a certain number of columns to the left of the given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="6e590-105">权限</span><span class="sxs-lookup"><span data-stu-id="6e590-105">Permissions</span></span>
<span data-ttu-id="6e590-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6e590-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e590-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="6e590-108">Permission type</span></span>      | <span data-ttu-id="6e590-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6e590-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6e590-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6e590-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6e590-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6e590-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6e590-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6e590-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e590-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="6e590-113">Not supported.</span></span>    |
|<span data-ttu-id="6e590-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="6e590-114">Application</span></span> | <span data-ttu-id="6e590-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6e590-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6e590-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6e590-116">HTTP request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6e590-117">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="6e590-117">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/columnsBefore(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="6e590-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="6e590-118">Function parameters</span></span>

| <span data-ttu-id="6e590-119">参数</span><span class="sxs-lookup"><span data-stu-id="6e590-119">Parameter</span></span>    | <span data-ttu-id="6e590-120">类型</span><span class="sxs-lookup"><span data-stu-id="6e590-120">Type</span></span>   |<span data-ttu-id="6e590-121">说明</span><span class="sxs-lookup"><span data-stu-id="6e590-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6e590-122">count</span><span class="sxs-lookup"><span data-stu-id="6e590-122">count</span></span>|<span data-ttu-id="6e590-123">Int32</span><span class="sxs-lookup"><span data-stu-id="6e590-123">Int32</span></span>|<span data-ttu-id="6e590-p102">可选。生成的范围中要包含的列数。一般来说，使用正数可以在当前范围之外创建一个范围。也可以使用负数在当前范围之内创建一个范围。默认值为 1。</span><span class="sxs-lookup"><span data-stu-id="6e590-p102">Optional. The number of columns to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="6e590-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="6e590-129">Request headers</span></span>
| <span data-ttu-id="6e590-130">名称</span><span class="sxs-lookup"><span data-stu-id="6e590-130">Name</span></span>       | <span data-ttu-id="6e590-131">说明</span><span class="sxs-lookup"><span data-stu-id="6e590-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6e590-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e590-132">Authorization</span></span>  | <span data-ttu-id="6e590-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6e590-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6e590-135">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="6e590-135">Workbook-Session-Id</span></span>  | <span data-ttu-id="6e590-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="6e590-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e590-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="6e590-138">Request body</span></span>
<span data-ttu-id="6e590-139">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6e590-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e590-140">响应</span><span class="sxs-lookup"><span data-stu-id="6e590-140">Response</span></span>
<span data-ttu-id="6e590-141">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [workbookRange](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6e590-141">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e590-142">示例</span><span class="sxs-lookup"><span data-stu-id="6e590-142">Example</span></span>
<span data-ttu-id="6e590-143">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="6e590-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6e590-144">请求</span><span class="sxs-lookup"><span data-stu-id="6e590-144">Request</span></span>
<span data-ttu-id="6e590-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6e590-145">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_columnsbefore",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/columnsBefore(count=2)
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6e590-146">C#</span><span class="sxs-lookup"><span data-stu-id="6e590-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrange-columnsbefore-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6e590-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="6e590-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrange-columnsbefore-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6e590-148">目标-C</span><span class="sxs-lookup"><span data-stu-id="6e590-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrange-columnsbefore-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6e590-149">Java</span><span class="sxs-lookup"><span data-stu-id="6e590-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookrange-columnsbefore-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6e590-150">响应</span><span class="sxs-lookup"><span data-stu-id="6e590-150">Response</span></span>
<span data-ttu-id="6e590-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6e590-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 157

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnHidden": true,
  "columnIndex": 99
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
