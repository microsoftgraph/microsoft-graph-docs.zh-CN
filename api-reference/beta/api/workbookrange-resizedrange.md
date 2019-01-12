---
title: 'workbookRange: resizedRange'
description: 获取与当前范围对象类似的范围对象，但其右下角可通过一定数量的行和列进行展开（或合拢）。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 4068da86c1653a01a478d385c5c854c700e50ae9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931333"
---
# <a name="workbookrange-resizedrange"></a><span data-ttu-id="13300-103">workbookRange: resizedRange</span><span class="sxs-lookup"><span data-stu-id="13300-103">workbookRange: resizedRange</span></span>

> <span data-ttu-id="13300-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="13300-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="13300-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="13300-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="13300-106">获取与当前范围对象类似的范围对象，但其右下角可通过一定数量的行和列进行展开（或合拢）。</span><span class="sxs-lookup"><span data-stu-id="13300-106">Gets a range object similar to the current range object, but with its bottom-right corner expanded (or contracted) by some number of rows and columns.</span></span>

## <a name="permissions"></a><span data-ttu-id="13300-107">权限</span><span class="sxs-lookup"><span data-stu-id="13300-107">Permissions</span></span>
<span data-ttu-id="13300-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="13300-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13300-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="13300-110">Permission type</span></span>      | <span data-ttu-id="13300-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="13300-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="13300-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="13300-112">Delegated (work or school account)</span></span> | <span data-ttu-id="13300-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="13300-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="13300-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="13300-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13300-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="13300-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="13300-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="13300-116">Application</span></span> | <span data-ttu-id="13300-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="13300-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="13300-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="13300-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/resizedRange(deltaRows={n}, deltaColumns={n})

```

## <a name="function-parameters"></a><span data-ttu-id="13300-119">函数参数</span><span class="sxs-lookup"><span data-stu-id="13300-119">Function parameters</span></span>

| <span data-ttu-id="13300-120">参数</span><span class="sxs-lookup"><span data-stu-id="13300-120">Parameter</span></span>    | <span data-ttu-id="13300-121">类型</span><span class="sxs-lookup"><span data-stu-id="13300-121">Type</span></span>   |<span data-ttu-id="13300-122">说明</span><span class="sxs-lookup"><span data-stu-id="13300-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="13300-123">deltarows</span><span class="sxs-lookup"><span data-stu-id="13300-123">deltarows</span></span>|<span data-ttu-id="13300-124">Int32</span><span class="sxs-lookup"><span data-stu-id="13300-124">Int32</span></span>|<span data-ttu-id="13300-p103">相对于当前范围，右下角展开的行数。使用正数可展开范围，使用负数可合拢范围</span><span class="sxs-lookup"><span data-stu-id="13300-p103">The number of rows by which to expand the bottom-right corner, relative to the current range. Use a positive number to expand the range, or a negative number to decrease it</span></span>|
|<span data-ttu-id="13300-127">deltaColumns</span><span class="sxs-lookup"><span data-stu-id="13300-127">deltaColumns</span></span>|<span data-ttu-id="13300-128">Int32</span><span class="sxs-lookup"><span data-stu-id="13300-128">Int32</span></span>|<span data-ttu-id="13300-p104">相对于当前范围，右下角展开的列数。使用正数可展开范围，使用负数可合拢范围。</span><span class="sxs-lookup"><span data-stu-id="13300-p104">The number of columnsby which to expand the bottom-right corner, relative to the current range. Use a positive number to expand the range, or a negative number to decrease it.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="13300-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="13300-131">Request headers</span></span>
| <span data-ttu-id="13300-132">名称</span><span class="sxs-lookup"><span data-stu-id="13300-132">Name</span></span>       | <span data-ttu-id="13300-133">说明</span><span class="sxs-lookup"><span data-stu-id="13300-133">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="13300-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="13300-134">Authorization</span></span>  | <span data-ttu-id="13300-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="13300-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="13300-137">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="13300-137">Workbook-Session-Id</span></span>  | <span data-ttu-id="13300-p106">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="13300-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="13300-140">请求正文</span><span class="sxs-lookup"><span data-stu-id="13300-140">Request body</span></span>
<span data-ttu-id="13300-141">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="13300-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13300-142">响应</span><span class="sxs-lookup"><span data-stu-id="13300-142">Response</span></span>

<span data-ttu-id="13300-143">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [workbookRange](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="13300-143">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13300-144">示例</span><span class="sxs-lookup"><span data-stu-id="13300-144">Example</span></span>
<span data-ttu-id="13300-145">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="13300-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="13300-146">请求</span><span class="sxs-lookup"><span data-stu-id="13300-146">Request</span></span>
<span data-ttu-id="13300-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="13300-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_resizedrange"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range/resizedRange(deltarows={n}, deltaColumns={n})
```

##### <a name="response"></a><span data-ttu-id="13300-148">响应</span><span class="sxs-lookup"><span data-stu-id="13300-148">Response</span></span>
<span data-ttu-id="13300-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="13300-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
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
