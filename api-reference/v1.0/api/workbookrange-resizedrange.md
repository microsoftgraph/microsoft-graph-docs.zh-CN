---
title: 'workbookRange: resizedRange'
description: 获取与当前范围对象类似的范围对象，但其右下角可通过一定数量的行和列进行展开（或合拢）。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 89dc3cf7635bb858cf1a818059e21a31c09da77a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055657"
---
# <a name="workbookrange-resizedrange"></a><span data-ttu-id="526f6-103">workbookRange: resizedRange</span><span class="sxs-lookup"><span data-stu-id="526f6-103">workbookRange: resizedRange</span></span>

<span data-ttu-id="526f6-104">命名空间：microsoft.graph 获取一个与当前 range 对象类似的 range 对象，但其右下角展开 (或按) 行和列数缩小。</span><span class="sxs-lookup"><span data-stu-id="526f6-104">Namespace: microsoft.graph Gets a range object similar to the current range object, but with its bottom-right corner expanded (or contracted) by some number of rows and columns.</span></span>

## <a name="permissions"></a><span data-ttu-id="526f6-105">权限</span><span class="sxs-lookup"><span data-stu-id="526f6-105">Permissions</span></span>
<span data-ttu-id="526f6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="526f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="526f6-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="526f6-108">Permission type</span></span>      | <span data-ttu-id="526f6-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="526f6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="526f6-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="526f6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="526f6-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="526f6-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="526f6-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="526f6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="526f6-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="526f6-113">Not supported.</span></span>    |
|<span data-ttu-id="526f6-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="526f6-114">Application</span></span> | <span data-ttu-id="526f6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="526f6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="526f6-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="526f6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/{id}/range/resizedRange(deltaRows={n}, deltaColumns={n})
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id}/range/resizedRange(deltaRows={n}, deltaColumns={n})

```

## <a name="function-parameters"></a><span data-ttu-id="526f6-117">函数参数</span><span class="sxs-lookup"><span data-stu-id="526f6-117">Function parameters</span></span>

| <span data-ttu-id="526f6-118">参数</span><span class="sxs-lookup"><span data-stu-id="526f6-118">Parameter</span></span>    | <span data-ttu-id="526f6-119">类型</span><span class="sxs-lookup"><span data-stu-id="526f6-119">Type</span></span>   |<span data-ttu-id="526f6-120">说明</span><span class="sxs-lookup"><span data-stu-id="526f6-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="526f6-121">deltaRows</span><span class="sxs-lookup"><span data-stu-id="526f6-121">deltaRows</span></span>|<span data-ttu-id="526f6-122">Int32</span><span class="sxs-lookup"><span data-stu-id="526f6-122">Int32</span></span>|<span data-ttu-id="526f6-p102">相对于当前范围，右下角展开的行数。使用正数可展开范围，使用负数可合拢范围</span><span class="sxs-lookup"><span data-stu-id="526f6-p102">The number of rows by which to expand the bottom-right corner, relative to the current range. Use a positive number to expand the range, or a negative number to decrease it</span></span>|
|<span data-ttu-id="526f6-125">deltaColumns</span><span class="sxs-lookup"><span data-stu-id="526f6-125">deltaColumns</span></span>|<span data-ttu-id="526f6-126">Int32</span><span class="sxs-lookup"><span data-stu-id="526f6-126">Int32</span></span>|<span data-ttu-id="526f6-127">相对于当前范围，右下角展开的列数。</span><span class="sxs-lookup"><span data-stu-id="526f6-127">The number of columns by which to expand the bottom-right corner, relative to the current range.</span></span> <span data-ttu-id="526f6-128">使用正数可展开范围，使用负数可合拢范围。</span><span class="sxs-lookup"><span data-stu-id="526f6-128">Use a positive number to expand the range, or a negative number to decrease it.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="526f6-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="526f6-129">Request headers</span></span>
| <span data-ttu-id="526f6-130">名称</span><span class="sxs-lookup"><span data-stu-id="526f6-130">Name</span></span>       | <span data-ttu-id="526f6-131">说明</span><span class="sxs-lookup"><span data-stu-id="526f6-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="526f6-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="526f6-132">Authorization</span></span>  | <span data-ttu-id="526f6-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="526f6-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="526f6-135">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="526f6-135">Workbook-Session-Id</span></span>  | <span data-ttu-id="526f6-p105">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="526f6-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="526f6-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="526f6-138">Request body</span></span>
<span data-ttu-id="526f6-139">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="526f6-139">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="526f6-140">响应</span><span class="sxs-lookup"><span data-stu-id="526f6-140">Response</span></span>
<span data-ttu-id="526f6-141">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [workbookRange](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="526f6-141">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="526f6-142">示例</span><span class="sxs-lookup"><span data-stu-id="526f6-142">Example</span></span>
<span data-ttu-id="526f6-143">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="526f6-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="526f6-144">请求</span><span class="sxs-lookup"><span data-stu-id="526f6-144">Request</span></span>
<span data-ttu-id="526f6-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="526f6-145">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_resizedrange",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/resizedRange(deltaRows={n}, deltaColumns={n})
```

##### <a name="response"></a><span data-ttu-id="526f6-146">响应</span><span class="sxs-lookup"><span data-stu-id="526f6-146">Response</span></span>
<span data-ttu-id="526f6-147">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="526f6-147">Here is an example of the response.</span></span> <span data-ttu-id="526f6-148">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="526f6-148">Note: The response object shown here might be shortened for readability.</span></span>
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
  "description": "workbookRange: resizedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

