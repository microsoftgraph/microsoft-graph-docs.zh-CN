---
title: Worksheet:Range
description: 获取地址或名称指定的 range 对象。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: bacde9f1157533fc749fc6031b771f4973a307d0
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50578177"
---
# <a name="worksheet-range"></a><span data-ttu-id="c7ac0-103">Worksheet:Range</span><span class="sxs-lookup"><span data-stu-id="c7ac0-103">Worksheet: Range</span></span>

<span data-ttu-id="c7ac0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7ac0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7ac0-105">获取地址或名称指定的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="c7ac0-105">Gets the range object specified by the address or name.</span></span>
## <a name="permissions"></a><span data-ttu-id="c7ac0-106">权限</span><span class="sxs-lookup"><span data-stu-id="c7ac0-106">Permissions</span></span>
<span data-ttu-id="c7ac0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c7ac0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7ac0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c7ac0-109">Permission type</span></span>      | <span data-ttu-id="c7ac0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c7ac0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7ac0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c7ac0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c7ac0-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7ac0-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c7ac0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c7ac0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7ac0-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7ac0-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c7ac0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c7ac0-115">Application</span></span> | <span data-ttu-id="c7ac0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c7ac0-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c7ac0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c7ac0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/Range
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/Range

```
## <a name="request-headers"></a><span data-ttu-id="c7ac0-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="c7ac0-118">Request headers</span></span>
| <span data-ttu-id="c7ac0-119">名称</span><span class="sxs-lookup"><span data-stu-id="c7ac0-119">Name</span></span>       | <span data-ttu-id="c7ac0-120">说明</span><span class="sxs-lookup"><span data-stu-id="c7ac0-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c7ac0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7ac0-121">Authorization</span></span>  | <span data-ttu-id="c7ac0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c7ac0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c7ac0-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c7ac0-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="c7ac0-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="c7ac0-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7ac0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c7ac0-127">Request body</span></span>
<span data-ttu-id="c7ac0-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="c7ac0-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c7ac0-129">参数</span><span class="sxs-lookup"><span data-stu-id="c7ac0-129">Parameter</span></span>    | <span data-ttu-id="c7ac0-130">类型</span><span class="sxs-lookup"><span data-stu-id="c7ac0-130">Type</span></span>   |<span data-ttu-id="c7ac0-131">说明</span><span class="sxs-lookup"><span data-stu-id="c7ac0-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c7ac0-132">address</span><span class="sxs-lookup"><span data-stu-id="c7ac0-132">address</span></span>|<span data-ttu-id="c7ac0-133">string</span><span class="sxs-lookup"><span data-stu-id="c7ac0-133">string</span></span>|<span data-ttu-id="c7ac0-p104">可选。区域的地址或名称。如果未指定，则返回整个工作表区域。</span><span class="sxs-lookup"><span data-stu-id="c7ac0-p104">Optional. The address or the name of the range. If not specified, the entire worksheet range is returned.</span></span>|

## <a name="response"></a><span data-ttu-id="c7ac0-137">响应</span><span class="sxs-lookup"><span data-stu-id="c7ac0-137">Response</span></span>

<span data-ttu-id="c7ac0-138">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [workbookRange](../resources/workbookrange.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c7ac0-138">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7ac0-139">示例</span><span class="sxs-lookup"><span data-stu-id="c7ac0-139">Example</span></span>
<span data-ttu-id="c7ac0-140">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="c7ac0-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c7ac0-141">请求</span><span class="sxs-lookup"><span data-stu-id="c7ac0-141">Request</span></span>
<span data-ttu-id="c7ac0-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c7ac0-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c7ac0-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="c7ac0-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "worksheet_range"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/Range
Content-type: application/json
Content-length: 32

{
  "address": "address-value"
}
```
# <a name="c"></a>[<span data-ttu-id="c7ac0-144">C#</span><span class="sxs-lookup"><span data-stu-id="c7ac0-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheet-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c7ac0-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c7ac0-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheet-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c7ac0-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c7ac0-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheet-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c7ac0-147">Java</span><span class="sxs-lookup"><span data-stu-id="c7ac0-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheet-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c7ac0-148">响应</span><span class="sxs-lookup"><span data-stu-id="c7ac0-148">Response</span></span>
<span data-ttu-id="c7ac0-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c7ac0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Worksheet: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


