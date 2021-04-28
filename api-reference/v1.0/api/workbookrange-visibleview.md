---
title: 'workbookRange: visibleView'
description: 需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅权限。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: cc18dd61d7a1307c11e968a383d3e0ea72a64dc2
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055650"
---
# <a name="workbookrange-visibleview"></a><span data-ttu-id="58c5d-104">workbookRange: visibleView</span><span class="sxs-lookup"><span data-stu-id="58c5d-104">workbookRange: visibleView</span></span>

<span data-ttu-id="58c5d-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58c5d-105">Namespace: microsoft.graph</span></span>


## <a name="permissions"></a><span data-ttu-id="58c5d-106">权限</span><span class="sxs-lookup"><span data-stu-id="58c5d-106">Permissions</span></span>
<span data-ttu-id="58c5d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="58c5d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58c5d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="58c5d-109">Permission type</span></span>      | <span data-ttu-id="58c5d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="58c5d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="58c5d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="58c5d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="58c5d-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="58c5d-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="58c5d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="58c5d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58c5d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="58c5d-114">Not supported.</span></span>    |
|<span data-ttu-id="58c5d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="58c5d-115">Application</span></span> | <span data-ttu-id="58c5d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="58c5d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="58c5d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="58c5d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id}/range(address={address})/visibleView
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id}/range(address={address})/visibleView
```
## <a name="request-headers"></a><span data-ttu-id="58c5d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="58c5d-118">Request headers</span></span>
| <span data-ttu-id="58c5d-119">名称</span><span class="sxs-lookup"><span data-stu-id="58c5d-119">Name</span></span>       | <span data-ttu-id="58c5d-120">说明</span><span class="sxs-lookup"><span data-stu-id="58c5d-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="58c5d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="58c5d-121">Authorization</span></span>  | <span data-ttu-id="58c5d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="58c5d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="58c5d-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="58c5d-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="58c5d-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="58c5d-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="58c5d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="58c5d-127">Request body</span></span>

### <a name="response"></a><span data-ttu-id="58c5d-128">响应</span><span class="sxs-lookup"><span data-stu-id="58c5d-128">Response</span></span>
<span data-ttu-id="58c5d-129">如果成功，此方法在响应正文中返回 `200 OK`响应代码和 [workbookRangeView](../resources/workbookrangeview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="58c5d-129">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58c5d-130">示例</span><span class="sxs-lookup"><span data-stu-id="58c5d-130">Example</span></span>
<span data-ttu-id="58c5d-131">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="58c5d-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="58c5d-132">请求</span><span class="sxs-lookup"><span data-stu-id="58c5d-132">Request</span></span>
<span data-ttu-id="58c5d-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="58c5d-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="58c5d-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="58c5d-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "workbookrange_visibleview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView
```
# <a name="c"></a>[<span data-ttu-id="58c5d-135">C#</span><span class="sxs-lookup"><span data-stu-id="58c5d-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrange-visibleview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="58c5d-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="58c5d-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrange-visibleview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="58c5d-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="58c5d-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrange-visibleview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="58c5d-138">Java</span><span class="sxs-lookup"><span data-stu-id="58c5d-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookrange-visibleview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="58c5d-139">响应</span><span class="sxs-lookup"><span data-stu-id="58c5d-139">Response</span></span>
<span data-ttu-id="58c5d-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="58c5d-140">Here is an example of the response.</span></span> <span data-ttu-id="58c5d-141">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="58c5d-141">Note: The response object shown here might be shortened for readability.</span></span>
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

