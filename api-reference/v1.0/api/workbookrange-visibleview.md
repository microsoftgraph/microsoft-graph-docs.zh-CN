---
title: 'workbookRange: visibleView'
description: 若要调用此 API, 必须有以下权限之一。 若要了解详细信息，包括如何选择权限的信息，请参阅权限。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 284e38d68a48bfaef395335600345cb3134080db
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35278440"
---
# <a name="workbookrange-visibleview"></a><span data-ttu-id="539fb-104">workbookRange: visibleView</span><span class="sxs-lookup"><span data-stu-id="539fb-104">workbookRange: visibleView</span></span>


## <a name="permissions"></a><span data-ttu-id="539fb-105">权限</span><span class="sxs-lookup"><span data-stu-id="539fb-105">Permissions</span></span>
<span data-ttu-id="539fb-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="539fb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="539fb-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="539fb-108">Permission type</span></span>      | <span data-ttu-id="539fb-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="539fb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="539fb-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="539fb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="539fb-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="539fb-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="539fb-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="539fb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="539fb-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="539fb-113">Not supported.</span></span>    |
|<span data-ttu-id="539fb-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="539fb-114">Application</span></span> | <span data-ttu-id="539fb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="539fb-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="539fb-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="539fb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView
```
## <a name="request-headers"></a><span data-ttu-id="539fb-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="539fb-117">Request headers</span></span>
| <span data-ttu-id="539fb-118">名称</span><span class="sxs-lookup"><span data-stu-id="539fb-118">Name</span></span>       | <span data-ttu-id="539fb-119">说明</span><span class="sxs-lookup"><span data-stu-id="539fb-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="539fb-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="539fb-120">Authorization</span></span>  | <span data-ttu-id="539fb-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="539fb-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="539fb-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="539fb-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="539fb-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="539fb-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="539fb-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="539fb-126">Request body</span></span>

### <a name="response"></a><span data-ttu-id="539fb-127">响应</span><span class="sxs-lookup"><span data-stu-id="539fb-127">Response</span></span>
<span data-ttu-id="539fb-128">如果成功，此方法在响应正文中返回 `200 OK`响应代码和 [workbookRangeView](../resources/workbookrangeview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="539fb-128">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="539fb-129">示例</span><span class="sxs-lookup"><span data-stu-id="539fb-129">Example</span></span>
<span data-ttu-id="539fb-130">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="539fb-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="539fb-131">请求</span><span class="sxs-lookup"><span data-stu-id="539fb-131">Request</span></span>
<span data-ttu-id="539fb-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="539fb-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_visibleview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView
```

##### <a name="response"></a><span data-ttu-id="539fb-133">响应</span><span class="sxs-lookup"><span data-stu-id="539fb-133">Response</span></span>
<span data-ttu-id="539fb-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="539fb-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeView"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 194

{
  "cellAddresses": "cellAddresses-value",
  "columnCount": 99,
  "formulas": "formulas-value",
  "formulasLocal": "formulasLocal-value",
  "formulasR1C1": "formulasR1C1-value",
  "index": 99
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="539fb-137">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="539fb-137">SDK sample code</span></span>
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="539fb-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="539fb-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/workbookrange_visibleview-Javascript-snippets.md)]

# <a name="ctabcs"></a>[<span data-ttu-id="539fb-139">C#</span><span class="sxs-lookup"><span data-stu-id="539fb-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/workbookrange_visibleview-Cs-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="539fb-140">目标-C</span><span class="sxs-lookup"><span data-stu-id="539fb-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/workbookrange_visibleview-Objective-C-snippets.md)]
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
    "Error: /api-reference/v1.0/api/workbookrange-visibleview.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/workbookrange-visibleview.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/workbookrange-visibleview.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
