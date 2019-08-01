---
title: Range:UsedRange
description: 返回指定 range 对象的所用范围。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 0743237a118be88b99e96fb8fb7967564381ac37
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36025279"
---
# <a name="range-usedrange"></a><span data-ttu-id="1e747-103">Range:UsedRange</span><span class="sxs-lookup"><span data-stu-id="1e747-103">Range: UsedRange</span></span>

<span data-ttu-id="1e747-104">返回指定 range 对象的所用范围。</span><span class="sxs-lookup"><span data-stu-id="1e747-104">Returns the used range of the given range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1e747-105">权限</span><span class="sxs-lookup"><span data-stu-id="1e747-105">Permissions</span></span>
<span data-ttu-id="1e747-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1e747-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e747-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="1e747-108">Permission type</span></span>      | <span data-ttu-id="1e747-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1e747-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e747-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1e747-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1e747-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1e747-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1e747-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1e747-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e747-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="1e747-113">Not supported.</span></span>    |
|<span data-ttu-id="1e747-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="1e747-114">Application</span></span> | <span data-ttu-id="1e747-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1e747-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1e747-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1e747-116">HTTP request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1e747-117">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="1e747-117">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/usedRange
GET /workbook/worksheets/{id|name}/range(address='<address>')/usedRange
GET /workbook/tables/{id|name}/columns/{id|name}/range/usedRange

```
## <a name="request-headers"></a><span data-ttu-id="1e747-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="1e747-118">Request headers</span></span>
| <span data-ttu-id="1e747-119">名称</span><span class="sxs-lookup"><span data-stu-id="1e747-119">Name</span></span>       | <span data-ttu-id="1e747-120">说明</span><span class="sxs-lookup"><span data-stu-id="1e747-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1e747-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e747-121">Authorization</span></span>  | <span data-ttu-id="1e747-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1e747-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1e747-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1e747-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="1e747-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="1e747-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="1e747-127">路径参数</span><span class="sxs-lookup"><span data-stu-id="1e747-127">Path parameters</span></span>
| <span data-ttu-id="1e747-128">参数</span><span class="sxs-lookup"><span data-stu-id="1e747-128">Parameter</span></span>    | <span data-ttu-id="1e747-129">类型</span><span class="sxs-lookup"><span data-stu-id="1e747-129">Type</span></span>   |<span data-ttu-id="1e747-130">说明</span><span class="sxs-lookup"><span data-stu-id="1e747-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1e747-131">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="1e747-131">valuesOnly</span></span>|<span data-ttu-id="1e747-132">布尔</span><span class="sxs-lookup"><span data-stu-id="1e747-132">boolean</span></span>|<span data-ttu-id="1e747-p104">可选。仅将有值的单元格视为已使用的单元格。</span><span class="sxs-lookup"><span data-stu-id="1e747-p104">Optional. Considers only cells with values as used cells.</span></span>|

## <a name="response"></a><span data-ttu-id="1e747-135">响应</span><span class="sxs-lookup"><span data-stu-id="1e747-135">Response</span></span>

<span data-ttu-id="1e747-136">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1e747-136">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e747-137">示例</span><span class="sxs-lookup"><span data-stu-id="1e747-137">Example</span></span>
<span data-ttu-id="1e747-138">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="1e747-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1e747-139">请求</span><span class="sxs-lookup"><span data-stu-id="1e747-139">Request</span></span>
<span data-ttu-id="1e747-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1e747-140">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_usedrange"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/usedRange
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1e747-141">C#</span><span class="sxs-lookup"><span data-stu-id="1e747-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-usedrange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1e747-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="1e747-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-usedrange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1e747-143">目标-C</span><span class="sxs-lookup"><span data-stu-id="1e747-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-usedrange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1e747-144">Java</span><span class="sxs-lookup"><span data-stu-id="1e747-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-usedrange-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1e747-145">响应</span><span class="sxs-lookup"><span data-stu-id="1e747-145">Response</span></span>
<span data-ttu-id="1e747-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1e747-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1e747-149">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="1e747-149">HTTP</span></span>](#tab/http)
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

<span data-ttu-id="1e747-150">下面是一个指定可选`valuesOnly`参数的示例。</span><span class="sxs-lookup"><span data-stu-id="1e747-150">Here is an example specifying the optional `valuesOnly` parameter.</span></span>

##### <a name="request"></a><span data-ttu-id="1e747-151">请求</span><span class="sxs-lookup"><span data-stu-id="1e747-151">Request</span></span>
<span data-ttu-id="1e747-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1e747-152">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_usedrange_valuesonly"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/usedRange(valuesOnly=true)
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1e747-153">C#</span><span class="sxs-lookup"><span data-stu-id="1e747-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-usedrange-valuesonly-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1e747-154">Javascript</span><span class="sxs-lookup"><span data-stu-id="1e747-154">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-usedrange-valuesonly-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1e747-155">目标-C</span><span class="sxs-lookup"><span data-stu-id="1e747-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-usedrange-valuesonly-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1e747-156">Java</span><span class="sxs-lookup"><span data-stu-id="1e747-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-usedrange-valuesonly-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1e747-157">响应</span><span class="sxs-lookup"><span data-stu-id="1e747-157">Response</span></span>

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
  "cellCount": 90,
  "columnCount": 90,
  "columnIndex": 90,
  "valueTypes": "valueTypes-value"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: UsedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
