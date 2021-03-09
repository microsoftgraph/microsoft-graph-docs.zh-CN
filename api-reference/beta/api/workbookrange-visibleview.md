---
title: 'workbookRange: visibleView'
description: 调用此 API 需要以下权限之一。 要了解详细信息（包括如何选择权限），请参阅权限。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 1e80f4debc42b1051f4abf6f873933e44c17a12a
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50575145"
---
# <a name="workbookrange-visibleview"></a><span data-ttu-id="e5d54-104">workbookRange: visibleView</span><span class="sxs-lookup"><span data-stu-id="e5d54-104">workbookRange: visibleView</span></span>

<span data-ttu-id="e5d54-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5d54-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="permissions"></a><span data-ttu-id="e5d54-106">权限</span><span class="sxs-lookup"><span data-stu-id="e5d54-106">Permissions</span></span>
<span data-ttu-id="e5d54-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e5d54-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5d54-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e5d54-109">Permission type</span></span>      | <span data-ttu-id="e5d54-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e5d54-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5d54-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e5d54-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e5d54-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e5d54-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e5d54-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e5d54-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5d54-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e5d54-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e5d54-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e5d54-115">Application</span></span> | <span data-ttu-id="e5d54-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e5d54-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e5d54-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e5d54-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id}/range(address={address})/visibleView
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id}/range(address={address})/visibleView
```
## <a name="request-headers"></a><span data-ttu-id="e5d54-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e5d54-118">Request headers</span></span>
| <span data-ttu-id="e5d54-119">名称</span><span class="sxs-lookup"><span data-stu-id="e5d54-119">Name</span></span>       | <span data-ttu-id="e5d54-120">说明</span><span class="sxs-lookup"><span data-stu-id="e5d54-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e5d54-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5d54-121">Authorization</span></span>  | <span data-ttu-id="e5d54-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e5d54-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e5d54-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e5d54-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="e5d54-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="e5d54-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5d54-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e5d54-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="e5d54-128">响应</span><span class="sxs-lookup"><span data-stu-id="e5d54-128">Response</span></span>

<span data-ttu-id="e5d54-129">如果成功，此方法在响应正文中返回 `200 OK`响应代码和 [workbookRangeView](../resources/workbookrangeview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e5d54-129">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5d54-130">示例</span><span class="sxs-lookup"><span data-stu-id="e5d54-130">Example</span></span>
<span data-ttu-id="e5d54-131">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="e5d54-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e5d54-132">请求</span><span class="sxs-lookup"><span data-stu-id="e5d54-132">Request</span></span>
<span data-ttu-id="e5d54-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e5d54-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e5d54-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="e5d54-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "workbookrange_visibleview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView
```
# <a name="c"></a>[<span data-ttu-id="e5d54-135">C#</span><span class="sxs-lookup"><span data-stu-id="e5d54-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrange-visibleview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e5d54-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e5d54-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrange-visibleview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e5d54-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e5d54-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrange-visibleview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e5d54-138">Java</span><span class="sxs-lookup"><span data-stu-id="e5d54-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookrange-visibleview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e5d54-139">响应</span><span class="sxs-lookup"><span data-stu-id="e5d54-139">Response</span></span>
<span data-ttu-id="e5d54-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e5d54-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


