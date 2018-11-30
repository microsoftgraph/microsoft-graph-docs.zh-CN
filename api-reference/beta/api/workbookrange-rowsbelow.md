---
title: 'workbookRange: rowsBelow'
description: 获取给定范围下方的一定数量的行。
ms.openlocfilehash: 530526a4a443d8a6d2985c9dea0724ed3f8c5b87
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042506"
---
# <a name="workbookrange-rowsbelow"></a><span data-ttu-id="d7687-103">workbookRange: rowsBelow</span><span class="sxs-lookup"><span data-stu-id="d7687-103">workbookRange: rowsBelow</span></span>

> <span data-ttu-id="d7687-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d7687-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d7687-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d7687-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d7687-106">获取给定范围下方的一定数量的行。</span><span class="sxs-lookup"><span data-stu-id="d7687-106">Gets certain number of rows below a given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="d7687-107">权限</span><span class="sxs-lookup"><span data-stu-id="d7687-107">Permissions</span></span>
<span data-ttu-id="d7687-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d7687-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7687-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d7687-110">Permission type</span></span>      | <span data-ttu-id="d7687-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d7687-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7687-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d7687-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d7687-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d7687-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d7687-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d7687-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7687-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d7687-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d7687-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d7687-116">Application</span></span> | <span data-ttu-id="d7687-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d7687-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7687-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d7687-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="d7687-119">函数参数</span><span class="sxs-lookup"><span data-stu-id="d7687-119">Function parameters</span></span>

| <span data-ttu-id="d7687-120">参数</span><span class="sxs-lookup"><span data-stu-id="d7687-120">Parameter</span></span>    | <span data-ttu-id="d7687-121">类型</span><span class="sxs-lookup"><span data-stu-id="d7687-121">Type</span></span>   |<span data-ttu-id="d7687-122">说明</span><span class="sxs-lookup"><span data-stu-id="d7687-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d7687-123">count</span><span class="sxs-lookup"><span data-stu-id="d7687-123">count</span></span>|<span data-ttu-id="d7687-124">Int32</span><span class="sxs-lookup"><span data-stu-id="d7687-124">Int32</span></span>|<span data-ttu-id="d7687-p103">可选。生成的范围中要包含的行数。一般来说，使用正数可以在当前范围之外创建一个范围。也可以使用负数在当前范围之内创建一个范围。默认值为 1。</span><span class="sxs-lookup"><span data-stu-id="d7687-p103">Optional. The number of rows to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="d7687-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="d7687-130">Request headers</span></span>
| <span data-ttu-id="d7687-131">名称</span><span class="sxs-lookup"><span data-stu-id="d7687-131">Name</span></span>       | <span data-ttu-id="d7687-132">说明</span><span class="sxs-lookup"><span data-stu-id="d7687-132">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d7687-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7687-133">Authorization</span></span>  | <span data-ttu-id="d7687-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d7687-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d7687-136">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d7687-136">Workbook-Session-Id</span></span>  | <span data-ttu-id="d7687-p105">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="d7687-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7687-139">请求正文</span><span class="sxs-lookup"><span data-stu-id="d7687-139">Request body</span></span>
<span data-ttu-id="d7687-140">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d7687-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d7687-141">响应</span><span class="sxs-lookup"><span data-stu-id="d7687-141">Response</span></span>

<span data-ttu-id="d7687-142">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [workbookRange](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d7687-142">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7687-143">示例</span><span class="sxs-lookup"><span data-stu-id="d7687-143">Example</span></span>
<span data-ttu-id="d7687-144">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="d7687-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d7687-145">请求</span><span class="sxs-lookup"><span data-stu-id="d7687-145">Request</span></span>
<span data-ttu-id="d7687-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d7687-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_rowsBelow"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=2)
```

##### <a name="response"></a><span data-ttu-id="d7687-147">响应</span><span class="sxs-lookup"><span data-stu-id="d7687-147">Response</span></span>
<span data-ttu-id="d7687-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d7687-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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