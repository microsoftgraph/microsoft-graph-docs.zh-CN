---
title: 'workbookRange: resizedRange'
description: 获取与当前范围对象类似的范围对象，但其右下角可通过一定数量的行和列进行展开（或合拢）。
ms.openlocfilehash: 167aef7a1d7c975298b80d9e27aad7043b276b35
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008495"
---
# <a name="workbookrange-resizedrange"></a><span data-ttu-id="e5955-103">workbookRange: resizedRange</span><span class="sxs-lookup"><span data-stu-id="e5955-103">workbookRange: resizedRange</span></span>
<span data-ttu-id="e5955-104">获取与当前范围对象类似的范围对象，但其右下角可通过一定数量的行和列进行展开（或合拢）。</span><span class="sxs-lookup"><span data-stu-id="e5955-104">Gets a range object similar to the current range object, but with its bottom-right corner expanded (or contracted) by some number of rows and columns.</span></span>

## <a name="permissions"></a><span data-ttu-id="e5955-105">权限</span><span class="sxs-lookup"><span data-stu-id="e5955-105">Permissions</span></span>
<span data-ttu-id="e5955-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e5955-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5955-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e5955-108">Permission type</span></span>      | <span data-ttu-id="e5955-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e5955-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5955-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e5955-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e5955-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e5955-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e5955-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e5955-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5955-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="e5955-113">Not supported.</span></span>    |
|<span data-ttu-id="e5955-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e5955-114">Application</span></span> | <span data-ttu-id="e5955-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e5955-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e5955-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e5955-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/resizedRange(deltaRows={n}, deltaColumns={n})

```

## <a name="function-parameters"></a><span data-ttu-id="e5955-117">函数参数</span><span class="sxs-lookup"><span data-stu-id="e5955-117">Function parameters</span></span>

| <span data-ttu-id="e5955-118">参数</span><span class="sxs-lookup"><span data-stu-id="e5955-118">Parameter</span></span>    | <span data-ttu-id="e5955-119">类型</span><span class="sxs-lookup"><span data-stu-id="e5955-119">Type</span></span>   |<span data-ttu-id="e5955-120">说明</span><span class="sxs-lookup"><span data-stu-id="e5955-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e5955-121">deltaRows</span><span class="sxs-lookup"><span data-stu-id="e5955-121">deltaRows</span></span>|<span data-ttu-id="e5955-122">Int32</span><span class="sxs-lookup"><span data-stu-id="e5955-122">Int32</span></span>|<span data-ttu-id="e5955-p102">相对于当前范围，右下角展开的行数。使用正数可展开范围，使用负数可合拢范围</span><span class="sxs-lookup"><span data-stu-id="e5955-p102">The number of rows by which to expand the bottom-right corner, relative to the current range. Use a positive number to expand the range, or a negative number to decrease it</span></span>|
|<span data-ttu-id="e5955-125">deltaColumns</span><span class="sxs-lookup"><span data-stu-id="e5955-125">deltaColumns</span></span>|<span data-ttu-id="e5955-126">Int32</span><span class="sxs-lookup"><span data-stu-id="e5955-126">Int32</span></span>|<span data-ttu-id="e5955-127">扩展的右下角，相对于当前范围的列数。</span><span class="sxs-lookup"><span data-stu-id="e5955-127">The number of columns by which to expand the bottom-right corner, relative to the current range.</span></span> <span data-ttu-id="e5955-128">使用扩展范围，为正数或负数降低它。</span><span class="sxs-lookup"><span data-stu-id="e5955-128">Use a positive number to expand the range, or a negative number to decrease it.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="e5955-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="e5955-129">Request headers</span></span>
| <span data-ttu-id="e5955-130">名称</span><span class="sxs-lookup"><span data-stu-id="e5955-130">Name</span></span>       | <span data-ttu-id="e5955-131">说明</span><span class="sxs-lookup"><span data-stu-id="e5955-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e5955-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5955-132">Authorization</span></span>  | <span data-ttu-id="e5955-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e5955-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e5955-135">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e5955-135">Workbook-Session-Id</span></span>  | <span data-ttu-id="e5955-p105">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="e5955-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5955-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="e5955-138">Request body</span></span>
<span data-ttu-id="e5955-139">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e5955-139">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="e5955-140">响应</span><span class="sxs-lookup"><span data-stu-id="e5955-140">Response</span></span>
<span data-ttu-id="e5955-141">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [workbookRange](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e5955-141">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5955-142">示例</span><span class="sxs-lookup"><span data-stu-id="e5955-142">Example</span></span>
<span data-ttu-id="e5955-143">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="e5955-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e5955-144">请求</span><span class="sxs-lookup"><span data-stu-id="e5955-144">Request</span></span>
<span data-ttu-id="e5955-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e5955-145">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_resizedrange",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/resizedRange(deltaRows={n}, deltaColumns={n})
```

##### <a name="response"></a><span data-ttu-id="e5955-146">响应</span><span class="sxs-lookup"><span data-stu-id="e5955-146">Response</span></span>
<span data-ttu-id="e5955-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e5955-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
