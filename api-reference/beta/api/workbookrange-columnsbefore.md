---
title: 'workbookRange: columnsBefore'
description: 获取给定范围左侧的一定数量的列。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: a7cfd3da52a8a045f4521d4d30883512708f0694
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48975928"
---
# <a name="workbookrange-columnsbefore"></a><span data-ttu-id="f3e7a-103">workbookRange: columnsBefore</span><span class="sxs-lookup"><span data-stu-id="f3e7a-103">workbookRange: columnsBefore</span></span>

<span data-ttu-id="f3e7a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3e7a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3e7a-105">获取给定范围左侧的一定数量的列。</span><span class="sxs-lookup"><span data-stu-id="f3e7a-105">Gets a certain number of columns to the left of the given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="f3e7a-106">权限</span><span class="sxs-lookup"><span data-stu-id="f3e7a-106">Permissions</span></span>
<span data-ttu-id="f3e7a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f3e7a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3e7a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f3e7a-109">Permission type</span></span>      | <span data-ttu-id="f3e7a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f3e7a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f3e7a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f3e7a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f3e7a-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f3e7a-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f3e7a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f3e7a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3e7a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f3e7a-114">Not supported.</span></span>    |
|<span data-ttu-id="f3e7a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f3e7a-115">Application</span></span> | <span data-ttu-id="f3e7a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f3e7a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f3e7a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f3e7a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/columnsBefore(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="f3e7a-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="f3e7a-118">Function parameters</span></span>

| <span data-ttu-id="f3e7a-119">参数</span><span class="sxs-lookup"><span data-stu-id="f3e7a-119">Parameter</span></span>    | <span data-ttu-id="f3e7a-120">类型</span><span class="sxs-lookup"><span data-stu-id="f3e7a-120">Type</span></span>   |<span data-ttu-id="f3e7a-121">说明</span><span class="sxs-lookup"><span data-stu-id="f3e7a-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f3e7a-122">count</span><span class="sxs-lookup"><span data-stu-id="f3e7a-122">count</span></span>|<span data-ttu-id="f3e7a-123">Int32</span><span class="sxs-lookup"><span data-stu-id="f3e7a-123">Int32</span></span>|<span data-ttu-id="f3e7a-p102">生成的范围中要包含的列数。一般来说，使用正数可以在当前范围之外创建一个范围。也可以使用负数在当前范围之内创建一个范围。默认值为 1。</span><span class="sxs-lookup"><span data-stu-id="f3e7a-p102">The number of columns to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="f3e7a-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="f3e7a-128">Request headers</span></span>
| <span data-ttu-id="f3e7a-129">名称</span><span class="sxs-lookup"><span data-stu-id="f3e7a-129">Name</span></span>       | <span data-ttu-id="f3e7a-130">说明</span><span class="sxs-lookup"><span data-stu-id="f3e7a-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f3e7a-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3e7a-131">Authorization</span></span>  | <span data-ttu-id="f3e7a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f3e7a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f3e7a-134">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f3e7a-134">Workbook-Session-Id</span></span>  | <span data-ttu-id="f3e7a-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="f3e7a-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3e7a-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="f3e7a-137">Request body</span></span>
<span data-ttu-id="f3e7a-138">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f3e7a-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f3e7a-139">响应</span><span class="sxs-lookup"><span data-stu-id="f3e7a-139">Response</span></span>
<span data-ttu-id="f3e7a-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [workbookRange](../resources/workbookrange.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f3e7a-140">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3e7a-141">示例</span><span class="sxs-lookup"><span data-stu-id="f3e7a-141">Example</span></span>
<span data-ttu-id="f3e7a-142">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="f3e7a-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f3e7a-143">请求</span><span class="sxs-lookup"><span data-stu-id="f3e7a-143">Request</span></span>
<span data-ttu-id="f3e7a-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f3e7a-144">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f3e7a-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="f3e7a-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "workbookrange_columnsbefore"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range/columnsBefore(count=2)
```
# <a name="c"></a>[<span data-ttu-id="f3e7a-146">C#</span><span class="sxs-lookup"><span data-stu-id="f3e7a-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrange-columnsbefore-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f3e7a-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f3e7a-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrange-columnsbefore-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f3e7a-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f3e7a-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrange-columnsbefore-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f3e7a-149">Java</span><span class="sxs-lookup"><span data-stu-id="f3e7a-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookrange-columnsbefore-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f3e7a-150">响应</span><span class="sxs-lookup"><span data-stu-id="f3e7a-150">Response</span></span>
<span data-ttu-id="f3e7a-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f3e7a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


