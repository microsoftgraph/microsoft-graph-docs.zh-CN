---
title: 'workbookRange: visibleView'
description: 若要调用此 API, 必须有以下权限之一。 若要了解详细信息，包括如何选择权限的信息，请参阅权限。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: c2df35a9c34a69b028bbeb02da04cd9258df72fb
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36728914"
---
# <a name="workbookrange-visibleview"></a><span data-ttu-id="63f56-104">workbookRange: visibleView</span><span class="sxs-lookup"><span data-stu-id="63f56-104">workbookRange: visibleView</span></span>


## <a name="permissions"></a><span data-ttu-id="63f56-105">权限</span><span class="sxs-lookup"><span data-stu-id="63f56-105">Permissions</span></span>
<span data-ttu-id="63f56-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="63f56-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63f56-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="63f56-108">Permission type</span></span>      | <span data-ttu-id="63f56-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="63f56-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="63f56-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="63f56-110">Delegated (work or school account)</span></span> | <span data-ttu-id="63f56-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="63f56-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="63f56-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="63f56-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63f56-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="63f56-113">Not supported.</span></span>    |
|<span data-ttu-id="63f56-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="63f56-114">Application</span></span> | <span data-ttu-id="63f56-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="63f56-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="63f56-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="63f56-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView
```
## <a name="request-headers"></a><span data-ttu-id="63f56-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="63f56-117">Request headers</span></span>
| <span data-ttu-id="63f56-118">名称</span><span class="sxs-lookup"><span data-stu-id="63f56-118">Name</span></span>       | <span data-ttu-id="63f56-119">说明</span><span class="sxs-lookup"><span data-stu-id="63f56-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="63f56-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="63f56-120">Authorization</span></span>  | <span data-ttu-id="63f56-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="63f56-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="63f56-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="63f56-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="63f56-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="63f56-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="63f56-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="63f56-126">Request body</span></span>

### <a name="response"></a><span data-ttu-id="63f56-127">响应</span><span class="sxs-lookup"><span data-stu-id="63f56-127">Response</span></span>
<span data-ttu-id="63f56-128">如果成功，此方法在响应正文中返回 `200 OK`响应代码和 [workbookRangeView](../resources/workbookrangeview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="63f56-128">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63f56-129">示例</span><span class="sxs-lookup"><span data-stu-id="63f56-129">Example</span></span>
<span data-ttu-id="63f56-130">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="63f56-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="63f56-131">请求</span><span class="sxs-lookup"><span data-stu-id="63f56-131">Request</span></span>
<span data-ttu-id="63f56-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="63f56-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="63f56-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="63f56-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "workbookrange_visibleview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="63f56-134">C#</span><span class="sxs-lookup"><span data-stu-id="63f56-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrange-visibleview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="63f56-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="63f56-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrange-visibleview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="63f56-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="63f56-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrange-visibleview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="63f56-137">Java</span><span class="sxs-lookup"><span data-stu-id="63f56-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookrange-visibleview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="63f56-138">响应</span><span class="sxs-lookup"><span data-stu-id="63f56-138">Response</span></span>
<span data-ttu-id="63f56-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="63f56-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
