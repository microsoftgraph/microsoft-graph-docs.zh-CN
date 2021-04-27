---
title: 'workbookRange: columnsAfter'
description: 获取给定范围右侧的一定数量的列。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: b1b42f977c2c5d85eaf6295e204d293cf6c1feea
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52036056"
---
# <a name="workbookrange-columnsafter"></a><span data-ttu-id="520e5-103">workbookRange: columnsAfter</span><span class="sxs-lookup"><span data-stu-id="520e5-103">workbookRange: columnsAfter</span></span>

<span data-ttu-id="520e5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="520e5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="520e5-105">获取给定范围右侧的一定数量的列。</span><span class="sxs-lookup"><span data-stu-id="520e5-105">Gets a certain number of columns to the right of the given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="520e5-106">权限</span><span class="sxs-lookup"><span data-stu-id="520e5-106">Permissions</span></span>
<span data-ttu-id="520e5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="520e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="520e5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="520e5-109">Permission type</span></span>      | <span data-ttu-id="520e5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="520e5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="520e5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="520e5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="520e5-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="520e5-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="520e5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="520e5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="520e5-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="520e5-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="520e5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="520e5-115">Application</span></span> | <span data-ttu-id="520e5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="520e5-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="520e5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="520e5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id}/range/columnsAfter(count=n)
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id}/range/columnsAfter(count=n)

```
## <a name="function-parameters"></a><span data-ttu-id="520e5-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="520e5-118">Function parameters</span></span>

| <span data-ttu-id="520e5-119">参数</span><span class="sxs-lookup"><span data-stu-id="520e5-119">Parameter</span></span>    | <span data-ttu-id="520e5-120">类型</span><span class="sxs-lookup"><span data-stu-id="520e5-120">Type</span></span>   |<span data-ttu-id="520e5-121">说明</span><span class="sxs-lookup"><span data-stu-id="520e5-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="520e5-122">count</span><span class="sxs-lookup"><span data-stu-id="520e5-122">count</span></span>|<span data-ttu-id="520e5-123">Int32</span><span class="sxs-lookup"><span data-stu-id="520e5-123">Int32</span></span>|<span data-ttu-id="520e5-p102">生成的范围中要包含的列数。一般来说，使用正数可以在当前范围之外创建一个范围。也可以使用负数在当前范围之内创建一个范围。默认值为 1</span><span class="sxs-lookup"><span data-stu-id="520e5-p102">The number of columns to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1</span></span>|

## <a name="request-headers"></a><span data-ttu-id="520e5-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="520e5-128">Request headers</span></span>
| <span data-ttu-id="520e5-129">名称</span><span class="sxs-lookup"><span data-stu-id="520e5-129">Name</span></span>       | <span data-ttu-id="520e5-130">说明</span><span class="sxs-lookup"><span data-stu-id="520e5-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="520e5-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="520e5-131">Authorization</span></span>  | <span data-ttu-id="520e5-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="520e5-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="520e5-134">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="520e5-134">Workbook-Session-Id</span></span>  | <span data-ttu-id="520e5-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="520e5-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="520e5-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="520e5-137">Request body</span></span>
<span data-ttu-id="520e5-138">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="520e5-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="520e5-139">响应</span><span class="sxs-lookup"><span data-stu-id="520e5-139">Response</span></span>

<span data-ttu-id="520e5-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [workbookRange](../resources/workbookrange.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="520e5-140">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="520e5-141">示例</span><span class="sxs-lookup"><span data-stu-id="520e5-141">Example</span></span>
<span data-ttu-id="520e5-142">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="520e5-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="520e5-143">请求</span><span class="sxs-lookup"><span data-stu-id="520e5-143">Request</span></span>
<span data-ttu-id="520e5-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="520e5-144">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="520e5-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="520e5-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "workbookrange_columnsafter"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range/columnsAfter(count=2)
```
# <a name="c"></a>[<span data-ttu-id="520e5-146">C#</span><span class="sxs-lookup"><span data-stu-id="520e5-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrange-columnsafter-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="520e5-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="520e5-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrange-columnsafter-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="520e5-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="520e5-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrange-columnsafter-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="520e5-149">Java</span><span class="sxs-lookup"><span data-stu-id="520e5-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookrange-columnsafter-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="520e5-150">响应</span><span class="sxs-lookup"><span data-stu-id="520e5-150">Response</span></span>
<span data-ttu-id="520e5-151">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="520e5-151">Here is an example of the response.</span></span> <span data-ttu-id="520e5-152">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="520e5-152">Note: The response object shown here might be shortened for readability.</span></span>
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


