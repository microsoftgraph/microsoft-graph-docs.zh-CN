---
title: 'workbookRange: rowsAbove'
description: 获取给定范围上方的一定数量的行。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 7d80841d0e9cda13cf5cbca4430186737fbfcc44
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636917"
---
# <a name="workbookrange-rowsabove"></a><span data-ttu-id="bdaa0-103">workbookRange: rowsAbove</span><span class="sxs-lookup"><span data-stu-id="bdaa0-103">workbookRange: rowsAbove</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bdaa0-104">获取给定范围上方的一定数量的行。</span><span class="sxs-lookup"><span data-stu-id="bdaa0-104">Gets a certain number of rows above a given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="bdaa0-105">权限</span><span class="sxs-lookup"><span data-stu-id="bdaa0-105">Permissions</span></span>
<span data-ttu-id="bdaa0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bdaa0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bdaa0-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="bdaa0-108">Permission type</span></span>      | <span data-ttu-id="bdaa0-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bdaa0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bdaa0-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bdaa0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bdaa0-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bdaa0-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bdaa0-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bdaa0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bdaa0-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bdaa0-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bdaa0-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="bdaa0-114">Application</span></span> | <span data-ttu-id="bdaa0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="bdaa0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bdaa0-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bdaa0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/rowsAbove(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="bdaa0-117">函数参数</span><span class="sxs-lookup"><span data-stu-id="bdaa0-117">Function parameters</span></span>

| <span data-ttu-id="bdaa0-118">参数</span><span class="sxs-lookup"><span data-stu-id="bdaa0-118">Parameter</span></span>    | <span data-ttu-id="bdaa0-119">类型</span><span class="sxs-lookup"><span data-stu-id="bdaa0-119">Type</span></span>   |<span data-ttu-id="bdaa0-120">说明</span><span class="sxs-lookup"><span data-stu-id="bdaa0-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bdaa0-121">count</span><span class="sxs-lookup"><span data-stu-id="bdaa0-121">count</span></span>|<span data-ttu-id="bdaa0-122">Int32</span><span class="sxs-lookup"><span data-stu-id="bdaa0-122">Int32</span></span>|<span data-ttu-id="bdaa0-p102">可选。生成的范围中要包含的行数。一般来说，使用正数可以在当前范围之外创建一个范围。也可以使用负数在当前范围之内创建一个范围。默认值为 1。</span><span class="sxs-lookup"><span data-stu-id="bdaa0-p102">Optional. The number of rows to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="bdaa0-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="bdaa0-128">Request headers</span></span>
| <span data-ttu-id="bdaa0-129">名称</span><span class="sxs-lookup"><span data-stu-id="bdaa0-129">Name</span></span>       | <span data-ttu-id="bdaa0-130">说明</span><span class="sxs-lookup"><span data-stu-id="bdaa0-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bdaa0-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="bdaa0-131">Authorization</span></span>  | <span data-ttu-id="bdaa0-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bdaa0-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bdaa0-134">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="bdaa0-134">Workbook-Session-Id</span></span>  | <span data-ttu-id="bdaa0-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="bdaa0-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bdaa0-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="bdaa0-137">Request body</span></span>
<span data-ttu-id="bdaa0-138">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bdaa0-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bdaa0-139">响应</span><span class="sxs-lookup"><span data-stu-id="bdaa0-139">Response</span></span>

<span data-ttu-id="bdaa0-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [workbookRange](../resources/workbookrange.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bdaa0-140">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bdaa0-141">示例</span><span class="sxs-lookup"><span data-stu-id="bdaa0-141">Example</span></span>
<span data-ttu-id="bdaa0-142">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="bdaa0-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="bdaa0-143">请求</span><span class="sxs-lookup"><span data-stu-id="bdaa0-143">Request</span></span>
<span data-ttu-id="bdaa0-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bdaa0-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_rowsAbove"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range/rowsAbove(count=2)
```

##### <a name="response"></a><span data-ttu-id="bdaa0-145">响应</span><span class="sxs-lookup"><span data-stu-id="bdaa0-145">Response</span></span>
<span data-ttu-id="bdaa0-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bdaa0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="bdaa0-149">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="bdaa0-149">SDK sample code</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="bdaa0-150">语言</span><span class="sxs-lookup"><span data-stu-id="bdaa0-150">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/workbookrange_rowsAbove-Cs-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/workbookrange-rowsabove.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/workbookrange-rowsabove.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
