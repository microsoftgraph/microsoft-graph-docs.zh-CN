---
title: 'workbookRange: columnsBefore'
description: 获取给定范围左侧的一定数量的列。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 046c9c266657cd861c07c2c93ff327dd42e46326
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36421566"
---
# <a name="workbookrange-columnsbefore"></a><span data-ttu-id="db11e-103">workbookRange: columnsBefore</span><span class="sxs-lookup"><span data-stu-id="db11e-103">workbookRange: columnsBefore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db11e-104">获取给定范围左侧的一定数量的列。</span><span class="sxs-lookup"><span data-stu-id="db11e-104">Gets a certain number of columns to the left of the given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="db11e-105">权限</span><span class="sxs-lookup"><span data-stu-id="db11e-105">Permissions</span></span>
<span data-ttu-id="db11e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="db11e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db11e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="db11e-108">Permission type</span></span>      | <span data-ttu-id="db11e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="db11e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db11e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="db11e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="db11e-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="db11e-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="db11e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="db11e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db11e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="db11e-113">Not supported.</span></span>    |
|<span data-ttu-id="db11e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="db11e-114">Application</span></span> | <span data-ttu-id="db11e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="db11e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="db11e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="db11e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/columnsBefore(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="db11e-117">函数参数</span><span class="sxs-lookup"><span data-stu-id="db11e-117">Function parameters</span></span>

| <span data-ttu-id="db11e-118">参数</span><span class="sxs-lookup"><span data-stu-id="db11e-118">Parameter</span></span>    | <span data-ttu-id="db11e-119">类型</span><span class="sxs-lookup"><span data-stu-id="db11e-119">Type</span></span>   |<span data-ttu-id="db11e-120">说明</span><span class="sxs-lookup"><span data-stu-id="db11e-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="db11e-121">count</span><span class="sxs-lookup"><span data-stu-id="db11e-121">count</span></span>|<span data-ttu-id="db11e-122">Int32</span><span class="sxs-lookup"><span data-stu-id="db11e-122">Int32</span></span>|<span data-ttu-id="db11e-p102">生成的范围中要包含的列数。一般来说，使用正数可以在当前范围之外创建一个范围。也可以使用负数在当前范围之内创建一个范围。默认值为 1。</span><span class="sxs-lookup"><span data-stu-id="db11e-p102">The number of columns to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="db11e-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="db11e-127">Request headers</span></span>
| <span data-ttu-id="db11e-128">名称</span><span class="sxs-lookup"><span data-stu-id="db11e-128">Name</span></span>       | <span data-ttu-id="db11e-129">说明</span><span class="sxs-lookup"><span data-stu-id="db11e-129">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="db11e-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="db11e-130">Authorization</span></span>  | <span data-ttu-id="db11e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="db11e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="db11e-133">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="db11e-133">Workbook-Session-Id</span></span>  | <span data-ttu-id="db11e-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="db11e-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="db11e-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="db11e-136">Request body</span></span>
<span data-ttu-id="db11e-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="db11e-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db11e-138">响应</span><span class="sxs-lookup"><span data-stu-id="db11e-138">Response</span></span>
<span data-ttu-id="db11e-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [workbookRange](../resources/workbookrange.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="db11e-139">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db11e-140">示例</span><span class="sxs-lookup"><span data-stu-id="db11e-140">Example</span></span>
<span data-ttu-id="db11e-141">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="db11e-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="db11e-142">请求</span><span class="sxs-lookup"><span data-stu-id="db11e-142">Request</span></span>
<span data-ttu-id="db11e-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="db11e-143">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="db11e-144">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="db11e-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "workbookrange_columnsbefore"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range/columnsBefore(count=2)
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="db11e-145">C#</span><span class="sxs-lookup"><span data-stu-id="db11e-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrange-columnsbefore-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="db11e-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db11e-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrange-columnsbefore-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="db11e-147">目标-C</span><span class="sxs-lookup"><span data-stu-id="db11e-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrange-columnsbefore-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="db11e-148">响应</span><span class="sxs-lookup"><span data-stu-id="db11e-148">Response</span></span>
<span data-ttu-id="db11e-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="db11e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
