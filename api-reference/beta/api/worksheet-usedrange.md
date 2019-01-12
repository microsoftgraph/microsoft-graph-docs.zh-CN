---
title: Worksheet:UsedRange
description: 使用的区域是包含分配了值或格式化的任何单元格的最小区域。如果工作表为空，此函数将返回左上角的单元格。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: b5aa23496abbad6f78768acf20a7cfd3411654d9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915100"
---
# <a name="worksheet-usedrange"></a><span data-ttu-id="12f3b-104">Worksheet:UsedRange</span><span class="sxs-lookup"><span data-stu-id="12f3b-104">Worksheet: UsedRange</span></span>

<span data-ttu-id="12f3b-p102">使用的区域是包含分配了值或格式化的任何单元格的最小区域。如果工作表为空，此函数将返回左上角的单元格。</span><span class="sxs-lookup"><span data-stu-id="12f3b-p102">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>
## <a name="permissions"></a><span data-ttu-id="12f3b-107">权限</span><span class="sxs-lookup"><span data-stu-id="12f3b-107">Permissions</span></span>
<span data-ttu-id="12f3b-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="12f3b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12f3b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="12f3b-110">Permission type</span></span>      | <span data-ttu-id="12f3b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="12f3b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="12f3b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="12f3b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="12f3b-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12f3b-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="12f3b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="12f3b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12f3b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="12f3b-115">Not supported.</span></span>    |
|<span data-ttu-id="12f3b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="12f3b-116">Application</span></span> | <span data-ttu-id="12f3b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="12f3b-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="12f3b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="12f3b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/UsedRange

```

## <a name="function-parameters"></a><span data-ttu-id="12f3b-119">函数参数</span><span class="sxs-lookup"><span data-stu-id="12f3b-119">Function parameters</span></span>
<span data-ttu-id="12f3b-120">在请求 URL 中，提供可选的查询参数。</span><span class="sxs-lookup"><span data-stu-id="12f3b-120">In the request URL, provide an optional query parameter.</span></span>

| <span data-ttu-id="12f3b-121">参数</span><span class="sxs-lookup"><span data-stu-id="12f3b-121">Parameter</span></span>    | <span data-ttu-id="12f3b-122">类型</span><span class="sxs-lookup"><span data-stu-id="12f3b-122">Type</span></span>   |<span data-ttu-id="12f3b-123">说明</span><span class="sxs-lookup"><span data-stu-id="12f3b-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="12f3b-124">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="12f3b-124">valuesOnly</span></span>|<span data-ttu-id="12f3b-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="12f3b-125">Boolean</span></span>|<span data-ttu-id="12f3b-p104">可选。仅将具有值的单元格视为已使用的单元格（忽略格式）。</span><span class="sxs-lookup"><span data-stu-id="12f3b-p104">Optional. Considers only cells with values as used cells (ignores formatting).</span></span>|

## <a name="request-headers"></a><span data-ttu-id="12f3b-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="12f3b-128">Request headers</span></span>
| <span data-ttu-id="12f3b-129">名称</span><span class="sxs-lookup"><span data-stu-id="12f3b-129">Name</span></span>       | <span data-ttu-id="12f3b-130">说明</span><span class="sxs-lookup"><span data-stu-id="12f3b-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="12f3b-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="12f3b-131">Authorization</span></span>  | <span data-ttu-id="12f3b-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="12f3b-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="12f3b-134">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="12f3b-134">Workbook-Session-Id</span></span>  | <span data-ttu-id="12f3b-p106">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="12f3b-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="12f3b-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="12f3b-137">Request body</span></span>
<span data-ttu-id="12f3b-138">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="12f3b-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12f3b-139">响应</span><span class="sxs-lookup"><span data-stu-id="12f3b-139">Response</span></span>

<span data-ttu-id="12f3b-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="12f3b-140">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12f3b-141">示例</span><span class="sxs-lookup"><span data-stu-id="12f3b-141">Example</span></span>
<span data-ttu-id="12f3b-142">下面的示例展示了如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="12f3b-142">Here is an example that shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="12f3b-143">请求</span><span class="sxs-lookup"><span data-stu-id="12f3b-143">Request</span></span>
<span data-ttu-id="12f3b-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="12f3b-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_usedrange"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/UsedRange(valuesOnly=true)
```

##### <a name="response"></a><span data-ttu-id="12f3b-145">响应</span><span class="sxs-lookup"><span data-stu-id="12f3b-145">Response</span></span>
<span data-ttu-id="12f3b-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="12f3b-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet: UsedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
