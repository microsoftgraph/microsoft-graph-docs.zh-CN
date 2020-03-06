---
title: 'workbookRangeView: range'
description: 返回与 rangeView 资源相关联的范围。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 0eddeab46056555994c0da01bcf2874f044ffa24
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508707"
---
# <a name="workbookrangeview-range"></a><span data-ttu-id="07c66-103">workbookRangeView: range</span><span class="sxs-lookup"><span data-stu-id="07c66-103">workbookRangeView: range</span></span>

<span data-ttu-id="07c66-104">命名空间： microsoft. graph 返回与 rangeView 资源相关联的范围。</span><span class="sxs-lookup"><span data-stu-id="07c66-104">Namespace: microsoft.graph Return the range associated with the rangeView resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="07c66-105">权限</span><span class="sxs-lookup"><span data-stu-id="07c66-105">Permissions</span></span>
<span data-ttu-id="07c66-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="07c66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="07c66-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="07c66-108">Permission type</span></span>      | <span data-ttu-id="07c66-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="07c66-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="07c66-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="07c66-110">Delegated (work or school account)</span></span> | <span data-ttu-id="07c66-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="07c66-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="07c66-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="07c66-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07c66-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="07c66-113">Not supported.</span></span>    |
|<span data-ttu-id="07c66-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="07c66-114">Application</span></span> | <span data-ttu-id="07c66-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="07c66-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="07c66-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="07c66-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView/range

```
## <a name="request-headers"></a><span data-ttu-id="07c66-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="07c66-117">Request headers</span></span>
| <span data-ttu-id="07c66-118">名称</span><span class="sxs-lookup"><span data-stu-id="07c66-118">Name</span></span>       | <span data-ttu-id="07c66-119">说明</span><span class="sxs-lookup"><span data-stu-id="07c66-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="07c66-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="07c66-120">Authorization</span></span>  | <span data-ttu-id="07c66-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="07c66-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="07c66-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="07c66-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="07c66-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="07c66-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="07c66-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="07c66-126">Request body</span></span>

### <a name="response"></a><span data-ttu-id="07c66-127">响应</span><span class="sxs-lookup"><span data-stu-id="07c66-127">Response</span></span>
<span data-ttu-id="07c66-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [workbookRange](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="07c66-128">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07c66-129">示例</span><span class="sxs-lookup"><span data-stu-id="07c66-129">Example</span></span>
<span data-ttu-id="07c66-130">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="07c66-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="07c66-131">请求</span><span class="sxs-lookup"><span data-stu-id="07c66-131">Request</span></span>
<span data-ttu-id="07c66-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="07c66-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="07c66-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="07c66-133">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrangeview_range"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView/range
```
# <a name="c"></a>[<span data-ttu-id="07c66-134">C#</span><span class="sxs-lookup"><span data-stu-id="07c66-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrangeview-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="07c66-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="07c66-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrangeview-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="07c66-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="07c66-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrangeview-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="07c66-137">Java</span><span class="sxs-lookup"><span data-stu-id="07c66-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookrangeview-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="07c66-138">响应</span><span class="sxs-lookup"><span data-stu-id="07c66-138">Response</span></span>
<span data-ttu-id="07c66-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="07c66-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
