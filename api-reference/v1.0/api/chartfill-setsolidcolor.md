---
title: 'ChartFill: setSolidColor'
description: 将图表元素的填充格式设置为统一颜色。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: e2b0b99cd3ac431b15257b3698fc050822989e93
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50573717"
---
# <a name="chartfill-setsolidcolor"></a><span data-ttu-id="f8dac-103">ChartFill: setSolidColor</span><span class="sxs-lookup"><span data-stu-id="f8dac-103">ChartFill: setSolidColor</span></span>

<span data-ttu-id="f8dac-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8dac-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f8dac-105">将图表元素的填充格式设置为统一颜色。</span><span class="sxs-lookup"><span data-stu-id="f8dac-105">Sets the fill formatting of a chart element to a uniform color.</span></span>
## <a name="permissions"></a><span data-ttu-id="f8dac-106">权限</span><span class="sxs-lookup"><span data-stu-id="f8dac-106">Permissions</span></span>
<span data-ttu-id="f8dac-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f8dac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8dac-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f8dac-109">Permission type</span></span>      | <span data-ttu-id="f8dac-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f8dac-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f8dac-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f8dac-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f8dac-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f8dac-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f8dac-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f8dac-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8dac-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f8dac-114">Not supported.</span></span>    |
|<span data-ttu-id="f8dac-115">Application</span><span class="sxs-lookup"><span data-stu-id="f8dac-115">Application</span></span> | <span data-ttu-id="f8dac-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f8dac-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f8dac-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f8dac-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/format/fill/setSolidColor
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/format/fill/setSolidColor
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/title/format/fill/setSolidColor
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/title/format/fill/setSolidColor
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/legend/format/fill/setSolidColor
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/legend/format/fill/setSolidColor

```
## <a name="request-headers"></a><span data-ttu-id="f8dac-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f8dac-118">Request headers</span></span>
| <span data-ttu-id="f8dac-119">名称</span><span class="sxs-lookup"><span data-stu-id="f8dac-119">Name</span></span>       | <span data-ttu-id="f8dac-120">说明</span><span class="sxs-lookup"><span data-stu-id="f8dac-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f8dac-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8dac-121">Authorization</span></span>  | <span data-ttu-id="f8dac-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f8dac-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f8dac-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f8dac-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="f8dac-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="f8dac-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8dac-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f8dac-127">Request body</span></span>
<span data-ttu-id="f8dac-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="f8dac-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f8dac-129">参数</span><span class="sxs-lookup"><span data-stu-id="f8dac-129">Parameter</span></span>    | <span data-ttu-id="f8dac-130">类型</span><span class="sxs-lookup"><span data-stu-id="f8dac-130">Type</span></span>   |<span data-ttu-id="f8dac-131">说明</span><span class="sxs-lookup"><span data-stu-id="f8dac-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f8dac-132">color</span><span class="sxs-lookup"><span data-stu-id="f8dac-132">color</span></span>|<span data-ttu-id="f8dac-133">string</span><span class="sxs-lookup"><span data-stu-id="f8dac-133">string</span></span>|<span data-ttu-id="f8dac-134">表示窗体 #RRGGBB（例如“FFA500”）的边框线条颜色或作为已命名的 HTML 颜色（例如“orange”）的 HTML 颜色代码。</span><span class="sxs-lookup"><span data-stu-id="f8dac-134">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|

## <a name="response"></a><span data-ttu-id="f8dac-135">响应</span><span class="sxs-lookup"><span data-stu-id="f8dac-135">Response</span></span>

<span data-ttu-id="f8dac-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f8dac-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8dac-138">示例</span><span class="sxs-lookup"><span data-stu-id="f8dac-138">Example</span></span>
<span data-ttu-id="f8dac-139">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="f8dac-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f8dac-140">请求</span><span class="sxs-lookup"><span data-stu-id="f8dac-140">Request</span></span>
<span data-ttu-id="f8dac-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f8dac-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f8dac-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="f8dac-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chartfill_setsolidcolor"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/format/fill/setSolidColor
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```
# <a name="c"></a>[<span data-ttu-id="f8dac-143">C#</span><span class="sxs-lookup"><span data-stu-id="f8dac-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chartfill-setsolidcolor-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f8dac-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f8dac-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chartfill-setsolidcolor-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f8dac-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f8dac-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chartfill-setsolidcolor-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f8dac-146">Java</span><span class="sxs-lookup"><span data-stu-id="f8dac-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chartfill-setsolidcolor-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f8dac-147">响应</span><span class="sxs-lookup"><span data-stu-id="f8dac-147">Response</span></span>
<span data-ttu-id="f8dac-148">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f8dac-148">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartFill: setSolidColor",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

