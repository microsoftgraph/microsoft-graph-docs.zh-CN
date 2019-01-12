---
title: 'workbookRange: rowsBelow'
description: 获取给定范围下方的一定数量的行。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 3b0f4add673d7bf6a8e976b037c39256e69be72d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991690"
---
# <a name="workbookrange-rowsbelow"></a><span data-ttu-id="912af-103">workbookRange: rowsBelow</span><span class="sxs-lookup"><span data-stu-id="912af-103">workbookRange: rowsBelow</span></span>

<span data-ttu-id="912af-104">获取给定范围下方的一定数量的行。</span><span class="sxs-lookup"><span data-stu-id="912af-104">Gets certain number of rows below a given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="912af-105">权限</span><span class="sxs-lookup"><span data-stu-id="912af-105">Permissions</span></span>
<span data-ttu-id="912af-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="912af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="912af-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="912af-108">Permission type</span></span>      | <span data-ttu-id="912af-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="912af-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="912af-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="912af-110">Delegated (work or school account)</span></span> | <span data-ttu-id="912af-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="912af-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="912af-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="912af-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="912af-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="912af-113">Not supported.</span></span>    |
|<span data-ttu-id="912af-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="912af-114">Application</span></span> | <span data-ttu-id="912af-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="912af-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="912af-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="912af-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="912af-117">函数参数</span><span class="sxs-lookup"><span data-stu-id="912af-117">Function parameters</span></span>

| <span data-ttu-id="912af-118">参数</span><span class="sxs-lookup"><span data-stu-id="912af-118">Parameter</span></span>    | <span data-ttu-id="912af-119">类型</span><span class="sxs-lookup"><span data-stu-id="912af-119">Type</span></span>   |<span data-ttu-id="912af-120">说明</span><span class="sxs-lookup"><span data-stu-id="912af-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="912af-121">count</span><span class="sxs-lookup"><span data-stu-id="912af-121">count</span></span>|<span data-ttu-id="912af-122">Int32</span><span class="sxs-lookup"><span data-stu-id="912af-122">Int32</span></span>| <span data-ttu-id="912af-p102">可选。生成的范围中要包含的行数。一般来说，使用正数可以在当前范围之外创建一个范围。也可以使用负数在当前范围之内创建一个范围。默认值为 1。</span><span class="sxs-lookup"><span data-stu-id="912af-p102">Optional. The number of rows to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="912af-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="912af-128">Request headers</span></span>
| <span data-ttu-id="912af-129">名称</span><span class="sxs-lookup"><span data-stu-id="912af-129">Name</span></span>       | <span data-ttu-id="912af-130">说明</span><span class="sxs-lookup"><span data-stu-id="912af-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="912af-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="912af-131">Authorization</span></span>  | <span data-ttu-id="912af-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="912af-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="912af-134">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="912af-134">Workbook-Session-Id</span></span>  | <span data-ttu-id="912af-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="912af-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="912af-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="912af-137">Request body</span></span>
<span data-ttu-id="912af-138">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="912af-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="912af-139">响应</span><span class="sxs-lookup"><span data-stu-id="912af-139">Response</span></span>
<span data-ttu-id="912af-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [workbookRange](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="912af-140">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="912af-141">示例</span><span class="sxs-lookup"><span data-stu-id="912af-141">Example</span></span>
<span data-ttu-id="912af-142">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="912af-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="912af-143">请求</span><span class="sxs-lookup"><span data-stu-id="912af-143">Request</span></span>
<span data-ttu-id="912af-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="912af-144">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsBelow",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=2)
```

##### <a name="response"></a><span data-ttu-id="912af-145">响应</span><span class="sxs-lookup"><span data-stu-id="912af-145">Response</span></span>
<span data-ttu-id="912af-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="912af-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<span data-ttu-id="912af-149">如果调用不带`count`参数，此函数将默认为一行。</span><span class="sxs-lookup"><span data-stu-id="912af-149">If called without the `count` parameter, this function defaults to one row.</span></span>

##### <a name="request"></a><span data-ttu-id="912af-150">请求</span><span class="sxs-lookup"><span data-stu-id="912af-150">Request</span></span>
<span data-ttu-id="912af-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="912af-151">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsBelow_nocount",
  "idempotent": true
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsBelow
```

##### <a name="response"></a><span data-ttu-id="912af-152">响应</span><span class="sxs-lookup"><span data-stu-id="912af-152">Response</span></span>
<span data-ttu-id="912af-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="912af-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnHidden": true,
  "columnIndex": 99
}
```
