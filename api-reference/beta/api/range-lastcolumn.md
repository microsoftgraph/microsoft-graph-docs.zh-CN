---
title: Range:LastColumn
description: .
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 25e47476f4118d176363367275567b02bf68686a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36309102"
---
# <a name="range-lastcolumn"></a><span data-ttu-id="dfb46-103">Range:LastColumn</span><span class="sxs-lookup"><span data-stu-id="dfb46-103">Range: LastColumn</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dfb46-p101">获取区域内的最后一列。例如，“B2:D5”的最后一列是“D2:D5”。</span><span class="sxs-lookup"><span data-stu-id="dfb46-p101">Gets the last column within the range. For example, the last column of "B2:D5" is "D2:D5".</span></span>
## <a name="permissions"></a><span data-ttu-id="dfb46-106">权限</span><span class="sxs-lookup"><span data-stu-id="dfb46-106">Permissions</span></span>
<span data-ttu-id="dfb46-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dfb46-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dfb46-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="dfb46-109">Permission type</span></span>      | <span data-ttu-id="dfb46-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dfb46-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dfb46-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dfb46-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dfb46-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dfb46-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dfb46-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dfb46-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dfb46-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dfb46-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dfb46-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="dfb46-115">Application</span></span> | <span data-ttu-id="dfb46-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="dfb46-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dfb46-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dfb46-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/LastColumn
GET /workbook/worksheets/{id|name}/range(address='<address>')/LastColumn
GET /workbook/tables/{id|name}/columns/{id|name}/range/LastColumn

```
## <a name="request-headers"></a><span data-ttu-id="dfb46-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="dfb46-118">Request headers</span></span>
| <span data-ttu-id="dfb46-119">名称</span><span class="sxs-lookup"><span data-stu-id="dfb46-119">Name</span></span>       | <span data-ttu-id="dfb46-120">说明</span><span class="sxs-lookup"><span data-stu-id="dfb46-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="dfb46-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="dfb46-121">Authorization</span></span>  | <span data-ttu-id="dfb46-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dfb46-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dfb46-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="dfb46-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="dfb46-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="dfb46-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dfb46-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="dfb46-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="dfb46-128">响应</span><span class="sxs-lookup"><span data-stu-id="dfb46-128">Response</span></span>

<span data-ttu-id="dfb46-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [workbookRange](../resources/workbookrange.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dfb46-129">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dfb46-130">示例</span><span class="sxs-lookup"><span data-stu-id="dfb46-130">Example</span></span>
<span data-ttu-id="dfb46-131">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="dfb46-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="dfb46-132">请求</span><span class="sxs-lookup"><span data-stu-id="dfb46-132">Request</span></span>
<span data-ttu-id="dfb46-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dfb46-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="dfb46-134">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="dfb46-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "range_lastcolumn"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/LastColumn
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dfb46-135">C#</span><span class="sxs-lookup"><span data-stu-id="dfb46-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-lastcolumn-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dfb46-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dfb46-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-lastcolumn-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dfb46-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="dfb46-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-lastcolumn-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="dfb46-138">Java</span><span class="sxs-lookup"><span data-stu-id="dfb46-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-lastcolumn-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="dfb46-139">响应</span><span class="sxs-lookup"><span data-stu-id="dfb46-139">Response</span></span>
<span data-ttu-id="dfb46-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dfb46-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Range: LastColumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
