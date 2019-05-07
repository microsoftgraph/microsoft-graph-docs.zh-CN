---
title: Range:EntireRow
description: 获取表示范围整行的对象。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: b529d33cc78de29ed69d60aa20352bb575e005d2
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33607550"
---
# <a name="range-entirerow"></a><span data-ttu-id="7f04a-103">Range:EntireRow</span><span class="sxs-lookup"><span data-stu-id="7f04a-103">Range: EntireRow</span></span>

<span data-ttu-id="7f04a-104">获取表示范围整行的对象。</span><span class="sxs-lookup"><span data-stu-id="7f04a-104">Gets an object that represents the entire row of the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="7f04a-105">权限</span><span class="sxs-lookup"><span data-stu-id="7f04a-105">Permissions</span></span>
<span data-ttu-id="7f04a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7f04a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f04a-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="7f04a-108">Permission type</span></span>      | <span data-ttu-id="7f04a-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7f04a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f04a-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7f04a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7f04a-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7f04a-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7f04a-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7f04a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f04a-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="7f04a-113">Not supported.</span></span>    |
|<span data-ttu-id="7f04a-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="7f04a-114">Application</span></span> | <span data-ttu-id="7f04a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7f04a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f04a-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7f04a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/entireRow
GET /workbook/worksheets/{id|name}/range(address='<address>'/entireRow
GET /workbook/tables/{id|name}/columns/{id|name}/range/entireRow

```
## <a name="request-headers"></a><span data-ttu-id="7f04a-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="7f04a-117">Request headers</span></span>
| <span data-ttu-id="7f04a-118">名称</span><span class="sxs-lookup"><span data-stu-id="7f04a-118">Name</span></span>       | <span data-ttu-id="7f04a-119">说明</span><span class="sxs-lookup"><span data-stu-id="7f04a-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7f04a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f04a-120">Authorization</span></span>  | <span data-ttu-id="7f04a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7f04a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7f04a-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7f04a-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="7f04a-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="7f04a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f04a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="7f04a-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="7f04a-127">响应</span><span class="sxs-lookup"><span data-stu-id="7f04a-127">Response</span></span>

<span data-ttu-id="7f04a-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7f04a-128">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f04a-129">示例</span><span class="sxs-lookup"><span data-stu-id="7f04a-129">Example</span></span>
<span data-ttu-id="7f04a-130">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="7f04a-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7f04a-131">请求</span><span class="sxs-lookup"><span data-stu-id="7f04a-131">Request</span></span>
<span data-ttu-id="7f04a-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7f04a-132">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_entirerow"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/entireRow
```

##### <a name="response"></a><span data-ttu-id="7f04a-133">响应</span><span class="sxs-lookup"><span data-stu-id="7f04a-133">Response</span></span>
<span data-ttu-id="7f04a-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7f04a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="7f04a-137">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="7f04a-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7f04a-138">语言</span><span class="sxs-lookup"><span data-stu-id="7f04a-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/range_entirerow-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7f04a-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="7f04a-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/range_entirerow-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: EntireRow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/range-entirerow.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/range-entirerow.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
