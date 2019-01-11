---
title: 'workbookRange: rowsAbove'
description: 获取给定范围上方的一定数量的行。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 0eb7a9ec6539854d4148148e2d283df0eaa366d9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875010"
---
# <a name="workbookrange-rowsabove"></a><span data-ttu-id="c00b2-103">workbookRange: rowsAbove</span><span class="sxs-lookup"><span data-stu-id="c00b2-103">workbookRange: rowsAbove</span></span>

<span data-ttu-id="c00b2-104">获取给定范围上方的一定数量的行。</span><span class="sxs-lookup"><span data-stu-id="c00b2-104">Gets a certain number of rows above a given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="c00b2-105">权限</span><span class="sxs-lookup"><span data-stu-id="c00b2-105">Permissions</span></span>
<span data-ttu-id="c00b2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c00b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c00b2-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c00b2-108">Permission type</span></span>      | <span data-ttu-id="c00b2-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c00b2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c00b2-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c00b2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c00b2-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c00b2-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c00b2-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c00b2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c00b2-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="c00b2-113">Not supported.</span></span>    |
|<span data-ttu-id="c00b2-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c00b2-114">Application</span></span> | <span data-ttu-id="c00b2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c00b2-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c00b2-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c00b2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/rowsAbove(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="c00b2-117">函数参数</span><span class="sxs-lookup"><span data-stu-id="c00b2-117">Function parameters</span></span>

| <span data-ttu-id="c00b2-118">参数</span><span class="sxs-lookup"><span data-stu-id="c00b2-118">Parameter</span></span>    | <span data-ttu-id="c00b2-119">类型</span><span class="sxs-lookup"><span data-stu-id="c00b2-119">Type</span></span>   |<span data-ttu-id="c00b2-120">说明</span><span class="sxs-lookup"><span data-stu-id="c00b2-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c00b2-121">count</span><span class="sxs-lookup"><span data-stu-id="c00b2-121">count</span></span>|<span data-ttu-id="c00b2-122">Int32</span><span class="sxs-lookup"><span data-stu-id="c00b2-122">Int32</span></span>|<span data-ttu-id="c00b2-p102">可选。生成的范围中要包含的行数。一般来说，使用正数可以在当前范围之外创建一个范围。也可以使用负数在当前范围之内创建一个范围。默认值为 1。</span><span class="sxs-lookup"><span data-stu-id="c00b2-p102">Optional. The number of rows to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="c00b2-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="c00b2-128">Request headers</span></span>
| <span data-ttu-id="c00b2-129">名称</span><span class="sxs-lookup"><span data-stu-id="c00b2-129">Name</span></span>       | <span data-ttu-id="c00b2-130">说明</span><span class="sxs-lookup"><span data-stu-id="c00b2-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c00b2-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="c00b2-131">Authorization</span></span>  | <span data-ttu-id="c00b2-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c00b2-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c00b2-134">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c00b2-134">Workbook-Session-Id</span></span>  | <span data-ttu-id="c00b2-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="c00b2-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c00b2-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="c00b2-137">Request body</span></span>
<span data-ttu-id="c00b2-138">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c00b2-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c00b2-139">响应</span><span class="sxs-lookup"><span data-stu-id="c00b2-139">Response</span></span>
<span data-ttu-id="c00b2-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [workbookRange](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c00b2-140">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c00b2-141">示例</span><span class="sxs-lookup"><span data-stu-id="c00b2-141">Example</span></span>
<span data-ttu-id="c00b2-142">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="c00b2-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c00b2-143">请求</span><span class="sxs-lookup"><span data-stu-id="c00b2-143">Request</span></span>
<span data-ttu-id="c00b2-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c00b2-144">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsAbove",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsAbove(count=2)
```

##### <a name="response"></a><span data-ttu-id="c00b2-145">响应</span><span class="sxs-lookup"><span data-stu-id="c00b2-145">Response</span></span>
<span data-ttu-id="c00b2-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c00b2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<span data-ttu-id="c00b2-149">如果调用不带可选`count`参数，此函数返回的区域上方的单个行。</span><span class="sxs-lookup"><span data-stu-id="c00b2-149">If called without the optional `count` parameter, this function returns the single row above the range.</span></span>

##### <a name="request"></a><span data-ttu-id="c00b2-150">请求</span><span class="sxs-lookup"><span data-stu-id="c00b2-150">Request</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsAbove_nocount",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsAbove
```

##### <a name="response"></a><span data-ttu-id="c00b2-151">响应</span><span class="sxs-lookup"><span data-stu-id="c00b2-151">Response</span></span>
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
