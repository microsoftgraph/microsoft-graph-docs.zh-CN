---
title: Worksheet:UsedRange
description: 使用的区域是包含分配了值或格式化的任何单元格的最小区域。如果工作表为空，此函数将返回左上角的单元格。
localization_priority: Normal
ms.openlocfilehash: edbe1a45f22ec07b0225be70549a2a7d59faf7eb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894360"
---
# <a name="worksheet-usedrange"></a><span data-ttu-id="775e2-104">Worksheet:UsedRange</span><span class="sxs-lookup"><span data-stu-id="775e2-104">Worksheet: UsedRange</span></span>

<span data-ttu-id="775e2-p102">使用的区域是包含分配了值或格式化的任何单元格的最小区域。如果工作表为空，此函数将返回左上角的单元格。</span><span class="sxs-lookup"><span data-stu-id="775e2-p102">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>
## <a name="permissions"></a><span data-ttu-id="775e2-107">权限</span><span class="sxs-lookup"><span data-stu-id="775e2-107">Permissions</span></span>
<span data-ttu-id="775e2-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="775e2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="775e2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="775e2-110">Permission type</span></span>      | <span data-ttu-id="775e2-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="775e2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="775e2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="775e2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="775e2-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="775e2-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="775e2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="775e2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="775e2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="775e2-115">Not supported.</span></span>    |
|<span data-ttu-id="775e2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="775e2-116">Application</span></span> | <span data-ttu-id="775e2-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="775e2-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="775e2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="775e2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/usedRange

```

## <a name="function-parameters"></a><span data-ttu-id="775e2-119">函数参数</span><span class="sxs-lookup"><span data-stu-id="775e2-119">Function parameters</span></span>
<span data-ttu-id="775e2-120">在请求 URL 中，您可以提供可选参数。</span><span class="sxs-lookup"><span data-stu-id="775e2-120">In the request URL you may provide optional parameters.</span></span>

| <span data-ttu-id="775e2-121">参数</span><span class="sxs-lookup"><span data-stu-id="775e2-121">Parameter</span></span>    | <span data-ttu-id="775e2-122">类型</span><span class="sxs-lookup"><span data-stu-id="775e2-122">Type</span></span>   |<span data-ttu-id="775e2-123">说明</span><span class="sxs-lookup"><span data-stu-id="775e2-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="775e2-124">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="775e2-124">valuesOnly</span></span>|<span data-ttu-id="775e2-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="775e2-125">Boolean</span></span>|<span data-ttu-id="775e2-p104">可选。仅将具有值的单元格视为已使用的单元格（忽略格式）。</span><span class="sxs-lookup"><span data-stu-id="775e2-p104">Optional. Considers only cells with values as used cells (ignores formatting).</span></span>|

## <a name="request-headers"></a><span data-ttu-id="775e2-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="775e2-128">Request headers</span></span>
| <span data-ttu-id="775e2-129">名称</span><span class="sxs-lookup"><span data-stu-id="775e2-129">Name</span></span>       | <span data-ttu-id="775e2-130">说明</span><span class="sxs-lookup"><span data-stu-id="775e2-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="775e2-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="775e2-131">Authorization</span></span>  | <span data-ttu-id="775e2-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="775e2-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="775e2-134">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="775e2-134">Workbook-Session-Id</span></span>  | <span data-ttu-id="775e2-p106">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="775e2-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="775e2-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="775e2-137">Request body</span></span>
<span data-ttu-id="775e2-138">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="775e2-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="775e2-139">响应</span><span class="sxs-lookup"><span data-stu-id="775e2-139">Response</span></span>

<span data-ttu-id="775e2-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="775e2-140">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="775e2-141">示例</span><span class="sxs-lookup"><span data-stu-id="775e2-141">Example</span></span>
<span data-ttu-id="775e2-142">下面的示例展示了如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="775e2-142">Here is an example that shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="775e2-143">请求</span><span class="sxs-lookup"><span data-stu-id="775e2-143">Request</span></span>
<span data-ttu-id="775e2-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="775e2-144">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "worksheet_usedrange"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/usedRange
```

##### <a name="response"></a><span data-ttu-id="775e2-145">响应</span><span class="sxs-lookup"><span data-stu-id="775e2-145">Response</span></span>
<span data-ttu-id="775e2-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="775e2-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "addressLocal": "addressLocal-value"
}
```

<span data-ttu-id="775e2-149">此外，此函数可调用带有可选`valuesOnly`参数。</span><span class="sxs-lookup"><span data-stu-id="775e2-149">Alternatively, this function can be called with the optional `valuesOnly` parameter.</span></span>

##### <a name="request"></a><span data-ttu-id="775e2-150">请求</span><span class="sxs-lookup"><span data-stu-id="775e2-150">Request</span></span>
<span data-ttu-id="775e2-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="775e2-151">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "worksheet_usedrange_valuesonly"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/usedRange(valuesOnly=true)
```

##### <a name="response"></a><span data-ttu-id="775e2-152">响应</span><span class="sxs-lookup"><span data-stu-id="775e2-152">Response</span></span>
<span data-ttu-id="775e2-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="775e2-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
