---
title: 'workbookRange: columnsAfter'
description: 获取给定范围右侧的一定数量的列。
author: lumine2008
ms.openlocfilehash: b80657c6afb7709049a1e0ccaa3c3b232f5501c7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304233"
---
# <a name="workbookrange-columnsafter"></a><span data-ttu-id="9b38a-103">workbookRange: columnsAfter</span><span class="sxs-lookup"><span data-stu-id="9b38a-103">workbookRange: columnsAfter</span></span>

<span data-ttu-id="9b38a-104">获取给定范围右侧的一定数量的列。</span><span class="sxs-lookup"><span data-stu-id="9b38a-104">Gets a certain number of columns to the right of the given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="9b38a-105">权限</span><span class="sxs-lookup"><span data-stu-id="9b38a-105">Permissions</span></span>
<span data-ttu-id="9b38a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9b38a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b38a-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9b38a-108">Permission type</span></span>      | <span data-ttu-id="9b38a-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9b38a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9b38a-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9b38a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9b38a-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9b38a-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9b38a-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9b38a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b38a-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="9b38a-113">Not supported.</span></span>    |
|<span data-ttu-id="9b38a-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="9b38a-114">Application</span></span> | <span data-ttu-id="9b38a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9b38a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9b38a-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9b38a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/columnsAfter(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="9b38a-117">函数参数</span><span class="sxs-lookup"><span data-stu-id="9b38a-117">Function parameters</span></span>

| <span data-ttu-id="9b38a-118">参数</span><span class="sxs-lookup"><span data-stu-id="9b38a-118">Parameter</span></span>    | <span data-ttu-id="9b38a-119">Type</span><span class="sxs-lookup"><span data-stu-id="9b38a-119">Type</span></span>   |<span data-ttu-id="9b38a-120">说明</span><span class="sxs-lookup"><span data-stu-id="9b38a-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9b38a-121">count</span><span class="sxs-lookup"><span data-stu-id="9b38a-121">count</span></span>|<span data-ttu-id="9b38a-122">Int32</span><span class="sxs-lookup"><span data-stu-id="9b38a-122">Int32</span></span>|<span data-ttu-id="9b38a-123">可选。</span><span class="sxs-lookup"><span data-stu-id="9b38a-123">Optional.</span></span> <span data-ttu-id="9b38a-124">要在结果区域中包括的列数。</span><span class="sxs-lookup"><span data-stu-id="9b38a-124">The number of columns to include in the resulting range.</span></span> <span data-ttu-id="9b38a-125">一般情况下，使用正数创建当前范围之外的范围。</span><span class="sxs-lookup"><span data-stu-id="9b38a-125">In general, use a positive number to create a range outside the current range.</span></span> <span data-ttu-id="9b38a-126">为负数还可用于创建当前范围内的范围。</span><span class="sxs-lookup"><span data-stu-id="9b38a-126">You can also use a negative number to create a range within the current range.</span></span> <span data-ttu-id="9b38a-127">默认值为 1</span><span class="sxs-lookup"><span data-stu-id="9b38a-127">The default value is 1</span></span>|

## <a name="request-headers"></a><span data-ttu-id="9b38a-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="9b38a-128">Request headers</span></span>
| <span data-ttu-id="9b38a-129">Name</span><span class="sxs-lookup"><span data-stu-id="9b38a-129">Name</span></span>       | <span data-ttu-id="9b38a-130">说明</span><span class="sxs-lookup"><span data-stu-id="9b38a-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9b38a-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b38a-131">Authorization</span></span>  | <span data-ttu-id="9b38a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9b38a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9b38a-134">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9b38a-134">Workbook-Session-Id</span></span>  | <span data-ttu-id="9b38a-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="9b38a-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b38a-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="9b38a-137">Request body</span></span>
<span data-ttu-id="9b38a-138">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9b38a-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9b38a-139">响应</span><span class="sxs-lookup"><span data-stu-id="9b38a-139">Response</span></span>
<span data-ttu-id="9b38a-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [workbookRange](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9b38a-140">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b38a-141">示例</span><span class="sxs-lookup"><span data-stu-id="9b38a-141">Example</span></span>
<span data-ttu-id="9b38a-142">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="9b38a-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9b38a-143">请求</span><span class="sxs-lookup"><span data-stu-id="9b38a-143">Request</span></span>
<span data-ttu-id="9b38a-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9b38a-144">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_columnsafter",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/columnsAfter(count=2)
```

##### <a name="response"></a><span data-ttu-id="9b38a-145">响应</span><span class="sxs-lookup"><span data-stu-id="9b38a-145">Response</span></span>
<span data-ttu-id="9b38a-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9b38a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
